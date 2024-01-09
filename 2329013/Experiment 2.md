                          Experiment-2:
Data Definition Language(DDL),Data Manipulation Language(DML) and Data Control Language(DCL):

Structured Query Language(SQL) as we all know is the database language by the use of which we can perform
certain operations on the existing database and also we can use this language to create a database. SQL uses certain
commands like CREATE, DROP, INSERT, etc. to carry out the required tasks.

SQL commands are like instructions to a table. It is used to interact with the database with some operations. It is also
used to perform specific tasks, functions, and queries of data. SQL can perform various tasks like creating a table,
adding data to tables, dropping the table, modifying the table, set permission for users.

DDL (Data Definition Language):-
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database
schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of
database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database
structures but not data. These commands are normally not used by a general user, who should be accessing the
database via an application.

List of DDL commands:

CREATE: This command is used to create the database or its objects (like table, index, function, views, store
procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are
removed.
COMMENT: This is used to add comments to the data dictionary.
RENAME: This is used to rename an object existing in the database
![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/290412fb-e834-4506-93b7-7a9bf913dfdf)


DML(Data Manipulation Language):-

The SQL commands that deal with the manipulation of data present in the database belong to DML or Data
Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that
controls access to data and to the database. Basically, DCL statements are grouped with DML statements.

List of DML commands:

INSERT: It is used to insert data into a table.

UPDATE: It is used to update existing data within a table.

DELETE: It is used to delete records from a database table.

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/cf8a9055-7734-4358-af9a-c03cb18bb24a)


![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/af5dfda4-6a77-4e8b-9c90-99d4c5698321)


DCL (Data Control Language):-
DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other
controls of the database system.

List of DCL commands:

GRANT: This command gives users access privileges to the database.
Syntax:
GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/6833f60b-43e5-45ed-9136-8482e65b2c2b)

REVOKE: This command withdraws the user’s access privileges given by using the GRANT command.
Syntax:
REVOKE SELECT, UPDATE ON MY_TABLE FROM USER1, USER2.

















