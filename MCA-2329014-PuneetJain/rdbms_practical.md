# <p align="center">Guru Nanak Dev Engineering College, Ludhiana</p>
![front](https://user-images.githubusercontent.com/82715927/121130621-4a076380-c84c-11eb-85e0-81619d36d244.png)

### <p align="center">Practical File</p>
### <p align="center">Of</p>
### <p align="center">Relational Database Management Systems Lab</p>
### <p align="center">Course Code: "PGCA- 2208"</p>
### <p><h3 align="left">Submitted to :</br>Mr.Satinderpal Singh</h3><h3 align="right">Submitted by: </br>Puneet Jain</br>(MCA 1st sem.)</br>CRN:-2029014</h3></p>

Sr no|  Experiment Name |  Remarks|   
|---|---|---|
|  1| Comparative study of various Database Management Systems.  |   |   
|  2|Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL).   |   |   
|  3|How to apply Constraints at various levels. |   |   
|  4|View data in the required form using Operators, Functions and Joins.  |  |
|  5|Creating different types of Views for tailored presentation of data.  |  |
|  6|How to apply Conditional Controls in PL/SQL.   |  |
|  7|Error Handling using Internal Exceptions and External Exceptions.   |  |
|  8|Using various types of Cursors   |  |
|  9|How to run Stored Procedures and Functions.   |  |
|  10|Creating Packages and applying Triggers.   |  |
|  11|Creating Arrays and Nested Tables.  |  |

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## *1. Comparative study of various Database Management Systems.*
***Database Management System:***
A Database Management System (DBMS) is a specialized software designed to store, retrieve, and manipulate data. It acts as a mediator between the database, applications, and user interfaces to manage and organize data effectively. The system provides a comprehensive suite of tools to govern databases, ensuring data security, consistency, and integrity.

A DBMS supports various applications, from simple storage and retrieval tasks to complex data-driven systems, by implementing efficient data access and management practices. Additionally, the system can handle concurrent users, maintain transactional consistency, and provide robust backup and recovery options, making it an essential component in any data-centric environment.

**Types of databases:**
</br>(1)MySQL </br>(2)MariaDB </br>(3)Oracle </br>(4)PostgreSQL </br>(5)SQLite 

## ***(1)MySQL***-
MySQL is one of the most popular relational database systems. Originally an open-source solution, MySQL is now owned by Oracle Corporation. Today, MySQL is a pillar of LAMP application software. That means it’s a part of Linux, Apache, MySQL, and Perl/PHP/Python stack. Having C and C++ under the hood, MySQL works well with such system platforms as Windows, Linux, MacOS, IRIX, and others.

### **Pros of MySQL:**

**(i) Free installation**-The community edition of MySQL is free to download. With a basic set of tools for individual use, MySQL community edition is a good option, to begin with. Of course, there are other, prepaid versions for Enterprise or Cluster purposes with richer functionality. Nevertheless, if your company is too small to pay for one of them, the free-to-download model is the most suitable for a fresh start.

**(ii) Simple syntax and mild complexity**-MySQL’s structure and style are very plain. Developers even consider MySQL a database with a human-like language. MySQL is often used in tandem with the PHP programming language. Because they share a gentle learning curve, it’s much easier to form a team to manage your database. Also, MySQL is easy to use. For instance, most of the tasks can be executed right in the command line, reducing development steps.

**(iii) Cloud compatibility**-Business-oriented by nature and originally developed for the web, MySQL is supported by the most popular cloud providers.  It’s available on leading platforms like Amazon, Microsoft, and others. This makes MySQL even more attractive and gives businesses room for growth.

### **Cons of MySQL:**

**(i) Scalability challenges**-MySQL was not built with scalability in mind, which is inherent in its code. Theoretically, you can scale MySQL, but it will need more engineering effort than any of the NoSQL databases. So, if you expect one day your database will increase substantially, keep this limitation in mind or choose another DBMS option.

**(ii)Partial open-source support**-Although MySQL has an open-source part, it’s mostly under Oracle’s license. This limits the MySQL community in terms of improving the DBMS. Why do you care? Because when you have completely open-source support, you expect many problem-specific implementations and community assistance. This is not the case when the software belongs to corporate owners, and you have to pay for support.

