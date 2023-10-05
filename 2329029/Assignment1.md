1-Difference between DDL, DML and DCL.

*<b>DDL Commands</b>*

1: DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL: The CREATE command creates database objects, tables, and triggers.

2: ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.

3: The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.

4: The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.

5: The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.



*<b>DML Commands</b>*

DML commands are SQL commands that perform operations like storing data in database tables, modifying and deleting existing rows, retrieving data, or updating data.

1: The SELECT command fetches data or records from one or more tables in the SQL database. The retrieved data gets displayed in a result table known as the result set.

2: The INSERT command inserts one or more new records into the table in the SQL database.

3: The UPDATE command updates or changes the existing data or records in a table in the SQL database.

4: The DELETE command deletes all the existing records and the allocated spaces from a table in the SQL database. We can use the WHERE clause with the AND or OR operators to delete selected rows from the database.

5: The MERGE command deals with insertion, updation, and deletion in the same SQL statement.

6: The CALL command calls or invokes a stored procedure.

7: The EXPLAIN PLAN command describes the access path to the data. It returns the execution plans for the statements like INSERT, UPDATE, and DELETE in the readable format for users to check the SQL Queries.

8: The LOCK TABLE command ensures the consistency, atomicity, and durability of database transactions like reading and writing operations.

*<b>DCL</b>*

DCL commands are SQL commands that perform operations like giving and withdrawing database access from the user.

1- The GRANT command gives access privileges or permissions like ALL, SELECT, and EXECUTE to the database objects like views, tables, etc, in SQL.

2- The REVOKE command withdraws access privileges or permissions given with the GRANT command.

