                         Experiment:-10
                  Creating packages and applying triggers
Packages are schema objects that groups logically related PL/SQL types, variables, and subprograms.
A package will have two mandatory parts −
•	Package specification
•	Package body or definition
Package Specification:-

The specification is the interface to the package. It just DECLARES the types, variables, constants, exceptions, cursors, and subprograms that can be referenced from outside the package. In other words, it contains all information about the content of the package, but excludes the code for the subprograms.
All objects placed in the specification are called public objects. Any subprogram not in the package specification but coded in the package body is called a private object.
The following code snippet shows a package specification having a single procedure. You can have many global variables defined and multiple procedures or functions inside a package.

CREATE PACKAGE cust_sal AS 

   PROCEDURE find_sal(c_id customers.id%type); 
   
END cust_sal; 

/
When the above code is executed at the SQL prompt, it produces the following result −

Package created.

Package Body:-
The package body has the codes for various methods declared in the package specification and other private declarations, which are hidden from the code outside the package.
The CREATE PACKAGE BODY Statement is used for creating the package body.
The following code snippet shows the package body declaration for the cust_sal package created above.
I assumed that we already have CUSTOMERS table created in our database as mentioned in the PL/SQL - Variables chapter.

CREATE OR REPLACE PACKAGE BODY cust_sal AS  
   
   PROCEDURE find_sal(c_id customers.id%TYPE) IS 
   
   c_sal customers.salary%TYPE; 
   
   BEGIN 
   
      SELECT salary INTO c_sal 
      
      FROM customers 
      
            WHERE id = c_id;
            
      dbms_output.put_line('Salary: '|| c_sal); 
      
   END find_sal; 
   
END cust_sal; 

/

When the above code is executed at the SQL prompt, it produces the following result −
Package body created.
Using the Package Elements
The package elements (variables, procedures or functions) are accessed with the following syntax −
package_name.element_name;

Example
The following program provides a more complete package. We will use the CUSTOMERS table stored in our database with the following records −
Select * from customers;  


| ID | NAME     | AGE | ADDRESS   | SALARY   | 
|----|----|----|----|----|
|  1 | Ramesh   |  32 | Ahmedabad |  3000.00 | 
|  2 | Khilan   |  25 | Delhi     |  3000.00 | 
|  3 | kaushik  |  23 | Kota      |  3000.00 | 
|  4 | Chaitali |  25 | Mumbai    |  7500.00 | 
|  5 | Hardik   |  27 | Bhopal    |  9500.00 | 
|  6 | Komal    |  22 | MP        |  5500.00 | 


The Package Specification

CREATE OR REPLACE PACKAGE c_package AS 

   -- Adds a customer 
   
   PROCEDURE addCustomer(c_id   customers.id%type, 
   
   c_name customers.Name%type,
   
   c_age  customers.age%type, 
   
   c_addr customers.address%type,  
   
   c_sal  customers.salary%type); 
   
   
   -- Removes a customer 
   
   PROCEDURE delCustomer(c_id  customers.id%TYPE); 
   
   --Lists all customers 
   
   PROCEDURE listCustomer; 
   
  
END c_package; 

/
When the above code is executed at the SQL prompt, it creates the above package and displays the following result −

Package created.

Creating the Package Body

CREATE OR REPLACE PACKAGE BODY c_package AS

   PROCEDURE addCustomer(c_id  customers.id%type, 
   
      c_name customers.Name%type, 
      
      c_age  customers.age%type, 
      
      c_addr  customers.address%type,
      
      c_sal   customers.salary%type) 
      
   IS 
   
   BEGIN 
   
      INSERT INTO customers (id,name,age,address,salary) 
      
         VALUES(c_id, c_name, c_age, c_addr, c_sal); 
         
   END addCustomer; 
   
   
   PROCEDURE delCustomer(c_id   customers.id%type) IS 
   
   BEGIN 
   
      DELETE FROM customers 
      
      WHERE id = c_id; 
      
   END delCustomer;  
   
   
   PROCEDURE listCustomer IS 
   
   CURSOR c_customers is 
   
      SELECT  name FROM customers; 
      
   TYPE c_list is TABLE OF customers.Name%type; 
   
   name_list c_list := c_list(); 
   
   counter integer :=0; 
   
   BEGIN 
   
      FOR n IN c_customers LOOP 
      
      counter := counter +1; 
      
      name_list.extend; 
      
      name_list(counter) := n.name;
      
      dbms_output.put_line('Customer(' ||counter|| ')'||name_list(counter)); 
      
      END LOOP; 
      
   END listCustomer;
   
END c_package; 
/
The above example makes use of the nested table. We will discuss the concept of nested table in the next chapter.

When the above code is executed at the SQL prompt, it produces the following result −

Package body created.

Using The Package

The following program uses the methods declared and defined in the package c_package.

DECLARE 

   code customers.id%type:= 8; 
   
BEGIN 

   c_package.addcustomer(7, 'Rajnish', 25, 'Chennai', 3500); 
   
   c_package.addcustomer(8, 'Subham', 32, 'Delhi', 7500);
   
   c_package.listcustomer; 
   
   c_package.delcustomer(code); 
   
   c_package.listcustomer; 
   
END; 

/  
When the above code is executed at the SQL prompt, it produces the following result −

Customer(1): Ramesh  

Customer(2): Khilan  

Customer(3): kaushik   

Customer(4): Chaitali  

Customer(5): Hardik  

Customer(6): Komal 