**(iii)Limited compliance with SQL standards**-Structured Query Language has specific standards. MySQL doesn’t completely follow them, i.e., MySQL provides no support for some standard SQL features. On the other hand, MySQL has some extensions and distinct features that don’t match the Structured Query Language standards. It’s not a big deal for small web applications. The issues may appear when you have to shift to other databases, which will likely happen when your business starts growing.

## ***(2)MariaDB***-
MariaDB, an open-source fork from MySQL, is a great SQL database example with commercial support. It works under a GNU General Public License and has similar commands, APIs, and libraries to MySQL.

### **Pros of MariaDB:**

**(i)Encryption**-For MariaDB, open source doesn’t mean insecure. In addition to internal security and password check, MariaDB provides such features as PAM and LDAP authentication, Kerberos, and user roles. Combined with encrypted tablespaces, tables, and logs, it creates a robust protective layer for data. Beyond that, MariaDB publishes related releases on each security update, keeping the security patches totally transparent.

**(ii)Broad functionality**-MariaDB has introduced a lot of new features in the last few years. For instance, GIS support suggests smooth coordinate storage and location data queries. Dynamic columns allow a single DBMS to provide both SQL and NoSQL data handling for different needs. You can also extend its functionality with plugins that are available at MySQL via 3rd parties only. MariaDB is shipped with storage engines for NoSQL backend, legacy database migration tools, sharding options, and much more.

**(iii)High performance**-Although MariaDB originates from the MySQL engine, it’s gotten very far in terms of performance. Extensive optimization features improve thread pool management and data processing. Thus, when rows from the table are deleted, the operating system immediately accesses the free space, eliminating gaps in the tablespace. On top of that, the database management system suggests engine-independent table statistics. This feature enhances the optimizer’s performance, accelerates query processing, and helps customize data analysis.

### **Cons of MariaDB:**

**(i)Still a growing community**-Although MariaDB has substantial open-source contribution, its community has yet to grow much. Since this database management system was established not so long ago, the number of professionals involved is relatively small.

**(ii)Gaps between MySQL and MariaDB update versions**-Though the MariaDB team is constantly merging its code with MySQL’s, it’s already not that simple to keep them in line. Given the currently existing differences between MariaDB 10.6 and MySQL 8.0.32, further deviations are yet to come. Additionally, MySQL engineers introduced some native features to the code that are only available to commercial MySQL users. This can create compatibility issues or data migration problems from MariaDB back to MySQL.

## ***(3)Oracle***-
Oracle is a relational database management system created and run by the Oracle Corporation. Among all the types of SQL databases, Oracle stands out. Currently, it supports multiple data models like document, graph, relational, and key-value within a single database. In its latest releases, it refocused on cloud computing. Oracle database engine licensing is fully proprietary, with both free and paid options available.

## **Pros of Oracle:**

**(i)Innovations for daily workflow**-Starting with the Oracle 12c release, when the software entered the hybrid cloud era, new cloud computing technologies appeared regularly. With every new release, Oracle tries to keep up with the innovation pace while focusing on information security, including active data guard, partitioning, improved backup, and recovery.

**(ii)Large capacity**-Oracle’s multi-model solution allows for accommodating and processing a vast amount of data. Thanks to the recently released multi-tenancy feature, the database architecture now simplifies packing many databases and manages them smoothly. In combination with in-memory data processing capabilities, it creates a strong engine for synchronous data processing.

## **Cons of Oracle:**

**(i)High cost**-Though the Oracle database has free editions, they are very limited in terms of functionality. Standard Edition, which doesn’t include all available features, costs $17,500 per unit. The Enterprise Edition is over $47,000 per unit.

**(ii)Resource-consuming technology**-The Oracle database needs powerful infrastructure. Not only does installation require a lot of disk space, but you’ll also have to consider constant hardware updates if you deploy it on-premises.

**(iii)Hard learning curve**-Oracle database is not a system to start using right away. It’s better to have certified Oracle DB engineers to run it. Oracle’s documentation, while covering many issues, can sometimes be overwhelming and even confusing. So, to install and run an Oracle database, you’ll have to consider hiring dedicated experts.

