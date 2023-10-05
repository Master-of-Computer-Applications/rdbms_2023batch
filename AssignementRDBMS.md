###<p align = "Center">Difference between Dcl Dml Ddl? </p>

DCL
Data Control Language (or DCL) consists of statements that control security and concurrent access to table data.

COMMIT
Instructs the XDB Server to make permanent all data changes resulting from DML statements executed by a transaction.

CONNECT
Connects the application process (or user) to a designated XDB Server or DB2 location. This location becomes the current location for the application process or user.

GRANT (Database Privileges)
Assigns access privileges to XDB Server users or applications.

LOCK TABLE
Extends XDB Server's automatic record and table level locking functions (in a multi-user system) by acquiring explicit locks on a particular table.

REVOKE (Database Privileges)
Cancels access privileges for XDB Server users or applications.

REVOKE (Sequence Privileges)
Revokes the privileges on a user-defined sequence.

Dml
DML stands for Data Manipulation Language. Tables and formulas are helpful when communicating with data stored up to a point in a database through SQL (Structured Query Language), but a time comes when we actually want to execute some fairly complicated data interactions. We will also need the Data Manipulation Language in that situation. DML is a way to inform a database precisely what we want it to do by conversing in a manner that it has been built to comprehend from scratch. When it comes to interacting with existing data, whether adding, moving, or deleting data, it provides a convenient way to do so.

Characteristics of DML
It performs interpret-only data queries. It is used in a database schema to recall and manipulate the information. DML It is a dialect which is used to select, insert, delete and update data in a database. Data Manipulation Language (DML) commands are as follows:

SELECT Command
This command is used to get data out of the database. It helps users of the database to access from an operating system, the significant data they need. It sends a track result set from one tables or more.

Syntax :

SELECT * 
FROM <table_name>; 
Example:

SELECT * 
FROM students;

OR

SELECT * 
FROM students
where due_fees <=20000;

INSERT Command
This command is used to enter the information or values into a row. We can connect one or more records to a single table within a repository using this instruction. This is often used to connect an unused tag to the documents.

Syntax:

INSERT INTO <table_name> ('column_name1' <datatype>, 'column_name2' <datatype>)
VALUES ('value1', 'value2'); 
Example :

INSERT INTO students ('stu_id' int, 'stu_name' varchar(20), 'city' varchar(20))
VALUES ('1', 'Nirmit', 'Gorakhpur'); 
UPDATE Command
This command is used to alter existing table records. Within a table, it modifies data from one or more records. This command is used to alter the data which is already present in a table.

Syntax:

UPDATE <table_name>
SET <column_name = value>
WHERE condition; 
Example:

UPDATE students
SET due_fees = 20000
WHERE stu_name = 'Mini'; 

DELETE Command
It deletes all archives from a table. This command is used to erase some or all of the previous table’s records. If we do not specify the ‘WHERE’ condition then all the rows would be erased or deleted.

Syntax:

DELETE FROM <table_name>
WHERE <condition>; 
Example:

DELETE FROM students
WHERE stu_id = '001'; 

Ddl
Data Definition Language(DDL) is a subset of SQL and a part of DBMS(Database Management System). DDL consist of Commands to commands like CREATE, ALTER, TRUNCATE and DROP. These commands are used to create or modify the tables in SQL.

DDL Commands :
In this section, We will cover the following DDL commands as follows.

Create
Alter 
truncate
drop
Rename 

Command-1 :
CREATE :
This command is used to create a new table in SQL. The user has to give information like table name, column names, and their datatypes.

Syntax –

CREATE TABLE table_name
(
column_1 datatype,
column_2 datatype,
column_3 datatype,
....
);

Example –
We need to create a table for storing Student information of a particular College. Create syntax would be as below.

CREATE TABLE Student_info
(
College_Id number(2),
College_name varchar(30),
Branch varchar(10)
);
Command-2 :
ALTER :
This command is used to add, delete or change columns in the existing table. The user needs to know the existing table name and can do add, delete or modify tasks easily.

Syntax –
Syntax to add a column to an existing table.

ALTER TABLE table_name
ADD column_name datatype;

Example –
In our Student_info table, we want to add a new column for CGPA. The syntax would be as below as follows.

ALTER TABLE Student_info
ADD CGPA number;
Command-3 :
TRUNCATE :
This command is used to remove all rows from the table, but the structure of the table still exists.

Syntax –
Syntax to remove an existing table.

TRUNCATE TABLE table_name;
Example –
The College Authority wants to remove the details of all students for new batches but wants to keep the table structure. The command they can use is as follows.

TRUNCATE TABLE Student_info;
Command -5

RENAME:

It is possible to change name of table with or without data in it using simple RENAME command.

We can rename any table object at any point of time.

Syntax –

RENAME TABLE <Table Name> To <New_Table_Name>;
Example:

If you want to change the name of the table from Employee to Emp we can use rename command as 


