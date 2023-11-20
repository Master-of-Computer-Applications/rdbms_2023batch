
# <p align="center">ASSIGNMENT OF RDMBS</p>
## DDL (Data Definition Language):
 DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
 
### **List of DDL commands:**
 
 **CREATE:** This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).

**DROP:** This command is used to delete objects from the database.

**ALTER:** This is used to alter the structure of the database.

**TRUNCATE:** This is used to remove all records from a table, including all spaces allocated for the records are removed.

**COMMENT:** This is used to add comments to the data dictionary.

**RENAME:** This is used to rename an object existing in the database.


## DML(Data Manipulation Language):
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.

### **List of DML commands:**

**INSERT:** It is used to insert data into a table.

**UPDATE:** It is used to update existing data within a table.

**DELETE:** It is used to delete records from a database table.


## DCL (Data Control Language):
DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system.

### **List of DCL commands:**

**GRANT:** This command gives users access privileges to the database.

**REVOKE:** This command withdraws the user’s access privileges given by using the GRANT command.


# <p align="left"> Differences Between DDL, DML,and DCL.</p>

DDL | DML | DCL
|---|---|---|
DDL stands for Data Definition Language.|DML stands for Data Manipulation Language.|DCL stands for Data Control Language.
It helps us to define the structure of the database.|It helps us to manage the data.|t helps us to control the access and permission of the database.
It affects the entire table data.|It only affects the specified row(s) of the table.|It applies to the complete table.
Changes are permanent.|We can roll back our changes in the DML language.|We can roll back the changes in the DCL language.
It helps in defining the fields or columns of the tables.|It helps us to define rows or records of the tables.|It helps us to control access to the information in the database.
They are auto-committed (changes made are permanent).|They are not auto-committed (changes are not permanent).|They are not auto-committed (changes are not permanent). 
They don't have further classification.|They are of two types procedural and non-procedural.|They don't have any further classification.
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.| Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.