## ***(4)PostgreSQL***- 
The PostgreSQL database management system shares its popularity with MySQL. This is an object-relational DBMS where user-defined objects and table approaches are combined to build more complex data structures. Besides that, PostgreSQL has a lot of similarities with MySQL. It’s aimed at strengthening the standards of compliance and extensibility. Consequently, it can process any workload, for both single-machine products and complex applications. Owned and developed by PostgreSQL Global Development Group, it still remains completely open-source. This DBMS is available for use with platforms like Microsoft, iOS, Android, and many more.

## **Pros of PostgreSQL:**

**(i)Great scalability**-Vertical scalability is a hallmark of PostgreSQL. Considering that almost any custom software solution tends to grow, resulting in database extension, this particular option certainly supports business growth and development.

**(ii)Support for custom data types**-PostgreSQL natively supports many data types by default, such as JSON, XML, H-Store, and others. PostgreSQL takes advantage of it, being one of the few relational databases with strong support for NoSQL features. Additionally, it allows users to define their own data types. As your software business model may need different types of databases throughout its existence for better performance or application comprehensiveness, this option brings improved flexibility to the table.

**(iii)Easily-integrated third-party tools**-The PostgreSQL database management system has the strong support of additional tools, both free and commercial. The scope of these includes extensions to improve many aspects. For example, ClusterControl provides impressive assistance in managing, monitoring, and scaling SQL and NoSQL open-source databases. To make data comparison and synchronization more effective, consider using DB Data Directive. In case you’re going to scale up your data to heavy workloads, the pgBackRest backup and restore system will be a nice option to choose from.

**(iv)Open-source and community-driven support**-Postgres is completely open-source and supported by its community, strengthening it as a complete ecosystem. Additionally, developers can always expect free and prompt community assistance.

## **Cons of PostgreSQL:**

**(i)Inconsistent documentation**-While PostgreSQL has a large community and strongly supports its participants, the documentation still lacks consistency and completeness. As the PostgreSQL community is rather distributed, the documentation doesn’t follow uniform standards for all Postgre features.

**(ii)Lack of reporting and auditing instruments**-A significant shortcoming of PostgreSQL is the absence of revising tools that would show the current condition of a database. You have to continuously check if something goes wrong. There’s always a risk that DB engineers will notice a failure too late.

## ***(5)SQLite***- 
SQLite is a self-sufficient, serverless, and no-configuration-required database management system. Frequently utilized as an embedded database, it is popular for small-scale mobile and desktop applications.

## **Pros of SQLite:**

**(i)Small in size and easily portable**-SQLite is a streamlined database engine that operates without a separate server process. The entire database is contained within a single cross-platform disk file, enhancing its portability and simplifying its integration into applications.

**(ii)Minimal resource consumption**-SQLite is engineered for optimal memory and disk space efficiency, making it an ideal choice for applications with constrained resources, such as those found in mobile and IoT devices.

**(iii)Reliable and user-friendly**-SQLite is an ACID-compliant database, ensuring the integrity and consistency of data. Additionally, it is simple to set up and demands minimal configuration.

## **Cons of SQLite:**

**(i)Restricted concurrency**-SQLite employs file-based locking, limiting its capacity to manage multiple concurrent write operations. This makes it less appropriate for applications with high write concurrency or multiple users accessing the database simultaneously.

**(ii)Absence of advanced features**-SQLite lacks some of the sophisticated features found in other database management systems, such as stored procedures, triggers, or user-defined functions.

**(iii)Restricted scalability**-Owing to its serverless structure, SQLite is not tailored for extensive applications or distributed settings. Its performance may diminish when handling substantial datasets or elevated levels of concurrent access.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## *2. Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL).*

## **DDL Commands**:

DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:

1-The CREATE command creates database objects, tables, and triggers.</br>
2-ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.</br>
3-The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.</br>
4-The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.</br>
5-The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.</br>

## **DML Commands**:

