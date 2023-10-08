[Experiment-2(AJAYPAL).md](https://github.com/AjaypalSinghMahal/rdbms_2023batch/files/12840088/Experiment-2.AJAYPAL.md)
Data Definition Language(DDL),Data Manipulation Language(DML) and Data Control Language(DCL):

Structured Query Language(SQL) as we all know is the database language by the use of which we can perform certain operations on the existing database and also we can use this language to create a database. SQL uses certain commands like CREATE, DROP, INSERT, etc. to carry out the required tasks. 
SQL commands are like instructions to a table. It is used to interact with the database with some operations. It is also used to perform specific tasks, functions, and queries of data. SQL can perform various tasks like creating a table, adding data to tables, dropping the table, modifying the table, set permission for users.

DDL (Data Definition Language)

DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.

List of DDL commands: 

CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
COMMENT: This is used to add comments to the data dictionary.
RENAME: This is used to rename an object existing in the database.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/5e9f972f-4191-4554-8f38-319ff54ab108)

DML(Data Manipulation Language)

The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.

List of DML commands: 

INSERT: It is used to insert data into a table.
UPDATE: It is used to update existing data within a table.
DELETE: It is used to delete records from a database table.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/ebb7d5a1-e720-4e16-a9f4-be324a4e0eb4)

DCL (Data Control Language)

DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system. 

List of  DCL commands: 

GRANT: This command gives users access privileges to the database.

Syntax:

GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;  
REVOKE: This command withdraws the user’s access privileges given by using the GRANT command.
Syntax:
REVOKE SELECT, UPDATE ON MY_TABLE FROM USER1, USER2.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/f8f988d6-f5f6-4d72-8e0d-bba06064c45d)

