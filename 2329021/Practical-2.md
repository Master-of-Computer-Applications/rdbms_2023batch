NAME - Sukhpreet Singh
<br>CRN - 2329021
<br>PRACTICAL - 1
<br>QUESTION :- Data Definition Language(DDL), Data manipulation Language(DML) and Data Control Language(DCL)
# Data Definition Language(DDL)
<p>
Data Definition Language (DDL) is a subset of SQL. It is a language for describing data and its relationships in a database. You can generate DDL in a script for database objects to: Keep a snapshot of the database structure. Set up a test system where the database acts like the production system but contains no data.
</p>

### DDL Commands:

* Create
* Alter 
* truncate
* drop
* Rename 
<br>

<b><p>CREATE</p></b>
<p>This command is used to create a new table in SQL. The user has to give information like table name, column names, and their datatypes.</p>

<div style="border: 1px solid ; padding: 10px;">
<b>CREATE TABLE table_name</b>
<br><b>(</b>
<br><b>column_1 datatype,</b>
<br><b>column_2 datatype,</b>
<br><b>column_3 datatype,</b>
<br><b>....</b>
<br><b>);</b>
</div>

<b><p>ALTER</p></b>
<p>This command is used to add, delete or change columns in the existing table. The user needs to know the existing table name and can do add, delete or modify tasks easily.</p>
<b>ALTER TABLE table_name</b>
<br><b>ADD column_name datatype;</b>

# Data Manipulation Language(DML)
<p>
  DML is an abbreviation for Data Manipulation Language. Represents a collection of programming languages explicitly used to make changes to the database, such as: CRUD operations to create, read, update and delete data. Using INSERT, SELECT, UPDATE, and DELETE commands.
</p>

### DML Commands:

* INSERT
* SELECT
* UPDATE
* DELETE

# Data Control Language(DCL)
<p>
  Data Control Language (or DCL) consists of statements that control security and concurrent access to table data. Instructs the XDB Server to make permanent all data changes resulting from DML statements executed by a transaction. Connects the application process (or user) to a designated XDB Server or DB2 location.
</p>

### DCL Commands:

* GRANT
* REVOKE
* COMMIT
* ROLLBACK
