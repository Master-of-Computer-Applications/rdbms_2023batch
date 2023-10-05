# <p align="center">RDBMS ASSIGNMENT</p>
## Defination of Commands  
### SQL stands for Structured Query Language. SQL commands are the instructions used to communicate with a database to perform tasks, functions, and queries with data. <br> 
### SQL commands can be used to search the database and to do other functions like creating tables, adding data to tables, modifying data, and dropping tables. <br>
|Data Definition Language (DDL)|Data Manipulation Language|Data Control Language|
| :---  | :--- |:---|
|DDL changes the structure of the table like creating a table, deleting a table, altering a table, etc.| DML commands are used to modify the database. It is responsible for all form of changes in the database.|DCL commands are used to grant and take back authority from any database user.|
|All the command of DDL are auto-committed that means it permanently save all the changes in the database.|The command of DML is not auto-committed that means it can't permanently save all the changes in the database. They can be rollback.|DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system. |
|Syntax: CREATE TABLE TABLE_NAME (COLUMN_NAME DATATYPES[,....]); |Syntax: INSERT INTO TABLE_NAME VALUES (value1, value2, value3, .... valueN); | syntax: GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER; |
|commands: create, alter, drop and trucate| commands: insert, update , delete| commands: grant and revoke|
|CREATE It is used to create a new table in the database.|INSERT: The INSERT statement is a SQL query. It is used to insert data into the row of a table.|Grant: It is used to give user access privileges to a database.|