Customer(7): Rajnish 

Customer(8): Subham 

Customer(1): Ramesh 

Customer(2): Khilan 

Customer(3): kaushik  

Customer(4): Chaitali  

Customer(5): Hardik  

Customer(6): Komal

Customer(7): Rajnish 


PL/SQL procedure successfully completed

 Trigger:-
 
Trigger is invoked by Oracle engine automatically whenever a specified event occurs.Trigger is stored into database and invoked repeatedly, when specific condition match.
Triggers are stored programs, which are automatically executed or fired when some event occurs.
Triggers are written to be executed in response to any of the following events.
o	A database manipulation (DML) statement (DELETE, INSERT, or UPDATE).
o	A database definition (DDL) statement (CREATE, ALTER, or DROP).
o	A database operation (SERVERERROR, LOGON, LOGOFF, STARTUP, or SHUTDOWN).
Triggers could be defined on the table, view, schema, or database with which the event is associated.

Advantages of Triggers:-

These are the following advantages of Triggers:

o	Trigger generates some derived column values automatically

o	Enforces referential integrity

o	Event logging and storing information on table access

o	Auditing

o	Synchronous replication of tables

o	Imposing security authorizations

o	Preventing invalid transactions

Creating a trigger:

Syntax for creating trigger:-

CREATE [OR REPLACE ] TRIGGER trigger_name

{BEFORE | AFTER | INSTEAD OF }

{INSERT [OR] | UPDATE [OR] | DELETE}

[OF col_name]

ON table_name

[REFERENCING OLD AS o NEW AS n]

[FOR EACH ROW]

WHEN (condition)

DECLARE

Declaration-statements

BEGIN

Executable-statements

EXCEPTION

Exception-handling-statements

END;

Here,
o	CREATE [OR REPLACE] TRIGGER trigger_name:

  It creates or replaces an existing trigger with the trigger_name.
  
o	{BEFORE | AFTER | INSTEAD OF} : This specifies when the trigger would be executed.
The INSTEAD OF clause is used for creating trigger on a view.
o	{INSERT [OR] | UPDATE [OR] | DELETE}: This specifies the DML operation.
o	[OF col_name]: This specifies the column name that would be updated.
o	[ON table_name]: This specifies the name of the table associated with the trigger.
o	[REFERENCING OLD AS o NEW AS n]: This allows you to refer new and old values for various DML statements, like INSERT, UPDATE, and DELETE.
o	[FOR EACH ROW]: This specifies a row level trigger, i.e., the trigger would be executed for each row being affected. Otherwise the trigger will execute just once when the SQL statement is executed, which is called a table level trigger.
o	WHEN (condition): This provides a condition for rows for which the trigger would fire. This clause is valid only for row level triggers.
PL/SQL Trigger Example:-
Let's take a simple example to demonstrate the trigger. In this example, we are using the following CUSTOMERS table:

Create table and have records:

ID	NAME	AGE	ADDRESS	SALARY
1	Ramesh	23	Allahabad	20000
2	Suresh	22	Kanpur	22000
3	Mahesh	24	Ghaziabad	24000
4	Chandan	25	Noida	26000
5	Alex	21	Paris	28000
6	Sunita	20	Delhi	30000

Create trigger:

Let's take a program to create a row level trigger for the CUSTOMERS table that would fire for INSERT or UPDATE or DELETE operations performed on the CUSTOMERS table. This trigger will display the salary difference between the old values and new values:

CREATE OR REPLACE TRIGGER display_salary_changes

BEFORE DELETE OR INSERT OR UPDATE ON customers
FOR EACH ROW

WHEN (NEW.ID > 0)
DECLARE

sal_diff number;

BEGIN

sal_diff := :NEW.salary  - :OLD.salary;
dbms_output.put_line('Old salary: ' || :OLD.salary);
dbms_output.put_line('New salary: ' || :NEW.salary);
dbms_output.put_line('Salary difference: ' || sal_diff);
END;
/
After the execution of the above code at SQL Prompt, it produces the following result.

Trigger created.

Check the salary difference by procedure:

Use the following code to get the old salary, new salary and salary difference after the trigger created.

DECLARE

total_rows number(2);

BEGIN

UPDATE  customers

SET salary = salary + 5000;

IF sql%notfound THEN

dbms_output.put_line('no customers updated');

ELSIF sql%found THEN

total_rows := sql%rowcount;

dbms_output.put_line( total_rows || ' customers updated ');

END IF;

END;
/
Output:

Old salary: 20000
New salary: 25000

Salary difference: 5000
Old salary: 22000
New salary: 27000

Salary difference: 5000
Old salary: 24000
New salary: 29000

Salary difference: 5000
Old salary: 26000
New salary: 31000

Salary difference: 5000
Old salary: 28000
New salary: 33000

Salary difference: 5000
Old salary: 30000
New salary: 35000

Salary difference: 5000

6 customers updated 

Note: As many times you executed this code, the old and new both salary is incremented by 5000 and hence the salary difference is always 5000.
After the execution of above code again, you will get the following result.
Old salary: 25000
New salary: 30000
Salary difference: 5000

Old salary: 27000
New salary: 32000
Salary difference: 5000

Old salary: 29000
New salary: 34000
Salary difference: 5000

Old salary: 31000
New salary: 36000
Salary difference: 5000

Old salary: 33000
New salary: 38000
Salary difference: 5000

Old salary: 35000
New salary: 40000
Salary difference: 5000

6 customers updated