DML commands are SQL commands that perform operations like storing data in database tables, modifying and deleting existing rows, retrieving data, or updating data.

  1-The SELECT command fetches data or records from one or more tables in the SQL database. The retrieved data gets displayed in a result table known as the result set.</br>
  2-The INSERT command inserts one or more new records into the table in the SQL database.</br>
  3-The UPDATE command updates or changes the existing data or records in a table in the SQL database.</br>
  4-The DELETE command deletes all the existing records and the allocated spaces from a table in the SQL database. We can use the WHERE clause with the AND or OR operators to delete selected rows from the database.</br>
  5-The MERGE command deals with insertion, updation, and deletion in the same SQL statement.</br>
  6-The CALL command calls or invokes a stored procedure.</br>
  7-The EXPLAIN PLAN command describes the access path to the data. It returns the execution plans for the statements like INSERT, UPDATE, and DELETE in the readable format for users to check the SQL Queries.</br>
  8-The LOCK TABLE command ensures the consistency, atomicity, and durability of database transactions like reading and writing operations.</br>

## **DCL Commands**:

DCL commands are SQL commands that perform operations like giving and withdrawing database access from the user.

  1-The GRANT command gives access privileges or permissions like ALL, SELECT, and EXECUTE to the database objects like views, tables, etc, in SQL.</br>
  2-The REVOKE command withdraws access privileges or permissions given with the GRANT command.

## ***Differences Between DDL, DML,and DCL:***
DDL | DML | DCL
|---|---|---|
DDL stands for Data Definition Language.|DML stands for Data Manipulation Language.|DCL stands for Data Control Language.
It helps us to define the structure of the database.|It helps us to manage the data.|t helps us to control the access and permission of the database.
It affects the entire table data.|It only affects the specified row(s) of the table.|It applies to the complete table.
Changes are permanent.|We can roll back our changes in the DML language.|We can roll back the changes in the DCL language.
It helps in defining the fields or columns of the tables.|It helps us to define rows or records of the tables.|It helps us to control access to the information in the database.
They are auto-committed (changes made are permanent).|They are not auto-committed (changes are not permanent).|They are not auto-committed (changes are not permanent). 
They don't have further classification.|They are of two types procedural and non-procedural.|They don't have any further classification.
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## *3. How to apply Constraints at various levels.*
SQL constraints are used to specify rules for the data in a table.

Constraints are used to limit the type of data that can go into a table. This ensures the accuracy and reliability of the data in the table. If there is any violation between the constraint and the data action, the action is aborted.

Constraints can be column level or table level. Column level constraints apply to a column, and table level constraints apply to the whole table.

-The following constraints are commonly used in SQL:

  (1) NOT NULL - Ensures that a column cannot have a NULL value</br>
  (2) UNIQUE - Ensures that all values in a column are different</br>
  (3) PRIMARY KEY - A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table</br>
  (4) FOREIGN KEY - Prevents actions that would destroy links between tables</br>
  (5) CHECK - Ensures that the values in a column satisfies a specific condition</br>
  (6) DEFAULT - Sets a default value for a column if no value is specified</br>
  (7) CREATE INDEX - Used to create and retrieve data from the database very quickly</br>

## **(1) NOT NULL Constraint**- 
By default, a column can hold NULL values.

The NOT NULL constraint enforces a column to NOT accept NULL values.

This enforces a field to always contain a value, which means that you cannot insert a new record, or update a record without adding a value to this field.

_QUERY:_
```python
CREATE TABLE class (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int
);
```

_Output:_ 
![Screenshot from 2023-10-12 14-33-26](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/635a0b17-ff22-411e-805e-b541cb56acb1)


## **(2) UNIQUE Constraints**- 
The UNIQUE constraint ensures that all values in a column are different.

Both the UNIQUE and PRIMARY KEY constraints provide a guarantee for uniqueness for a column or set of columns.

A PRIMARY KEY constraint automatically has a UNIQUE constraint.

However, you can have many UNIQUE constraints per table, but only one PRIMARY KEY constraint per table.

_QUERY:_
```python
CREATE TABLE class (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int,
    UNIQUE(ID)
);
```

_Output:_ 
![Screenshot from 2023-10-12 14-47-24](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/f7e82b0f-9f41-4845-957b-b850f8c42ccd)


## **(3) PRIMARY KEY Constraint**- 
The PRIMARY KEY constraint uniquely identifies each record in a table.

