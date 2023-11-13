# <p align = "center">RDBMS Practical File</p>
# 1. Comparative study of various types of Database Managrment System.
### A Database Management System (DBMS) is a specialized software designed to store, retrieve, and manipulate data. It acts as a mediator between the database, applications, and user interfaces to manage and organize data effectively. The system provides a comprehensive suite of tools to govern databases, ensuring data security, consistency, and integrity. Types of dbms are: -

## Relational or SQL databases
### A relational database management system (RDBMS) is an information repository that organizes data into tables consisting of rows (records) and columns (attributes that contain the properties of these records). Each table represents a relation, and the rows (also called tuples) hold individual records within that relation. RDBMSs have a predefined schema with a strict structure and clear dependencies between different data points. Scalability. Relational databases usually scale vertically, meaning data lives on a single server, and scaling is done by adding more computer (CPU, GPU, and RAM) power to that one server. Performance. Relational databases perform well with intensive read/write operations on small to medium datasets. They also offer improved speed of data retrieval by adding indexes to data fields to query and join tables. 
### Security. Due to the integrated structure and data storage system, SQL databases don’t require much engineering effort to render them well-protected. They are a good choice for building and supporting complex software solutions, where any interaction has a range of consequences. 
### Most Commonly used database systems in SQL are: -
## MySQL
### MySQL is one of the most popular relational database systems. Originally an open-source solution, MySQL is now owned by Oracle Corporation. Today, MySQL is a pillar of LAMP application software. That means it’s a part of Linux, Apache, MySQL, and Perl/PHP/Python stack. Having C and C++ under the hood, MySQL works well with such system platforms as Windows, Linux, MacOS, IRIX, and others.
## MariaDB
### MariaDB  an open-source fork from MySQL, is a great SQL database example with commercial support. It works under a GNU General Public License and has similar commands, APIs, and libraries to MySQL.

## Non-Relational or NoSQL databases
### A non-relational or non-tabular database uses different data models for storing, managing, and accessing data. The most common data models are
   #### • document-oriented — to store, retrieve, and manage data such as JSON documents;
   #### • key-value — to represent data as a collection of key-value pairs, where keys are unique strings having corresponding data values;
   #### • graph — to store data in the node-edge-node structure where nodes are data points and edges are their relationships; and
   #### • wide-column — to store data in the tabular format with flexible columns, meaning they can vary from row to row in the same table.
### As these databases aren’t limited to a table structure, they are called NoSQL. They allow for storing unstructured data such as texts, photos, videos, PDF files, and a bunch of other formats. Data is simple to query but isn’t always classified into rows and columns as in a relational database. Scalability. When the number of data and requests increases, non-relational or NoSQL databases are usually scaled horizontally by adding more servers to the pool. They share data between various servers where each contains only a part of the data, decreasing the request-per-second rate in each server. Performance. Non-relational databases are known for their high performance: They have a distributed design, which lowers the performance load on the system and provides a large number of users with simultaneous access. 
### Security. Unlike relational systems, NoSQL databases have weak security, making them a major concern for many infrastructures. While they may provide ACID guarantees, they are typically available within the scope of one database partition. However, some DBMSs offer advanced security features that meet strict security and compliance standards.
### Most Commonly used database systems in NoSQL are: -
## MongoDB
### A free, open-source, non-relational DBMS, MongoDB also includes a commercial version. Although MongoDB wasn’t initially intended for structured data processing, it can be employed for applications that use both structured and unstructured data. In MongoDB, databases are connected to applications via database drivers. They are widely available within the database management system. Multiple data types are processed simultaneously and use the internal cache for this purpose.
## Redis
### An open-source, NoSQL, in-memory data structure store, Redis can also be used as a cache. Instead of documents, it uses key-value pairs. Its distinct feature is that there are several options for data structuring, such as lists, sets, and hashes.
# 2. Data Definition Language (DDL), Data Manipulation Language (DML), Data Control Language (DCL).
### SQL commands are like instructions to a table. It is used to interact with the database with some operations. It is also used to perform specific tasks, functions, and queries of data. SQL can perform various tasks like creating a table, adding data to tables, dropping the table, modifying the table, set permission for users.
### These SQL commands are mainly categorized into five categories:
   #### 1. DDL – Data Definition Language
   #### 2. DQL – Data Query Language
   #### 3. DML – Data Manipulation Language
   #### 4. DCL – Data Control Language
   #### 5. TCL – Transaction Control Language

## DATA DEFINITION LANGUAGE (DDL): -
### Ddl or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
### List of DDL commands: 
   #### • CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
   #### • DROP: This command is used to delete objects from the database.
   #### • ALTER: This is used to alter the structure of the database.
   #### • TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
   #### • COMMENT: This is used to add comments to the data dictionary.
   #### • RENAME: This is used to rename an object existing in the database.

## DATA MANIPULATION LANGUAGE (DML): -
### The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
### List of DML commands:
   #### • INSERT: It is used to insert data into a table.
   #### • UPDATE: It is used to update existing data within a table.
   #### • DELETE: It is used to delete records from a database table.
   
