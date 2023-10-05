*What are DDL, DML, and DCL in SQL?*

Data Definition Language, shortly termed DDL, is a subset of SQL commands that define the structure or schema of the database.

Data Manipulation Language, shortly termed DML, is an element in SQL language that deals with managing and manipulating data in the database.

Data Control Language, shortly termed DCL, is comprised of those commands in SQL that deal with controls, rights, and permission in the database system.

*What are DDL, DML, and DCL Commands?*

DDL Commands
DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:

The CREATE command creates database objects, tables, and triggers.
ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.
The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.
The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.
The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.

DML Commands
DML commands are SQL commands that perform operations like storing data in database tables, modifying and deleting existing rows, retrieving data, or updating data.

The SELECT command fetches data or records from one or more tables in the SQL database. The retrieved data gets displayed in a result table known as the result set.
The INSERT command inserts one or more new records into the table in the SQL database.
The UPDATE command updates or changes the existing data or records in a table in the SQL database.
The DELETE command deletes all the existing records and the allocated spaces from a table in the SQL database. We can use the WHERE clause with the AND or OR operators to delete selected rows from the database.
The MERGE command deals with insertion, updation, and deletion in the same SQL statement.
The CALL command calls or invokes a stored procedure.
The EXPLAIN PLAN command describes the access path to the data. It returns the execution plans for the statements like INSERT, UPDATE, and DELETE in the readable format for users to check the SQL Queries.
The LOCK TABLE command ensures the consistency, atomicity, and durability of database transactions like reading and writing operations.

*DML Example*
Let's take the example of INSERT, which is a DML command. The INSERT command inserts data into the table in the SQL database.

Let us consider a Student table in the SQL database having fields names as s_id, name, and age.

Student Table:

s_id	name	age
101	Esha	20
102	Suman	21
103	Durgesh	20
104	Amish	22

INSERT INTO Student VALUES(105, 'Nisha', 30);

Updated Student Table:

s_id	name	age
101	Esha	20
102	Suman	21
103	Durgesh	20
104	Amish	22
105	Nisha	30

Product Table:

Product_Id	Product_Name	Product_Price	Product_Quantity
P101	Chips	20	20
P102	Chocolates	60	40
P103	Maggi	75	5
P201	Biscuits	83	20
P203	Namkeen	40	50

UPDATE Product 
SET Product_Price = 80 
WHERE Product_Id = 'P201';  

Student Table:

Stu_Id	Stu_Name	Stu_Marks	Stu_Age
101	Ramesh	92	20
201	Jatin	83	19
202	Anuj	85	19
203	Monty	95	21
102	Saket	65	21
103	Sumit	78	19
104	Ashish	98	20

UPDATE Student 
SET Stu_Marks = 80, Stu_Age = 21 
WHERE Stu_Id = 103 AND Stu_Id = 202;

The updated table after executing the above SQL Query is:

Stu_Id	Stu_Name	Stu_Marks	Stu_Age
101	Ramesh	92	20
201	Jatin	83	19
202	Anuj	80	21
203	Monty	95	21
102	Saket	65	21
103	Sumit	80	21
104	Ashish	98	20