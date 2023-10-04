Ravneet Singh
#H1Data Definition Language,
Data Definition Language shortly termed DDL, is a subset of SQL commands that define the structure or schema of the database. 
DDL Commands
DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:

The CREATE command creates database objects, tables, and triggers.
ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.
The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.
The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.
The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.

Data Manipulation Language, shortly termed DML, is an element in SQL language that deals with managing and manipulating data in the database.
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

Data Control Language, shortly termed DCL, is comprised of those commands in SQL that deal with controls, rights, and permission in the database system.DCL Commands

DCL commands are SQL commands that perform operations like giving and withdrawing database access from the user.
The GRANT command gives access privileges or permissions like ALL, SELECT, and EXECUTE to the database objects like views, tables, etc, in SQL.
The REVOKE command withdraws access privileges or permissions given with the GRANT command.
