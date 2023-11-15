                                         Experiment:-6
                         How to apply Conditional Controls in PL/SQL:
PL/SQL is a block structured language that enables developers to combine the power of SQL with procedural statements. 
All the statements of a block are passed to oracle engine all at once which increases processing speed and decreases the traffic. 
Basics of PL/SQL:-
•	•PL/SQL stands for Procedural Language extensions to the Structured Query Language (SQL).
•	 PL/SQL is a combination of SQL along with the procedural features of programming languages.
•	Oracle uses a PL/SQL engine to processes the PL/SQL statements.
•	PL/SQL includes procedural language elements like conditions and loops. It allows declaration of constants and variables, procedures and functions, types and variable of those types and triggers.
Disadvantages of SQL:
•	SQL doesn’t provide the programmers with a technique of condition checking, looping and branching.
•	SQL statements are passed to Oracle engine one at a time which increases traffic and decreases speed.
•	SQL has no facility of error checking during manipulation of data.

Features of PL/SQL:
1.	PL/SQL is basically a procedural language, which provides the functionality of decision making, iteration and many more features of procedural programming languages.
2.	PL/SQL can execute a number of queries in one block using single command.
3.	One can create a PL/SQL unit such as procedures, functions, packages, triggers, and types, which are stored in the database for reuse by applications.
4.	PL/SQL provides a feature to handle the exception which occurs in PL/SQL block known as exception handling block.
5.	Applications written in PL/SQL are portable to computer hardware or operating system where Oracle is operational.
6.	PL/SQL Offers extensive error checking.

Structure of PL/SQL Block:
PL/SQL extends SQL by adding constructs found in procedural languages, resulting in a structural language that is more powerful than SQL. The basic unit in PL/SQL is a block. All PL/SQL programs are made up of blocks, which can be nested within each other. 
 Typically, each block performs a logical action in the program. A block has the following structure:
DECLARE
    declaration statements;

BEGIN
    executable statements

EXCEPTIONS
    exception handling statements

END;

There come situations in real life when we need to make some decisions and based on these decisions, we decide what should we do next. Similar situations arise in programming also where we need to make some decisions and based on these decisions we will execute the next block of code. Decision-making statements in programming languages decide the direction of flow of program execution. Decision-making statements available in pl/SQL are:
1.	if then statement
2.	if then else statements
3.	nested if-then statements
4.	if-then-elseif-then-else ladder
•	if then statement if then statement is the most simple decision-making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statement is executed otherwise not.
 Syntax:
if condition then
-- do something
end if;
Here, condition after evaluation will be either true or false.
if statement accepts boolean values – if the value is true then it will execute the block of statements below it otherwise not.
if and endif consider as a block here.
Example:-
set serveroutput on;
DECLARE
	x int:=10;
	y int:=80;
BEGIN
	if(y>x) then
		dbms_output.put_line('Result: ' ||y|| ' is greater than ' ||x);
	end if;
END;
OUTPUT:-

Result: 80 is greater than 10
PL/SQL procedure successfully completed.

•	if – then- else: The if statement alone tells us that if a condition is true it will execute a block of statements and if the condition is false it won’t. But what if we want to do something else if the condition is false. Here comes the else statement. We can use the else statement with if statement to execute a block of code when the condition is false.
 Syntax:-
if (condition) then
    -- Executes this block if
    -- condition is true
else 
    -- Executes this block if
    -- condition is false
set serveroutput on;

DECLARE

	x int;
 
BEGIN

	x := &x;
 
	if mod(x,2) = 0 then
 
		dbms_output.put_line('Even Number');
  
	else
 
		dbms_output.put_line('Odd Number');
  
	end if;
 
END;

OUTPUT:-

Enter value for x:6

Even Number

PL/SQL procedure successfully completed.

•	if...then...elsif...else statement:-

It is used to check multiple conditions. Sometimes it is required to test more than one condition in that case if...then...else statement cannot be used. For this purpose, if...then...elsif...else statement is suitable in which all the conditions are tested one by one and whichever condition is found to be TRUE, that block of code is executed. And if all the conditions result in FALSE then the else part is executed.

SYNTAX:-

if <test_condition1> then

	body of action
 
elsif <test_condition2>then

	body of action
 
elsif<test_condition3>then

	body of action
 
...
...
...
else

	body of action
 
end if;

set serveroutput on;

DECLARE

	a int;
 
	b int;
 
BEGIN
	a := &
 
 b := &b;
 
if(a>b) then

		dbms_output.put_line(‘a is greater than b’);
  
	elsif(b>a) then
 
		dbms_output.put_line(‘b is greater than a’);
  
	else
 
 
		dbms_output.put_line(‘Both a and b are equal’);
  
 end if;
 
END;

OUTPUT:-

Enter value for a: 8

Enter value for b: 5

a is greater than b

PL/SQL procedure successfully completed.
•	nested-if-then: A nested if-then is an if statement that is the target of another if statement. 
Nested if-then statements mean an if statement inside another if statement. Yes, PL/SQL allows us to nest if statements within if-then statements. i.e, we can place an if then statement inside another if then statement. 
Syntax:-

if (condition1) then

   -- Executes when condition1 is true
   
   if (condition2) then 
   
     -- Executes when condition2 is true
     
   end if;
   
end if;

Example:-

declare

num1 number:= 10;

num2 number:= 20;

num3 number:= 20;
 
begin

if num1 < num2 then

dbms_output.put_line('num1 small num2');
 
  if num1 < num3 then 
  
  dbms_output.put_line('num1 small num3 also');  end if;
 
end if;
 
dbms_output.put_line('after end if');

end;

Output:-

num1 small num2

num1 small num3 also after end if


•	if-then-elsif-then-else ladder:- Here, a user can decide among multiple options.
The if then statements are executed from the top down. 
As soon as one of the conditions controlling the if is true, the statement associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final else statement will be executed.
 Syntax:-
 
if (condition) then

    --statement
    
elsif (condition) then

    --statement
.
.
else

    --statement
    
Endif

Example:-

declare

num1 number:= 10;

num2 number:= 20;
 
begin
 
if num1 < num2 then

dbms_output.put_line('num1 small');
 
ELSEIF num1 = num2 then

dbms_output.put_line('both equal');
 
ELSE

dbms_output.put_line('num2 greater');end if;
 
dbms_output.put_line('after end if');

end;


Output:-
num1 small

after end if

