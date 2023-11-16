# <p align="center">Assignment of RDMBS</p>
# <p align="left">1-Differences Between DDL, DML,and DCL.</p>

DDL | DML | DCL
|---|---|---|
DDL stands for Data Definition Language.|DML stands for Data Manipulation Language.|DCL stands for Data Control Language.
It helps us to define the structure of the database.|It helps us to manage the data.|t helps us to control the access and permission of the database.
It affects the entire table data.|It only affects the specified row(s) of the table.|It applies to the complete table.
Changes are permanent.|We can roll back our changes in the DML language.|We can roll back the changes in the DCL language.
It helps in defining the fields or columns of the tables.|It helps us to define rows or records of the tables.|It helps us to control access to the information in the database.
They are auto-committed (changes made are permanent).|They are not auto-committed (changes are not permanent).|They are not auto-committed (changes are not permanent). 
They don't have further classification.|They are of two types procedural and non-procedural.|They don't have any further classification.
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.

# Data Definition Language
</br>Data Definition Language shortly termed DDL, is a subset of SQL commands that define the structure or schema of the database. 
## </br>DDL Commands
</br>DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:
</br>•	The CREATE command creates database objects, tables, and triggers.
</br>•	ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.
</br>•	The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.
</br>•	The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.
</br>•	The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.
### EXAMPLE: 
CREATE database students;
</br>DROP database students;
# </br>Data Manipulation Language
</br>Data Manipulation Language, shortly termed DML, is an element in SQL language that deals with managing and manipulating data in the database.
## </br>DML Commands
</br>DML commands are SQL commands that perform operations like storing data in database tables, modifying and deleting existing rows, retrieving data, or updating data.
</br>•	The SELECT command fetches data or records from one or more tables in the SQL database. The retrieved data gets displayed in a result table known as the result set.
</br>•	The INSERT command inserts one or more new records into the table in the SQL database.
</br>•	The UPDATE command updates or changes the existing data or records in a table in the SQL database.
</br>•	The DELETE command deletes all the existing records and the allocated spaces from a table in the SQL database. We can use the WHERE clause with the AND or OR operators to delete selected rows from the database.
</br>•	The MERGE command deals with insertion, updation, and deletion in the same SQL statement.
</br>•	The CALL command calls or invokes a stored procedure.
</br>•	The EXPLAIN PLAN command describes the access path to the data. It returns the execution plans for the statements like INSERT, UPDATE, and DELETE in the readable format for users to check the SQL Queries.
</br>•	The LOCK TABLE command ensures the consistency, atomicity, and durability of database transactions like reading and writing operations.
### EXAMPLE:
INSERT INTO students VALUES(1,"RAM");
# </br>Data Control Language
</br>Data Control Language, shortly termed DCL, is comprised of those commands in SQL that deal with controls, rights, and permission in the database system.
## </br>DCL Commands 
</br>•	DCL commands are SQL commands that perform operations like giving and withdrawing database access from the user.
</br>•	The GRANT command gives access privileges or permissions like ALL, SELECT, and EXECUTE to the database objects like views, tables, etc, in SQL.
</br>•	The REVOKE command withdraws access privileges or permissions given with the GRANT command.
### EXAMPLE:
GRANT SELECT, UPDATE ON students TO RAM;
# <p align="center">PRACTICAL FILE OF RDMBS</p>
## <p align="left"> Ques-1. Comparative study of various Database Management Systems</p>
A Database Management System (DBMS) is a software application or system that facilitates the creation, organization, storage, retrieval, and management of data in a structured and efficient manner. It serves as an intermediary between users or applications and the underlying database, providing tools and functionalities for data storage, access, security, and data integrity. DBMS systems are essential for effectively managing and manipulating data in various domains, including business, research, and software development.

There are numerous Database Management Systems (DBMS) available, each with its own features and strengths. Here are some of the well-known DBMS:

### Relational Database Management Systems (RDBMS):
    1.MySQL
    2.PostgreSQL
    3.Oracle Database
    4.Microsoft SQL Server
    5.SQLite
    6.Maria DB
    7.IBM Db2

### MySQL:
MySQL is an open-source relational database management system (RDBMS) used in a wide range of applications, especially web-related ones. It offers structured data storage, strong performance, and a large and active community of users and developers. It is known for its reliability and cost-effectiveness.
  - An open-source relational database management system.
  - Widely used for web applications, content management systems, and more.
  - Known for good performance and reliability for smaller to medium-sized applications.
  - Supports replication and clustering for scalability.
  - Adheres to ACID properties for data integrity.
  - Has a large and active community.

### SQLite:
SQLite is a lightweight, file-based, embedded database system often used for local data storage and mobile applications. It's known for its speed and simplicity, making it suitable for smaller-scale projects where high concurrency and large-scale data handling are not essential.
  - A serverless, self-contained database engine.
  - Primarily used for local data storage, embedded systems, and mobile applications.
  - Lightweight and fast but not suitable for heavy concurrent loads.
  - Not designed for high-concurrency or large-scale applications.
  - ACID-compliant for data integrity.
  - Features a minimal set of features, keeping it simple and lightweight.

### Oracle:
Oracle is a prominent and commercial relational database management system (RDBMS) often used in enterprise-level applications, known for its high performance, scalability, and advanced features, albeit with associated costs. It is widely used in organizations for managing and storing critical data.
  - A commercial database system with various licensing options.
  - Typically used in enterprise-level applications requiring high availability and scalability.
  - Offers high performance and advanced optimization features.
  - Supports clustering, partitioning, and high availability configurations.
  - Strictly adheres to ACID compliance.
  - Provides an extensive feature set, including advanced security and data warehousing.
  - Offers robust support services but can be costly.