Primary keys must contain UNIQUE values, and cannot contain NULL values.

A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).

_QUERY:_
```python
CREATE TABLE class (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int,
    PRIMARY KEY(ID)
);
```

_Output:_ 
![Screenshot from 2023-10-12 15-01-58](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/e78fb133-cec2-47ce-8f2c-04a1166f1c96)


## **(4) FOREIGN KEY Constraint**- 
The FOREIGN KEY constraint is used to prevent actions that would destroy links between tables.

A FOREIGN KEY is a field (or collection of fields) in one table, that refers to the PRIMARY KEY in another table.

The table with the foreign key is called the child table, and the table with the primary key is called the referenced or parent table.

_QUERY:_
```python
CREATE TABLE Department (
     DepID int,
     Field varchar(255),
     ID int,
     PRIMARY KEY(DepID),
     FOREIGN KEY(ID) REFERENCES class(ID)
);
```

_Output:_ 
![Screenshot from 2023-10-12 15-36-47](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/79c9fbec-f961-4cd4-a733-7c27dc3e10e5)


## **(5) CHECK Constraint**- 
The CHECK constraint is used to limit the value range that can be placed in a column.

If you define a CHECK constraint on a column it will allow only certain values for this column.

If you define a CHECK constraint on a table it can limit the values in certain columns based on values in other columns in the row.

_QUERY:_
```python
CREATE TABLE class (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int CHECK (Age<=23)
);
```

_Output:_ 
![Screenshot from 2023-10-12 15-56-38](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/344b8328-ca8e-49c7-8963-c9c0982fc8e3)


## **(6) DEFAULT Constraint**- 
The DEFAULT constraint is used to set a default value for a column.

The default value will be added to all new records, if no other value is specified.

_QUERY:_
```python
CREATE TABLE office(
       EmpName varchar(100) not null default'unnamed',
       Age int not null default'22',
       City varchar(100) default'Ludhiana'
);
```

_Output:_
![Screenshot from 2023-10-12 20-44-31](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/8990c3e0-3fe2-4018-8223-9de2a8c2d0b7)


## **(7) CREATE INDEX Statement**- 
The CREATE INDEX statement is used to create indexes in tables.

Indexes are used to retrieve data from the database more quickly than otherwise. The users cannot see the indexes, they are just used to speed up searches/queries.

_QUERY:_
```python
CREATE TABLE class (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int
);
 CREATE INDEX idx_LastName on class(LastName);
```

_Output:_
![Screenshot from 2023-10-12 20-55-10](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/1953aa5e-97e8-4c44-94f5-216fb728d2ca)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## *4. View data in the required form using Operators, Functions and Joins.*

### **Using operators-**
**(1) Arithmetic Operators:**

Operators| Description
|---|---|
|+  |Add|
|- 	|Subtract| 	
|* 	|Multiply| 	
|/ 	|Divide 	|
|% 	|Modulo|

_QUERY:_
```python
SELECT 50+50,50-50,50*50,50/50,50%50;
```
_Output:_
![Screenshot from 2023-11-02 12-43-59](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/0da1cf25-e63e-4932-b096-82fa94611f8b)

**(2) Bitwise Operators:**

Operators| Description
|---|---|
|& 	|Bitwise AND|
|1 |Bitwise OR|
|^ 	|Bitwise exclusive OR|

_QUERY:_
```python
select 25&20,25|20,25^20;
```
_Output:_
![Screenshot from 2023-11-02 12-57-26](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/7e0f709c-cf99-42cb-9d56-f13c6a0b4ee5)

**(3) Comparison Operators:**

Operators| Description
|---|---|
|= 	|Equal to |	
|> 	|Greater than |	
|< 	|Less than 	|
|>= 	|Greater than or equal to| 	
|<= 	|Less than or equal to 	|
|<> 	|Not equal to|

_QUERY:_
```python
SELECT 30=20,30>20,30<20,30>=30,30<=20,30<>20;
```
_Output:_
![Screenshot from 2023-11-02 13-04-48](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/3dada540-e74a-4eff-a28f-698f329bfaf6)

**(4) Logical Operators:**