## DATA CONTROL LANGUAGE (DCL): -
### DCL includes commands such as GRANT and REVOKE which mainly deal with the rights, permissions, and other controls of the database system.
### List of DCL commands:
### GRANT: This command gives users access privileges to the database.
#### Syntax:
#### GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;
### REVOKE: This command withdraws the user’s access privileges given by using the GRANT command.
#### Syntax:
#### REVOKE SELECT, UPDATE ON MY_TABLE FROM USER1, USER2;
# 3. How to apply constraints at various levels
### NOT NULL Constraint: - The NOT NULL constraint enforces a column to NOT accept NULL values. This enforces a field to always contain a value, which means that you cannot insert a new record, or update a record without adding a value to this field.
![NOT_CON](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/5a65a75c-3350-4536-9ec0-6822d4852494)
### PRIMARY KEY Constraint: - The PRIMARY KEY constraint uniquely identifies each record in a table. Primary keys must contain UNIQUE values, and cannot contain NULL values. A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).
![PRIMARY_CON](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/3f93b749-476a-4d47-ab1b-b6ab41974122)
### CHECK Constraint: - The CHECK constraint is used to limit the value range that can be placed in a column. If you define a CHECK constraint on a column it will allow only certain values for this column. If you define a CHECK constraint on a table it can limit the values in certain columns based on values in other columns in the row.
![CHECK_CON](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/47011998-4622-4f0e-8753-19c7e8ebfe66)
### DEFAULT Constraint: - The DEFAULT constraint is used to set a default value for a column. The default value will be added to all new records, if no other value is specified.
![DEFAULT_CON](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/a3c1a9a9-b207-43ee-9bdf-5808f646cd51)
# 4. View data in the required form using Operators, Function and Joins.
### OPERATORS: -
### 1. Comparison Operators: -
   #### • =: Equal to
   #### • != or <>: Not equal to
   #### • <: Less than
   #### • >: Greater than
   #### • <=: Less than or equal to
   #### • >=: Greater than or equal to
   ![add_op](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/edc5fcd2-e5f5-4d13-bcb2-799d1574fc23)
### 2. Logical Operators: -
   #### • AND: Logical AND
   #### • OR: Logical OR
   #### • NOT: Logical NOT
   ![logical_op](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/c7a1fe65-599c-41df-a55f-872e91bb0004)
### 3. IS NULL operator: -
 #### • Used to check for the absence of a value in a column.
 ![IS_OP](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/b22000ed-5c7a-4c48-98d6-5ab8d91a0647)
### 4. IN Operator: -
   #### • Used to specify a list of values to match against in a WHERE clause.
   ![IN_OP](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/e3cce972-82ba-425a-a9cf-ae085e88cad5)
### 5. BETWEEN Operator: -
  #### • Used to select a range of values.
  ![BETWEEN_OP](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/57fd3c46-7870-4c35-b1ae-5408bec4463c)
### 6. LIKE Operator: -
   #### • Used for pattern matching with wildcard characters (% for multiple characters and _ for a single character).
   ![LIKE_OP](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/015a0640-0cf3-4a5b-a266-4f860f9e69d9)
## FUNCTIONS: -
### 1. AGGREATE Function: - Aggregate functions operate on a set of values and return a single result. Common aggregate functions include:
   #### • COUNT(): Counts the number of rows.
   #### • SUM(): Calculates the sum of numeric values.
   #### • AVG(): Computes the average of numeric values.
   #### • MIN(): Returns the minimum value.
   #### • MAX(): Returns the maximum value.
   ![AGG_FUN](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/bc158f72-3667-41c3-ac8a-809b5353f0be)
### 2. STRING Function: -String functions allow you to manipulate text data.
   #### • CONCAT(): Combines two or more strings.
   #### • SUBSTRING(): Extracts a substring from a string.
   #### • UPPER(), LOWER(): Converts text to uppercase or lowercase.
   #### • LENGTH(), CHAR_LENGTH(): Returns the length of a string.
   
![STRING_FUN](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/f696c3fc-5d24-47b3-beda-bc83ccd10f0e)
### 3. MATHEMATICAL Function: - Mathematical functions perform numeric calculations.
   #### • ABS(): Returns the absolute value of a number.
   #### • ROUND(): Rounds a numeric value to a specified number of decimal places.
   #### • SQRT(): Calculates the square root of a number.
   ![MATH_FUN](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/bbcf75a8-03b9-4762-a3d0-cd14e7d17958)
## JOINS: -
### 1. INNER JOIN: - An INNER JOIN returns only the rows that have matching values in both tables being joined. It excludes rows with non-matching values in either table.

![INNER_JJ](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/31c28ac6-b616-4118-801d-5446bfc6a40a)

### 2. LEFT OUTER JOIN: - A LEFT JOIN returns all the rows from the left table and the matched rows from the right table. If there is no match in the right table, NULL values are returned.
![Selection_001](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/3720742f-491b-4b31-973a-5264992ddf5b)
