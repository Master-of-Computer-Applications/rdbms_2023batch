                                              Experiment:-9
                              How to run stored procedures and functions:
Stored procedure and Function, both can be defined as a set of logically written statements, stored in the database and are executed when called, to perform a specific task.
Both function as well as stored procedure have a unique named block of code which is compiled and stored in the database.
Any stored procedure or function created, remains useless unless it is called. Therefore, after creating a stored procedure or function it is necessary to make a call for that stored procedure or function from another PL/SQL block in order to serve the purpose for which it has been created.

Creating a Stored Procedure or Function:-
Whenever a block of code for stored procedure or function is written it is then, they are automatically compiled by the oracle engine. During compilation if any error occurs, we get a message on the screen saying that the procedure or function is created with compilation errors but actual error is not displayed.
In order to find out the compilation errors following statement can be executed:

SELECT * from USER_ERRORS;


Once it is compiled, it is then stored by the oracle engine in the database as a database object.

Stored Procedure or function's block of code in PL/SQL is made up of the following three sections:

•	Declarative section: In this section, variables, constants, cursor or exceptions that are going to be used by procedure or function are declared.
•	Executable section: In this section, the definition of procedure or function created is written. This section also contains the SQL or PL/SQL statements assigning values, controlling execution and manipulating data.
•	Exception Handling section: In this section, the expected exceptions are written which may arise during execution of code written in executable part. This section is optional.

Syntax for creating Stored Procedure:-
Below we have the basic syntax for creating a stored procedure in oracle:

CREATE OR REPLACE PROCEDURE <procedure_name> 

(<variable_name>IN/OUT/IN OUT <datatype>,

   <variable_name>IN/OUT/IN OUT <datatype>,...) IS/AS
   
variable/constant declaration;

BEGIN

	-- PL/SQL subprogram body;
 
EXCEPTION

	-- Exception Handling block ;
 
END <procedure_name>;

Let's understand the above code,

•	procedure_name is for procedure's name and variable_name is the variable name for variable used in the stored procedure.
•	CREATE or REPLACE PROCEDURE is a keyword used for specifying the name of the procedure to be created.
•	BEGIN, EXCEPTION and END are keywords used to indicate different sections of the procedure being created.

•	IN/OUT/IN OUT are parameter modes.

•	IN mode refers to READ ONLY mode which is used for a variable by which it will accept the value from the user. It is the default parameter mode.
•	OUT mode refers to WRITE ONLY mode which is used for a variable that will return the value to the user.
•	IN OUT mode refers to READ AND WRITE mode which is used for a variable that will either accept a value from the user or it will return the value to the user.
•	At the end, <procedure_name> is optional to write, you can simply use END statement to end the procedure definition.
•	In the code example below we have create a simple program to demonstrate the use of stored procedure for adding two numbers:

set serveroutput on;

CREATE OR REPACE PROCEDURE Sum(a IN number, b IN number) IS

c number; 

BEGIN

	c := a+b;
 
	dbms_output.put_line('Sum of two nos= '|| c);
 
END Sum;


OUTPUT:-    

Procedure created.

For calling the procedure created following code will be executed:

set serveroutput on;

DECLARE

	x number;
 
	y number;
 
BEGIN

	x := &x;
 
	y := &y;
 
	Sum(x,y);
 
END;

OUTPUT:-

Enter value for x: 10

Enter value for y: 20

Sum of two nos= 30

PL/SQL procedure successfully created.

Syntax for creating Functions in PL/SQL:-

Now that we know how to create stored procedures and how to use them in another PL/SQL code block, it's time to understand how to create Functions in PL/SQL.

CREATE OR REPLACE FUNCTION <function_name>

(<variable_name> IN <datatype>,

<variable_name> IN <datatype>,...)

RETURN <datatype> IS/AS

variable/constant declaration;

BEGIN

	-- PL/SQL subprogram body;
 
EXCEPTION

	-- Exception Handling block ;
 
END <function_name>;



Let's understand the above code,
•	function_name is for defining function's name and variable_name is the variable name for variable used in the function.
•	CREATE or REPLACE FUNCTION is a keyword used for specifying the name of the function to be created.
•	IN mode refers to READ ONLY mode which is used for a variable by which it will accept the value from the user. It is the default parameter mode.
•	RETURN is a keyword followed by a datatype specifying the datatype of a value that the function will return.

Most part of the above code is similar to the one used for defining a stored procedure.

In the code below we have a program to demonstrate the use of function for adding two numbers.

set serveroutput on;

CREATE OR REPLACE FUNCTION Sum(a IN number, b IN number) RETURN Number IS

c number;

BEGIN

	c := a+b;
 
	RETURN c;
 
END;


 OUTPUT:-
 
Function Created

For calling the function Sum following code will be executed:
set serveroutput on;


DECLARE

	no1 number;
 
	no2 number;
 
	result number;
 
BEGIN

	no1 := &no1;
 
	no2 := &no2;
 
	result := Sum(no1,no2);

dbms_output.put_line(‘Sum of two nos=’||result);

END;

OUTPUT:-

Enter value for no1:5

Enter value for no2:5

Sum of two nos=10

PL/SQL procedure successfully created. 

With this, now we know how to define and use a stored procedure in PL/SQL and how to define a function and use the function in PL/SQL.