### PostgreSQL:
PostgreSQL, often known as Postgres, is a powerful open-source relational database management system (RDBMS) known for its versatility, strong performance, and advanced features. It's widely used in various applications, and it strictly adheres to data integrity standards while offering an active open-source community.
  - An open-source relational database management system.
  - Suitable for various applications, especially those requiring advanced data features and extensibility.
  - Known for strong performance, especially for complex queries and large datasets.
  - Supports horizontal scaling and partitioning for large-scale applications.
  - Strictly adheres to ACID compliance.
  - Offers extensive features, including support for JSON data and full-text search.
  - Boasts an active open-source community and a rich ecosystem.

### MariaDB:
MariaDB is an open-source relational database management system that is compatible with MySQL. It provides strong performance, scalability options, and data integrity, making it a popular choice for web applications and software projects as a MySQL alternative. MariaDB benefits from an active community and offers features similar to MySQL while introducing some unique enhancements.
  - An open-source relational database management system, often used as a drop-in replacement for MySQL.
  - Suitable for web applications and offers performance similar to MySQL.
  - Has an active community and benefits from compatibility with MySQL for easier migration.
  - Supports clustering and replication for scaling.
  - Adheres to ACID properties.
  - Offers compatibility with MySQL while introducing unique features.
    
### Microsoft SQL Server:
Microsoft SQL Server is a commercial relational database management system (RDBMS) widely used in Windows-based enterprise applications and large organizations. It's known for its strong performance, scalability, and extensive features, particularly in business intelligence and data warehousing. SQL Server strictly adheres to data integrity standards and offers different editions to cater to diverse needs.
  - A commercial relational database management system developed by Microsoft.
  - Widely used in Windows-based enterprise applications and server environments.
  - Offers strong performance, scalability, and integration with Microsoft products.
  - Provides robust support for business intelligence and data warehousing.
  - Adheres to ACID compliance and offers advanced security features.
  - Comes with a range of editions to suit different needs, from small businesses to large

## <p align="left"> Ques-2. Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL) </p>
### DDL (Data Definition Language):
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.

### *List of DDL commands:*
 
*CREATE:* This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).

*DROP:* This command is used to delete objects from the database.

*ALTER:* This is used to alter the structure of the database.

*TRUNCATE:* This is used to remove all records from a table, including all spaces allocated for the records are removed.

*COMMENT:* This is used to add comments to the data dictionary.

*RENAME:* This is used to rename an object existing in the database.


## DML(Data Manipulation Language):
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.

### *List of DML commands:*

*INSERT:* It is used to insert data into a table.

*UPDATE:* It is used to update existing data within a table.

*DELETE:* It is used to delete records from a database table.


## DCL (Data Control Language):
DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system.

### *List of DCL commands:*

*GRANT:* This command gives users access privileges to the database.

*REVOKE:* This command withdraws the user’s access privileges given by using the GRANT command.


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
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.| Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT

## <p align="left"> Ques-3. How to apply Constraints at various levels. </p>

Constraints in the context of a relational database management system (RDBMS) are rules and conditions that are applied to the data in a database to ensure data integrity, accuracy, and consistency. They define the limitations and requirements for the data stored in database tables, helping to maintain the quality and reliability of the data. Constraints can be applied at various levels in a database, such as table level, column level, and database level. 

Some common types of constraints include:

### *Primary Key Constraint:*
Ensures that a column or a set of columns contains unique values, and no two rows can have the same values in the primary key column(s). It uniquely identifies each row in a table.
### *Unique Key*
Ensures that the values in a column or a set of columns are unique, but it doesn't necessarily require the uniqueness to identify each row. Multiple rows can have the same value as long as it's unique within the specified column(s).
### *Check Constraint*
Defines a condition or expression that must be true for data to be inserted or updated in a column. It allows you to enforce specific business rules or data validation.
### *Foreign Key*
Maintains referential integrity by linking a column in one table to the primary key of another table. This ensures that values in the foreign key column exist in the referenced table's primary key column.
### *Not Null*
Requires that a column cannot have a null (empty) value. It enforces the presence of data in the specified column.
### *Check Constraint*
Defines a condition that must be satisfied for data to be valid in a column. For example, you can use this constraint to enforce minimum or maximum values, data formats, or any custom business rules.

To apply constraints on a table named "student," you would typically use SQL statements. Here's an example of how you can create a "student" table with various constraints. Certainly, you can apply a foreign key constraint in the "student" table to establish a relationship with another table, such as a "courses" table. This relationship can represent the courses that each student is enrolled in. Here's an example of how to add a foreign key constraint to the "student" table:

 python
CREATE TABLE courses (
    course_id INT PRIMARY KEY,
    course_name VARCHAR(100)
);

CREATE TABLE student (
    student_id INT PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    date_of_birth DATE,
    email VARCHAR(100) UNIQUE,
    enrollment_date DATE,
    major VARCHAR(50) NOT NULL,
    GPA DECIMAL(3, 2) CHECK (GPA >= 0.0 AND GPA <= 4.0),
    course_enrolled INT,
    FOREIGN KEY (course_enrolled) REFERENCES courses(course_id)
);