Operators| Description
|---|---|
|ALL 	|TRUE if all of the subquery values meet the condition 	|
|AND 	|TRUE if all the conditions separated by AND is TRUE 	|
|ANY |	TRUE if any of the subquery values meet the condition 	|
|BETWEEN 	|TRUE if the operand is within the range of comparisons 	|
|EXISTS 	|TRUE if the subquery returns one or more records 	|
|IN 	|TRUE if the operand is equal to one of a list of expressions 	|
|LIKE 	|TRUE if the operand matches a pattern 	|
|NOT 	|Displays a record if the condition(s) is NOT TRUE 	|
|OR 	|TRUE if any of the conditions separated by OR is TRUE 	|
|SOME 	|TRUE if any of the subquery values meet the condition|

_QUERY:_
```python
SELECT * from class where Age=All(select Age from class where Age=16);
SELECT * from class where LastName="Jain" AND Age="16";
SELECT * from class where Age BETWEEN 16 AND 18;

```
_Output:_
![Screenshot from 2023-11-02 13-26-51](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/dd0a28f5-76e8-40de-8df0-3f23fc522768)

### **Using Functions-**
MySQL has many built-in functions.
</br>This reference contains string, numeric, date, and some advanced functions in MySQL.

**(1) String Functions:**

Function| Description
|---|---|
|ASCII 	|Returns the ASCII value for the specific character|
|CHAR_LENGTH 	|Returns the length of a string (in characters)|
|CHARACTER_LENGTH 	|Returns the length of a string (in characters)|
|CONCAT 	|Adds two or more expressions together|
|CONCAT_WS 	|Adds two or more expressions together with a separator|
|FIELD 	|Returns the index position of a value in a list of values|
|FIND_IN_SET 	|Returns the position of a string within a list of strings|
|FORMAT 	|Formats a number to a format like "#,###,###.##", rounded to a specified number of decimal places|
|INSERT 	|Inserts a string within a string at the specified position and for a certain number of characters|
|INSTR 	|Returns the position of the first occurrence of a string in another string|
|LCASE 	|Converts a string to lower-case|
|LEFT 	|Extracts a number of characters from a string (starting from left)|
|LENGTH 	|Returns the length of a string (in bytes)|
|LOCATE |	Returns the position of the first occurrence of a substring in a string|
|LOWER 	|Converts a string to lower-case|
|LPAD 	|Left-pads a string with another string, to a certain length|
|LTRIM 	|Removes leading spaces from a string|
|MID 	|Extracts a substring from a string (starting at any position)|
|POSITION 	|Returns the position of the first occurrence of a substring in a string|
|REPEAT 	|Repeats a string as many times as specified|
|REPLACE 	|Replaces all occurrences of a substring within a string, with a new substring|
|REVERSE 	|Reverses a string and returns the result|
|RIGHT 	|Extracts a number of characters from a string (starting from right)|
|RPAD 	|Right-pads a string with another string, to a certain length|
|RTRIM 	|Removes trailing spaces from a string|
|SPACE |Returns a string of the specified number of space characters|
|STRCMP 	|Compares two strings|
|SUBSTR 	|Extracts a substring from a string (starting at any position)|
|SUBSTRING 	|Extracts a substring from a string (starting at any position)|
|SUBSTRING_INDEX 	|Returns a substring of a string before a specified number of delimiter occurs|
|TRIM 	|Removes leading and trailing spaces from a string|
|UCASE 	|Converts a string to upper-case|
|UPPER 	|Converts a string to upper-case|

_QUERY:_
```python
SELECT ascii('t');
SELECT char_length('MyNameIsPuneetJain');
```
_Output:_
![Screenshot from 2023-11-02 13-58-01](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/9397a16d-0839-4d9d-8701-83fd1a2c446c)


