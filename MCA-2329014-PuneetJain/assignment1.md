# <p align="center">Assignment of RDMBS</p>
# <p align="left">1-Differentiate Between DDL, DML,and DCL.</p>


## **DDL Commands**:

DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:

1-The CREATE command creates database objects, tables, and triggers.</br>
2-ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.</br>
3-The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.</br>
4-The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.</br>
5-The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.</br>

## **DML Commands**:

DML commands are SQL commands that perform operations like storing data in database tables, modifying and deleting existing rows, retrieving data, or updating data.

  1-The SELECT command fetches data or records from one or more tables in the SQL database. The retrieved data gets displayed in a result table known as the result set.</br>
  2-The INSERT command inserts one or more new records into the table in the SQL database.</br>
  3-The UPDATE command updates or changes the existing data or records in a table in the SQL database.</br>
  4-The DELETE command deletes all the existing records and the allocated spaces from a table in the SQL database. We can use the WHERE clause with the AND or OR operators to delete selected rows from the database.</br>
  5-The MERGE command deals with insertion, updation, and deletion in the same SQL statement.</br>
  6-The CALL command calls or invokes a stored procedure.</br>
  7-The EXPLAIN PLAN command describes the access path to the data. It returns the execution plans for the statements like INSERT, UPDATE, and DELETE in the readable format for users to check the SQL Queries.</br>
  8-The LOCK TABLE command ensures the consistency, atomicity, and durability of database transactions like reading and writing operations.</br>

## **DCL Commands**:

DCL commands are SQL commands that perform operations like giving and withdrawing database access from the user.

  1-The GRANT command gives access privileges or permissions like ALL, SELECT, and EXECUTE to the database objects like views, tables, etc, in SQL.</br>
  2-The REVOKE command withdraws access privileges or permissions given with the GRANT command.

## ***Differences Between DDL, DML,and DCL:***
DDL | DML | DCL
|---|---|---|
DDL stands for Data Definition Language.|DML stands for Data Manipulation Language.|DCL stands for Data Control Language.
It helps us to define the structure of the database.|It helps us to manage the data.|t helps us to control the access and permission of the database.
It affects the entire table data.|It only affects the specified row(s) of the table.|It applies to the complete table.
Changes are permanent.|We can roll back our changes in the DML language.|We can roll back the changes in the DCL language.
It helps in defining the fields or columns of the tables.|It helps us to define rows or records of the tables.|It helps us to control access to the information in the database.
They are auto-committed (changes made are permanent).|They are not auto-committed (changes are not permanent).|They are not auto-committed (changes are not permanent). 
They don't have further classification.|They are of two types procedural and non-procedural.|They don't have any further classification.
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.
