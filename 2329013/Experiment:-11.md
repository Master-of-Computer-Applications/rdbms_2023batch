                                                          Experiment:-11
                                               Creating arrays and nested tables
	

Nested Tables In PL/SQL:-

The nested tables are like a single column database table or a 1-dimensional array where the array size is dynamic. 
Its subscript is of numeric type. We can get the nested table into a variable by giving the rows a subscript that begins with 1. This feature makes it similar in nature like an array.
A nested table can be held in a column of a database. It can also be used for manipulating SQL operations by joining tables. Since it is like a dynamic array so the upper limit can be of any size.
A nested table can have both dense and sparse collection characteristics which means any element can be deleted randomly (making it sparse) with the help of the DELETE procedure. The deletion of data causes a discontinuity in the index but the NEXT function helps to iterate to the next subscripts. Since the data is stored in the form of a table, it can be retrieved with the help of SELECT statements.
A nested table can be built at the schema level or in PL/SQL block. It is like a database object which is accessible within the database or subprogram.

Syntax of the nested table:

TYPE <<type>> IS TABLE OF <<element>> [NOT NULL];

Here, ‘type’ is the type specifier. ‘element’ is the data type.


Code implementation with the nested table:

DECLARE

    TYPE subject IS TABLE OF VARCHAR(15); 
    
    TYPE teacher IS TABLE OF VARCHAR2(20);
    
    subjectnames subject; 
    
    subjectteacher teacher; 
    
    summ integer; 
    
     BEGIN
 
    -- adding subject and its teachers to the table
    
    subjectnames := subject('PLSQL', 'SELENIUM', 'JMETER'); 
    
    subjectteacher:= teacher('Sashi', 'Mala', 'Mukund');
    
 
    -- returns count of number of elements in nested table
    
    summ:= subjectteacher.count;
 
    -- printing the content to the console
    
    dbms_output.put_line('Total Number of Teachers: '|| summ); 
    
    FOR i IN 1 .. summ LOOP 
    
         dbms_output.put_line('Subject:'||subjectnames(i)||', Teacher:' || subjectteacher(i)); 
         
    end loop; 
    
     END;

The output of the above code should be:
 


PL/SQL Arrays – VARRAY:-

In PL/SQL we have a varray named data structure which is a variable size array which can be used to store a fixed size of data elements of same type, sequentially, where the number of elements can vary from zero (empty) to the declared maximum size.
A varray stores data in contiguos memory locations where the first element is stored at the lowes address location and the last element is stored at the highest address location.
To access the data elements stored in a varray type variable, we use the syntax variable_name(index) where index starts from 1 for the first element and goes upto the current upper bound of elements which means the number of elements that exists at that given point(not the maximum size of the array).
The upper bound keeps on changing as you add or remove elements from an array, but it cannot exceed the maximum size of the array.
Whenever you store and fetch back a varray from the database, its indexes and the element order remain stable.
For example, in the diagram below we have a varray Marks of size 8 and 5 data elements are stored in it.
 
In the above varray Marks if you want to access the second element, all you need to do it Marks(2)
The database stores a varray variable as a single object. 
If a varray variable is less than 4 KB, it resides inside the table of which it is a column; otherwise, it resides outside the table but in the same tablespace.
________________________________________
Declaring a Varray Type:-
We can declare a new varray type using the TYPE statement inside the PL/SQL block.
TYPE varr_type_name IS VARRAY(n) of <element_type>
For example,

TYPE snamearray IS VARRAY(10) OF VARCHAR2(20);

Type sagearray IS VARRAY(10) OF INTEGER;

In the example above we have initialized two varray types, first one can hold 10 elements of type varchar and the second one can hold 10 elements of type integer.
An uninitialized varray variable is a null collection. You must initialize it, either by making it empty or by assigning a non-NULL value to it.
________________________________________
In the program below, we have used varray:

DECLARE 

   type snamesarray IS VARRAY(5) OF VARCHAR2(10); 
   
   type smarks IS VARRAY(5) OF INTEGER; 
   
BEGIN 

   snames namesarray := namesarray('John', 'Adam', 'Elly', 'Kate', 'Ron'); 
   
   marks smarks := smarks(42, 88, 62, 89, 97); 
   
   no_of_students := snames.count; 
   
   dbms_output.put_line('Total '|| no_of_students || ' Students'); 
   
   FOR i in 1 .. no_of_students LOOP 
   
      dbms_output.put_line('Student: ' || snames(i) || ' 
      
      Marks: ' || marks(i)); 
      
   END LOOP; 
   
     END; 

    /
    Copy

Total 5 Students 

Student: John  Marks: 42 

Student: Adam  Marks: 88 

Student: Elly  Marks: 62 

Student: Kate  Marks: 89 

Student: Ron  Marks: 97 


PL/SQL procedure successfully completed. 

As you can see in the example above, we have declared two varray types one for storing student names and another on for storing student's marks.
And then we have used them in our PL/SQL block for storing student names and student marks.