**(2) Numeric Functions:**
Function| Description
|---|---|
|ABS 	|Returns the absolute value of a number|
|ACOS 	|Returns the arc cosine of a number|
|ASIN 	|Returns the arc sine of a number|
|ATAN 	|Returns the arc tangent of one or two numbers|
|ATAN2 	|Returns the arc tangent of two numbers|
|AVG 	|Returns the average value of an expression|
|CEIL 	|Returns the smallest integer value that is >= to a number|
|CEILING 	|Returns the smallest integer value that is >= to a number|
|COS 	|Returns the cosine of a number|
|COT 	|Returns the cotangent of a number|
|COUNT 	|Returns the number of records returned by a select query|
|DEGREES 	|Converts a value in radians to degrees|
|DIV 	|Used for integer division|
|EXP 	|Returns e raised to the power of a specified number|
|FLOOR 	|Returns the largest integer value that is <= to a number|
|GREATEST 	|Returns the greatest value of the list of arguments|
|LEAST 	|Returns the smallest value of the list of arguments|
|LN 	|Returns the natural logarithm of a number|
|LOG 	|Returns the natural logarithm of a number, or the logarithm of a number to a specified base|
|LOG10 	|Returns the natural logarithm of a number to base 10|
|LOG2 	|Returns the natural logarithm of a number to base 2|
|MAX 	|Returns the maximum value in a set of values|
|MIN 	|Returns the minimum value in a set of values|
|MOD 	|Returns the remainder of a number divided by another number|
|PI 	|Returns the value of PI|
|POW 	|Returns the value of a number raised to the power of another number|
|POWER 	|Returns the value of a number raised to the power of another number|
|RADIANS 	|Converts a degree value into radians|
|RAND 	|Returns a random number|
|ROUND 	|Rounds a number to a specified number of decimal places|
|SIGN 	|Returns the sign of a number|
|SIN 	|Returns the sine of a number|
|SQRT 	|Returns the square root of a number|
|SUM 	|Calculates the sum of a set of values|
|TAN 	|Returns the tangent of a number|
|TRUNCATE 	|Truncates a number to the specified number of decimal places|

_QUERY:_
```python
SELECT ABS(-243.5);
SELECT ACOS(0.25);
SELECT ATAN(2.5);
SELECT CEIL(25.75);
```
_Output:_
![Screenshot from 2023-11-02 14-03-11](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/07e97868-a6ac-41f0-b2ba-1b288704073e)

**(3)Date Functions**
Function| Description
|---|---|
|Function 	|Description|
|ADDDATE 	|Adds a time/date interval to a date and then returns the date|
|ADDTIME 	|Adds a time interval to a time/datetime and then returns the time/datetime|
|CURDATE |	Returns the current date|
|CURRENT_DATE 	|Returns the current date|
|CURRENT_TIME 	|Returns the current time|
|CURRENT_TIMESTAMP 	|Returns the current date and time|
|CURTIME 	|Returns the current time|
|DATE 	|Extracts the date part from a datetime expression|
|DATEDIFF 	|Returns the number of days between two date values|
|DATE_ADD 	|Adds a time/date interval to a date and then returns the date|
|DATE_FORMAT 	|Formats a date|
|DATE_SUB 	|Subtracts a time/date interval from a date and then returns the date|
|DAY 	|Returns the day of the month for a given date|
|DAYNAME 	|Returns the weekday name for a given date|
|DAYOFMONTH 	|Returns the day of the month for a given date|
|DAYOFWEEK 	|Returns the weekday index for a given date|
|DAYOFYEAR 	|Returns the day of the year for a given date|
|EXTRACT 	|Extracts a part from a given date|
|FROM_DAYS 	|Returns a date from a numeric datevalue|
|HOUR |	Returns the hour part for a given date|
|LAST_DAY 	|Extracts the last day of the month for a given date|
|LOCALTIME 	|Returns the current date and time|
|LOCALTIMESTAMP 	|Returns the current date and time|
|MAKEDATE 	|Creates and returns a date based on a year and a number of days value|
|MAKETIME 	|Creates and returns a time based on an hour, minute, and second value|
|MICROSECOND 	|Returns the microsecond part of a time/datetime|
|MINUTE 	|Returns the minute part of a time/datetime|
|MONTH 	|Returns the month part for a given date|
|MONTHNAME |	Returns the name of the month for a given date|
|NOW| 	Returns the current date and time|
|PERIOD_ADD 	|Adds a specified number of months to a period|
|PERIOD_DIFF |	Returns the difference between two periods|
|QUARTER 	|Returns the quarter of the year for a given date value|
|SECOND 	|Returns the seconds part of a time/datetime|
|SEC_TO_TIME 	|Returns a time value based on the specified seconds|
|STR_TO_DATE 	|Returns a date based on a string and a format|
|SUBDATE| 	Subtracts a time/date interval from a date and then returns the date|
|SUBTIME 	|Subtracts a time interval from a datetime and then returns the time/datetime|
|SYSDATE |	Returns the current date and time|
|TIME 	|Extracts the time part from a given time/datetime|
|TIME_FORMAT 	|Formats a time by a specified format|
|TIME_TO_SEC 	|Converts a time value into seconds|
|TIMEDIFF 	|Returns the difference between two time/datetime expressions|
|TIMESTAMP |	Returns a datetime value based on a date or datetime value|
|TO_DAYS |	Returns the number of days between a date and date "0000-00-00"|
|WEEK 	|Returns the week number for a given date|
|WEEKDAY 	|Returns the weekday number for a given date|
|WEEKOFYEAR 	|Returns the week number for a given date|
|YEAR 	|Returns the year part for a given date|
|YEARWEEK 	|Returns the year and week number for a given date|

_QUERY:_
```python
SELECT NOW();
SELECT CURDATE();
SELECT CURTIME();
```
_Output:_
![Screenshot from 2023-11-02 14-11-28](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/e14ca96d-2411-42f7-b464-14996ad1170c)

**(4) Advanced Functions:**
Function| Description
|---|---|
|BIN 	|Returns a binary representation of a number|
|BINARY 	|Converts a value to a binary string|
|CASE 	|Goes through conditions and return a value when the first condition is met|
|CAST 	|Converts a value (of any type) into a specified datatype|
|COALESCE 	|Returns the first non-null value in a list|
|CONNECTION_ID 	|Returns the unique connection ID for the current connection|
|CONV 	|Converts a number from one numeric base system to another|
|CONVERT |	Converts a value into the specified datatype or character set|
|CURRENT_USER| 	Returns the user name and host name for the MySQL account that the server used to authenticate the current client|
|DATABASE 	|Returns the name of the current database|
|IF 	|Returns a value if a condition is TRUE, or another value if a condition is FALSE|
|IFNULL 	|Return a specified value if the expression is NULL, otherwise return the expression|
|ISNULL |	Returns 1 or 0 depending on whether an expression is NULL|
|LAST_INSERT_ID |	Returns the AUTO_INCREMENT id of the last row that has been inserted or updated in a table|
|NULLIF 	|Compares two expressions and returns NULL if they are equal. Otherwise, the first expression is returned|
|SESSION_USER 	|Returns the current MySQL user name and host name|
|SYSTEM_USER 	|Returns the current MySQL user name and host name|
|USER 	|Returns the current MySQL user name and host name|
|VERSION 	|Returns the current version of the MySQL database|


_QUERY:_
```python
SELECT BIN(18);
SELECT BINARY"PuneetJain";
SELECT CONNECTION_ID();
SELECT CURRENT_USER();
SELECT DATABASE();
```
_Output:_
![Screenshot from 2023-11-02 14-16-44](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/7a22eb25-90bf-4583-8e8d-6d78c249f1f1)



### **Using JOINS-**
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

**Different Types of SQL JOINs:</br>**
**(1) (INNER) JOIN:** Returns records that have matching values in both tables</br>
**(2) LEFT (OUTER) JOIN:** Returns all records from the left table, and the matched records from the right table</br>
**(3) RIGHT (OUTER) JOIN:** Returns all records from the right table, and the matched records from the left table</br>
**(4) FULL (OUTER) JOIN:** Returns all records when there is a match in either left or right table</br>

_QUERY:_
```python
SELECT * FROM Orders;
SELECT * FROM Customers;
SELECT Orders.OrderID,Customers.CustomerName,Orders.OrderDate
       FROM Orders
       INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;
```
_Output:_
![Screenshot from 2023-11-02 14-52-28](https://github.com/HoopedPJ/rdbms_2023batch/assets/144322043/cf15cf0d-7db6-47ab-b284-3a52103b8b9b)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## *5. Creating different types of Views for tailored presentation of data.*
