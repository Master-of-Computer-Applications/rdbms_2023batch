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

To apply constraints on a table named "student," you would typically use SQL statements. Here's an example of how you can create a "student" table with various constraints. Certainly, you can apply a foreign key constraint in the "student" table to establish a relationship with another table, such as a "courses" table. This relationship can represent the courses that each student is enrolled in. Here's an example of how to add a foreign key constraint to the "student" table:

``` python
CREATE TABLE courses (
    course_id INT PRIMARY KEY,
    course_name VARCHAR(100)
);

CREATE TABLE student (
    student_id INT PRIMARY KEY,
## <p align="left">Ques-4.View data in the required form using Operators, Functions and Joins.</p>

### SQL Operators
The SQL reserved words and characters are called operators, which are used with a WHERE clause in a SQL query. In SQL, an operator can either be a unary or binary operator. The unary operator uses only one operand for performing the unary operation, whereas the binary operator uses two operands for performing the binary operation.

#### Types of Operator

SQL operators are categorized in the following categories:

- SQL Arithmetic Operators

- SQL Comparison Operators

- SQL Logical Operators

- SQL Set Operators

- SQL Bit-wise Operators

- SQL Unary Operators

#### 1.SQL Arithmetic Operators
The Arithmetic Operators perform the mathematical operation on the numerical data of the SQL tables. These operators perform addition, subtraction, multiplication, and division operations on the numerical operands.

Following are the various arithmetic operators performed on the SQL data:
   - SQL Addition Operator (+)
   - SQL Subtraction Operator (-)
   - SQL Multiplication Operator (+)
   - SQL Division Operator (-)
   - SQL Modulus Operator (+)
    
#### 2.SQL Comparison Operators

The Comparison Operators in SQL compare two different data of SQL table and check whether they are the same, greater, and lesser. The SQL comparison operators are used with the WHERE clause in the SQL queries

Following are the various comparison operators which are performed on the data stored in the SQL database tables:
    - SQL Equal Operator (=)
    - SQL Not Equal Operator (!=)
    - SQL Greater Than Operator (>)
    - SQL Greater Than Equals to Operator (>=)
    - SQL Less Than Operator (<)\
    - SQL Less Than Equals to Operator (<=)

#### 3.SQL Logical Operators

The Logical Operators in SQL perform the Boolean operations, which give two results True and False. These operators provide True value if both operands match the logical condition.

Following are the various logical operators which are performed on the data stored in the SQL database tables:
    -SQL ALL operator
    - SQL AND operator
    - SQL OR operator
    - SQL BETWEEN operator
    - SQL IN operator
    - SQL NOT operator
    - SQL ANY operator
    - SQL LIKE operator
    
The Set Operators in SQL combine a similar type of data from two or more SQL database tables. It mixes the result, which is extracted from two or more SQL queries, into a single result.

#### 4.SQL Set Operators

Set operators combine more than one select statement in a single query and return a specific result set.

Following are the various set operators which are performed on the similar data stored in the two SQL database tables:
    - SQL Union Operator
    - SQL Union ALL Operator
    - SQL Intersect Operator
    - SQL Minus Operator
    
#### 5.SQL Bitwise Operators

The Bitwise Operators in SQL perform the bit operations on the Integer values. To understand the performance of Bitwise operators, you just knew the basics of Boolean algebra.

Following are the two important logical operators which are performed on the data stored in the SQL database tables:
    - Bitwise AND (&)
    - Bitwise OR(|)

#### 6.SQL Unary Operators

The Unary Operators in SQL perform the unary operations on the single data of the SQL table, i.e., these operators operate only on one operand.

These types of operators can be easily operated on the numeric data value of the SQL table.

Following are the various unary operators which are performed on the numeric data stored in the SQL table:
    - SQL Unary Positive Operator
    - SQL Unary Negative Operator
    - SQL Unary Bitwise NOT Operator

 ### SQL FUNCTIONS
 For doing operations on data SQL has many built-in functions, they are categorized in two categories and further sub-categorized in different seven functions under each category. The categories are: 
   *Aggregate functions*
    These functions are used to do operations from the values of the column and a single value is returned. 
        - AVG()
        - COUNT()
        - FIRST()
        - LAST()
        - MAX()
        - MIN()
        - SUM()
    *Scalar functions:*
    These functions are based on user input, these too returns single value. 
        - UCASE()
        - LCASE()
        - MID()
        - LEN()
        - ROUND()
        - NOW()
        - FORMAT()
  
### SQL JOIN

A JOIN clause is used to combine rows from two or more tables, based on a related column between them

*Different Types of SQL JOINS*

Here are the different types of the JOINs in SQL:
    - (INNER) JOIN: Returns records that have matching values in both tables
    - LEFT (OUTER) JOIN: Returns all records from the left table, and the matched records from the right table
    - RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table
    - FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table

    

Let's say you have two tables: employees and departments. The goal is to retrieve information about employees and their corresponding departments.

### Objective:
Retrieve a list of employee names, their department names, and display an indicator if their salary is above a certain threshold.


### Explanation:

SELECT Clause:

CONCAT(first_name, ' ', last_name) AS full_name: Concatenates the first_name and last_name columns into a new column named full_name.
department_name: Selects the department_name from the departments table.
salary: Selects the salary from the employees table.
CASE WHEN salary > 55000 THEN 'Above Threshold' ELSE 'Below Threshold' END AS salary_indicator: Uses a CASE statement to create a new column salary_indicator that indicates whether the salary is above a certain threshold

FROM Clause:

FROM employees: Specifies the primary table as employees.
JOIN departments ON employees.department_id = departments.department_id: Performs an INNER JOIN with the departments table based on the department_id column to link the two tables.

Result:

The query will return a result set with columns: full_name, department_name,salary, salary_indicator.

## <p align="left">Ques-5.Creating different types of Views for tailored presentation of data</p>

Views are a special version of tables in SQL. They provide a virtual table environment for various complex operations. You can select data from multiple tables, or you can select specific data based on certain criteria in views. It does not hold the actual data; it holds only the definition of the view in the data dictionary.
The view is a query stored in the data dictionary, on which the user can query just like they do on tables. It does not use the physical memory, only the query is stored in the data dictionary. It is computed dynamically, whenever the user performs any query on it. Changes made at any point in view are reflected in the actual base table.

### Simple View: 
A view based on only a single table, which doesn't contain GROUP BY clause and any functions.

### Complex View: 
A view based on multiple tables, which contain GROUP BY clause and functions.

### Inline View: 
A view based on a subquery in FROM Clause, that subquery creates a temporary table and simplifies the complex query.

### Materialized View: 
A view that stores the definition as well as data. It creates replicas of data by storing it physically.

![Screenshot from 2023-11-13 19-19-45](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/c8ddfadc-f585-4f21-8c5c-01420f6450d9)

![Screenshot from 2023-11-13 19-27-44](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/968cd387-837b-41cc-8fd0-9289b5a2bef3)


## <p align="left">Ques-6.How to apply Conditional Controls in PL/SQL</p>

In PL/SQL (Procedural Language/Structured Query Language), we can use conditional controls to execute different blocks of code based on certain conditions. There are several constructs for implementing conditional logic in PL/SQL, including the IF statement, CASE statement, and the IF-ELSIF-ELSE statement.

### IF STATEMENT
The IF statement is used to execute a block of code if a specified condition is true.

#### SYNTAX

IF condition THEN
   
    -- code to execute if condition is true
END IF;


### IF ELSE IF STATEMENT
This statement is an extension of the IF statement and allows you to specify multiple conditions and corresponding blocks of code to execute.

#### SYNTAX

IF 
condition1 
THEN
    
    -- code to execute if condition1 is true
ELSIF 
condition2 
THEN
    
    -- code to execute if condition2 is true
ELSE
     
     -- code to execute if none of the conditions are true
END IF;


### CASE STATEMENT 
The CASE statement is used to perform different actions based on the value of an expression.

#### SYNTAX

CASE
WHEN condition1 THEN
        
        -- code to execute if condition1 is true
WHEN condition2 THEN
        
        -- code to execute if condition2 is true
ELSE
        
        -- code to execute if none of the conditions are true
END CASE;

![Screenshot from 2023-11-13 20-59-29](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/1b1fdabd-75d0-49ac-890b-bcb50cd569f7)
11:03 pm
Thank you soo much🥹
11:15 pm
Bakie de jldi karke send kar die
11:15 pm
Plz
11:15 pm
TODAY
Bki sam mil ni rhe
8:10 am
Kive kra
8:10 am
😵‍💫
9:48 am
Ravneet ne kite nhi?
9:48 am
Kina hoya?
7:39 pm
?
7:48 pm
File da ta hogya
7:53 pm
7:56 pm
7:57 pm
7:58 pm
github.com
https://github.com/Master-of-Computer-Applications/rdbms_2023batch/pull/40
github.com
https://github.com/Master-of-Computer-Applications/rdbms_2023batch/pull/40
8:02 pm
github.com
https://github.com/samridhi0/rdbms_2023batch/edit/patch-3/2329018/RDBMS_file.md?pr=%2FMaster-of-Computer-Applications%2Frdbms_2023batch%2Fpull%2F40
github.com
https://github.com/samridhi0/rdbms_2023batch/edit/patch-3/2329018/RDBMS_file.md?pr=%2FMaster-of-Computer-Applications%2Frdbms_2023batch%2Fpull%2F40
8:08 pm



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
```
![Screenshot from 2023-10-16 11-22-05](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/2ad3cccf-66a7-4ae4-9527-475de9ad27bc)


To add data to the tables, you can use the SQL INSERT INTO statement as well.

``` python
-- Inserting sample data into the "courses" table
INSERT INTO courses (course_id, course_name)
VALUES
    (1, 'Introduction to Computer Science'),
    (2, 'Calculus I'),
    (3, 'Biology 101'),
    (4, 'History of Art'),
    (5, 'English Composition');
    
-- Inserting sample data into the "student" table
INSERT INTO student (student_id, first_name, last_name, date_of_birth, email, enrollment_date, major, new_gpa_column, course_enrolled)
VALUES
    (1, 'John', 'Doe', '1995-05-15', 'johndoe@example.com', '2023-09-01', 'Computer Science', 3.5, 1),
    (2, 'Jane', 'Smith', '1997-08-20', 'janesmith@example.com', '2023-09-01', 'Mathematics', 3.8, 2),
    (3, 'Alice', 'Johnson', '1998-03-10', 'alicejohnson@example.com', '2023-09-01', 'Biology', 3.2, 3);
```
![Screenshot from 2023-10-16 11-33-31](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/54b7a777-acc9-487e-8b50-6ae7fcdaf0e2)

## <p align="left">Ques-4.View data in the required form using Operators, Functions and Joins.</p>

### SQL Operators
The SQL reserved words and characters are called operators, which are used with a WHERE clause in a SQL query. In SQL, an operator can either be a unary or binary operator. The unary operator uses only one operand for performing the unary operation, whereas the binary operator uses two operands for performing the binary operation.

#### Types of Operator

SQL operators are categorized in the following categories:

- SQL Arithmetic Operators

- SQL Comparison Operators

- SQL Logical Operators

- SQL Set Operators

- SQL Bit-wise Operators

- SQL Unary Operators

#### 1.SQL Arithmetic Operators
The Arithmetic Operators perform the mathematical operation on the numerical data of the SQL tables. These operators perform addition, subtraction, multiplication, and division operations on the numerical operands.

Following are the various arithmetic operators performed on the SQL data:
   - SQL Addition Operator (+)
   - SQL Subtraction Operator (-)
   - SQL Multiplication Operator (+)
   - SQL Division Operator (-)
   - SQL Modulus Operator (+)
    
#### 2.SQL Comparison Operators

The Comparison Operators in SQL compare two different data of SQL table and check whether they are the same, greater, and lesser. The SQL comparison operators are used with the WHERE clause in the SQL queries

Following are the various comparison operators which are performed on the data stored in the SQL database tables:
    - SQL Equal Operator (=)
    - SQL Not Equal Operator (!=)
    - SQL Greater Than Operator (>)
    - SQL Greater Than Equals to Operator (>=)
    - SQL Less Than Operator (<)\
    - SQL Less Than Equals to Operator (<=)

#### 3.SQL Logical Operators

The Logical Operators in SQL perform the Boolean operations, which give two results True and False. These operators provide True value if both operands match the logical condition.

Following are the various logical operators which are performed on the data stored in the SQL database tables:
    -SQL ALL operator
    - SQL AND operator
    - SQL OR operator
    - SQL BETWEEN operator
    - SQL IN operator
    - SQL NOT operator
    - SQL ANY operator
    - SQL LIKE operator
    
The Set Operators in SQL combine a similar type of data from two or more SQL database tables. It mixes the result, which is extracted from two or more SQL queries, into a single result.

#### 4.SQL Set Operators

Set operators combine more than one select statement in a single query and return a specific result set.

Following are the various set operators which are performed on the similar data stored in the two SQL database tables:
    - SQL Union Operator
    - SQL Union ALL Operator
    - SQL Intersect Operator
    - SQL Minus Operator
    
#### 5.SQL Bitwise Operators

The Bitwise Operators in SQL perform the bit operations on the Integer values. To understand the performance of Bitwise operators, you just knew the basics of Boolean algebra.

Following are the two important logical operators which are performed on the data stored in the SQL database tables:
    - Bitwise AND (&)
    - Bitwise OR(|)

#### 6.SQL Unary Operators

The Unary Operators in SQL perform the unary operations on the single data of the SQL table, i.e., these operators operate only on one operand.

These types of operators can be easily operated on the numeric data value of the SQL table.

Following are the various unary operators which are performed on the numeric data stored in the SQL table:
    - SQL Unary Positive Operator
    - SQL Unary Negative Operator
    - SQL Unary Bitwise NOT Operator

 ### SQL FUNCTIONS
 For doing operations on data SQL has many built-in functions, they are categorized in two categories and further sub-categorized in different seven functions under each category. The categories are: 
   *Aggregate functions*
    These functions are used to do operations from the values of the column and a single value is returned. 
        - AVG()
        - COUNT()
        - FIRST()
        - LAST()
        - MAX()
        - MIN()
        - SUM()
    *Scalar functions:*
    These functions are based on user input, these too returns single value. 
        - UCASE()
        - LCASE()
        - MID()
        - LEN()
        - ROUND()
        - NOW()
        - FORMAT()
  
### SQL JOIN

A JOIN clause is used to combine rows from two or more tables, based on a related column between them

*Different Types of SQL JOINS*

Here are the different types of the JOINs in SQL:
    - (INNER) JOIN: Returns records that have matching values in both tables
    - LEFT (OUTER) JOIN: Returns all records from the left table, and the matched records from the right table
    - RIGHT (OUTER) JOIN: Returns all records from the right table, and the matched records from the left table
    - FULL (OUTER) JOIN: Returns all records when there is a match in either left or right table

    

Let's say you have two tables: employees and departments. The goal is to retrieve information about employees and their corresponding departments.

### Objective:
Retrieve a list of employee names, their department names, and display an indicator if their salary is above a certain threshold.
![sammridhi](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/508a1008-f322-4610-92d8-44eaf8270014)


### Explanation:

SELECT Clause:

CONCAT(first_name, ' ', last_name) AS full_name: Concatenates the first_name and last_name columns into a new column named full_name.
department_name: Selects the department_name from the departments table.
salary: Selects the salary from the employees table.
CASE WHEN salary > 55000 THEN 'Above Threshold' ELSE 'Below Threshold' END AS salary_indicator: Uses a CASE statement to create a new column salary_indicator that indicates whether the salary is above a certain threshold

FROM Clause:

FROM employees: Specifies the primary table as employees.
JOIN departments ON employees.department_id = departments.department_id: Performs an INNER JOIN with the departments table based on the department_id column to link the two tables.

Result:

The query will return a result set with columns: full_name, department_name,salary, salary_indicator.

## <p align="left">Ques-5.Creating different types of Views for tailored presentation of data</p>

Views are a special version of tables in SQL. They provide a virtual table environment for various complex operations. You can select data from multiple tables, or you can select specific data based on certain criteria in views. It does not hold the actual data; it holds only the definition of the view in the data dictionary.
The view is a query stored in the data dictionary, on which the user can query just like they do on tables. It does not use the physical memory, only the query is stored in the data dictionary. It is computed dynamically, whenever the user performs any query on it. Changes made at any point in view are reflected in the actual base table.

### Simple View: 
A view based on only a single table, which doesn't contain GROUP BY clause and any functions.

### Complex View: 
A view based on multiple tables, which contain GROUP BY clause and functions.

### Inline View: 
A view based on a subquery in FROM Clause, that subquery creates a temporary table and simplifies the complex query.![dell1](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/93240f6f-06db-4eaa-8704-328f22e9e8cd)


### Materialized View: 
A view that stores the definition as well as data. It creates replicas of data by storing it physically.

![samridhii](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/79e392ee-993f-43b8-8d7b-2d7ec77b65ad)


![samridhi](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/848e9d72-0d3e-4c75-9da1-cae701491ef2)



## <p align="left">Ques-6.How to apply Conditional Controls in PL/SQL</p>

In PL/SQL (Procedural Language/Structured Query Language), we can use conditional controls to execute different blocks of code based on certain conditions. There are several constructs for implementing conditional logic in PL/SQL, including the IF statement, CASE statement, and the IF-ELSIF-ELSE statement.

### IF STATEMENT
The IF statement is used to execute a block of code if a specified condition is true.

#### SYNTAX

IF condition THEN
   
    -- code to execute if condition is true
END IF;


### IF ELSE IF STATEMENT
This statement is an extension of the IF statement and allows you to specify multiple conditions and corresponding blocks of code to execute.

#### SYNTAX

IF 
condition1 
THEN
    
    -- code to execute if condition1 is true
ELSIF 
condition2 
THEN
    
    -- code to execute if condition2 is true
ELSE
     
     -- code to execute if none of the conditions are true
END IF;


### CASE STATEMENT 
The CASE statement is used to perform different actions based on the value of an expression.

#### SYNTAX

CASE
WHEN condition1 THEN
        
        -- code to execute if condition1 is true
WHEN condition2 THEN
        
        -- code to execute if condition2 is true
ELSE
        
        -- code to execute if none of the conditions are true
END CASE;


![samridhi@samridhi](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/d78208ac-ab8e-4ab0-97b6-6c149fc1cb92)
## <p align="left">Ques-7. Error Handling using Internal Exceptions and External Exceptions


An exception occurs when the PL/SQL engine encounters an instruction which it cannot execute due to an error that occurs at run-time. These errors will not be captured at the time of compilation and hence these needed to handle only at the run-time.

For example, if PL/SQL engine receives an instruction to divide any number by ‘0’, then the PL/SQL engine will throw it as an exception. The exception is only raised at the run-time by the PL/SQL engine.

Exceptions will stop the program from executing further, so to avoid such condition, they need to be captured and handled separately. This process is called as Exception-Handling, in which the programmer handles the exception that can occur at the run time.
Exception-Handling Syntax

Exceptions are handled at the block, level, i.e., once if any exception occurs in any block then the control will come out of execution part of that block. The exception will then be handled at the exception handling part of that block. After handling the exception, it is not possible to resend control back to the execution section of that block.

### Internal Exceptions:

Internal exceptions are errors that are raised automatically by the database engine in response to certain conditions. These exceptions are predefined and cover a range of common error scenarios. Some common internal exceptions include:

1. NO_DATA_FOUND: Raised when a SELECT INTO statement returns no rows.
2. TOO_MANY_ROWS: Raised when a SELECT INTO statement returns more than one row.
3. ZERO_DIVIDE: Raised when attempting to divide by zero.
4. DUP_VAL_ON_INDEX: Raised when trying to insert a duplicate value into a unique index.
5. OTHERS: A catch-all exception that handles any unhandled exception.

*Syntax*
     
     BEGIN TRY
   
    -- Your T-SQL statements here
   
    
    -- This is the main block where potential errors may occur

    -- Example: Divide by zero error
    DECLARE @Result INT;
    SET @Result = 1 / 0; -- This will cause a divide by zero error

     END TRY
    BEGIN CATCH
    -- This block will be executed if an error occurs in the TRY block

    PRINT 'An error occurred: ' + ERROR_MESSAGE(); -- Print the error message
    -- You can log the error, roll back transactions, or take other appropriate actions

    END CATCH;

Here is an example of using internal exceptions:

    DECLARE
    v_result NUMBER;
    BEGIN
    SELECT 10 / 0 INTO v_result FROM dual;
    EXCEPTION
    WHEN ZERO_DIVIDE THEN
      DBMS_OUTPUT.PUT_LINE('Error: Division by zero');
    WHEN OTHERS THEN
      DBMS_OUTPUT.PUT_LINE('An unexpected error occurred');
    END;

Here are some possible internal exceptions:
|Exception Name|	Description|	Scenario When Exception is Thrown|
|-----|-----|------|
ER_SCALAR_BUILTIN_NO_ROWS_CODE	|The Scalar function did not return any value.|	This exception is thrown when a SCALAR function does not return any row (value).
ER_BAD_FIELD_ERROR	|Column name does not exist.|	A column that does not exist in a table is referenced in a query.
ER_TABLE_EXISTS_ERROR|	Table already exists.	|While creating a table, a table with the same name already exists.
ER_BAD_TABLE_ERROR	|Table does not exist.	|A table that does not exist is referenced in a query.
ER_NO_SUCH_TABLE|	Table does not exist.|	A table that does not exist is referenced in a query.
ER_DUP_ENTRY_WITH_KEY_NAME|	Duplicate key error.| The error message contains the key name as well.	A duplicate value is entered for a column with a key constraint.
ER_WRONG_VALUE_COUNT_ON_ROW|	Column count does not match value count.	|The number of columns in a table and the number of values specified in the query are not the same. For example, INSERT query.
ER_PARSE_ERROR|	Issue with parsing dynamic SQL.|	There is an error in the SQL statement.
ER_FILE_NOT_FOUND|	Cannot find file, usually in LOAD DATA statements.|	Either the file does not exist or the file path is incorrect.    

### External Exceptions:

External exceptions, also known as user-defined exceptions, are custom exceptions that developers can define to handle specific errors in their code. These exceptions are raised explicitly using the RAISE statement. Developers can define their own error codes and messages for better error handling.

1. Declaration of User-Defined Exception:
- To declare a user-defined exception, you use the DECLARE section of a PL/SQL block.
- Syntax: DECLARE my_exception EXCEPTION;

2. Raising User-Defined Exception:

- You can raise the user-defined exception explicitly using the RAISE statement.
- Syntax: RAISE my_exception;

3. Handling User-Defined Exception:

- In the EXCEPTION section of your PL/SQL block, you can specify handlers for specific exceptions, including user-defined exceptions.

*Syntax:*

    EXCEPTION
    WHEN my_exception THEN
      -- Handle the exception here


Here's an example of using external exceptions:

    DECLARE
    my_exception EXCEPTION;
    v_number NUMBER := 5;
    BEGIN
    IF v_number > 10 THEN
      RAISE my_exception;
    END IF;
    EXCEPTION
    WHEN my_exception THEN
      DBMS_OUTPUT.PUT_LINE('Custom exception: Number is greater than 10');
    WHEN OTHERS THEN
      DBMS_OUTPUT.PUT_LINE('An unexpected error occurred');
    END;
    

## <p align="left">Ques-8. Using various types of Cursors 

In SQL, a cursor is a database object that allows you to interact with individual rows returned by a query. Cursors are often used when you need to process one row at a time, rather than fetching the entire result set at once. There are several types of cursors in SQL, and their usage depends on the specific requirements of your application. The main types of cursors are:

#### 1. Static Cursor: 
- A static cursor is not sensitive to changes made by other users to the data while the cursor is open.
- It fetches a snapshot of the data at the time the cursor is opened.

*Syntax:*

    DECLARE cursor_name CURSOR STATIC FOR
    SELECT column1, column2, ...
    FROM your_table;

*Example:*
   
    DECLARE static_cursor CURSOR STATIC FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;    

#### 2. Dynamic Cursor:
- A dynamic cursor reflects changes made by other users to the data while the cursor is open.
- It does not fetch a snapshot but rather retrieves the current data each time a fetch is made.
    
*Syntax:*

    DECLARE cursor_name CURSOR DYNAMIC FOR
    SELECT column1, column2, ...
    FROM your_table;

*Example:*

    DECLARE dynamic_cursor CURSOR DYNAMIC FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;

#### 3. Forward-Only Cursor:
- A forward-only cursor only allows fetching rows in a forward direction (from the first to the last row).
- It is the most lightweight and performs better in terms of resource usage.

*Syntax:*

    DECLARE cursor_name CURSOR FORWARD_ONLY FOR
    SELECT column1, column2, ...
    FROM your_table;

*Example:*
   
    DECLARE forward_only_cursor CURSOR FORWARD_ONLY FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;

#### 4. Scroll Cursor:
- A scroll cursor allows fetching rows in both forward and backward directions.
- It provides more flexibility but may be less efficient than forward-only cursors.

*Syntax:*

      DECLARE cursor_name CURSOR SCROLL FOR
      SELECT column1, column2, ...
      FROM your_table;

*Example:*

    DECLARE scroll_cursor CURSOR SCROLL FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;

  
#### 5. Keyset Cursor:
- A keyset cursor is similar to a dynamic cursor but is more optimized as it only retrieves the key values of the rows.
- It is sensitive to changes in the data but doesn't retrieve the actual data until a fetch is made.

*Syntax:*

    DECLARE cursor_name CURSOR KEYSET FOR
    SELECT column1, column2, ...
    FROM your_table;

*Example:*

    DECLARE keyset_cursor CURSOR KEYSET FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;


#### 6. Insensitive Cursor:
- An insensitive cursor creates a temporary copy of the result set, making it insensitive to changes in the underlying data.
- It is typically used when the data should remain static throughout the cursor's lifetime.

*Syntax:*

    DECLARE cursor_name CURSOR INSENSITIVE FOR
    SELECT column1, column2, ...
    FROM your_table;

*Example:*

    DECLARE insensitive_cursor CURSOR INSENSITIVE FOR
    SELECT employee_id, first_name, last_name, salary
    FROM employees;

After declaring a cursor, you can use the following template to open, fetch, and close the cursor:

    OPEN cursor_name;
    FETCH NEXT FROM cursor_name INTO @variable1, @variable2, ...;
    -- Process the fetched data here
    CLOSE cursor_name;

Here's an example of using a cursor to fetch and print employee names:

    DECLARE employee_cursor CURSOR FOR
    SELECT first_name, last_name
    FROM employees;

    OPEN employee_cursor;

    FETCH NEXT FROM employee_cursor INTO @first_name, @last_name;

    WHILE @@FETCH_STATUS = 0
    BEGIN
    PRINT 'Employee Name: ' + @first_name + ' ' + @last_name;
    FETCH NEXT FROM employee_cursor INTO @first_name, @last_name;
    END

    CLOSE employee_cursor;


## <p align="left">Ques-9. How to run Stored Procedures and Functions

Stored Procedures and Functions are database objects in SQL that contain a set of precompiled SQL statements. They are designed to perform specific tasks and can be reused, making database development more efficient. Both stored procedures and functions enhance code modularity, improve security, and allow for better performance optimization.

### Stored Procedures:

*1. Purpose:*
- Procedural Logic: Stored procedures contain a series of SQL statements and procedural logic, allowing for complex operations to be encapsulated in a single unit.

*2. Execution:*
-  Call Statement: Stored procedures are typically executed using a CALL or EXEC statement.

*3. Parameters:*
- Input/Output Parameters: Stored procedures can take input parameters, perform operations, and return results. They may also have output parameters.

*4. Transaction Control:*
- Transaction Management: Stored procedures can include transaction management commands (COMMIT and ROLLBACK) to control the scope of transactions.

*Running Stored Procedures:*

1. Creating a Stored Procedure:
- Before you can run a stored procedure, you need to create it. Use the CREATE PROCEDURE statement to define a stored procedure.

       CREATE PROCEDURE procedure_name
       AS
       BEGIN
       -- SQL statements for the procedure
       END;

2. Executing a Stored Procedure:
- Once the stored procedure is created, you can execute it using the EXEC or EXECUTE statement.

       EXEC procedure_name;
       -- or
       EXECUTE procedure_name;

*Example:*

    -- Creating a stored procedure
    CREATE PROCEDURE GetEmployeeCount
    AS
    BEGIN
    -- Select the total number of employees from the Employees table
    SELECT COUNT(*) AS EmployeeCount
    FROM Employees;
    END;
    GO

    -- Running the stored procedure
    EXEC GetEmployeeCount;

*Using delimiters*

![screenshoot](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/5061d529-0277-43eb-b19b-e392c3e9c026)


### Functions:

*1. Purpose:*
- Return Value: Functions are designed to return a single value or a table result, making them suitable for use in expressions or queries.

*2. Execution:*
- Select Statement: Functions are typically used within SELECT statements or as part of an expression.

*3. Parameters:*
- Input Parameters: Functions may accept input parameters, but they cannot have output parameters.

*4. Transaction Control:*
- No Transaction Management: Functions cannot contain transaction management commands like COMMIT or ROLLBACK.

*Running Functions:*

1. Creating a Function:
- Use the CREATE FUNCTION statement to define a function. Functions return a value and can be used in SQL queries.

       CREATE FUNCTION function_name
       RETURNS data_type
       AS
       BEGIN
       -- SQL statements for the function
       RETURN value;
       END;

2. Executing a Function:
- Functions are typically used within queries or other SQL statements.

       SELECT function_name(parameters);

*Example:*

    -- Creating a function
    CREATE FUNCTION GetAverageSalary()
    RETURNS DECIMAL(10, 2)
    AS
    BEGIN
    DECLARE @AvgSalary DECIMAL(10, 2);
    -- Calculate the average salary from the Employees table
    SELECT @AvgSalary = AVG(Salary)
    FROM Employees;
    RETURN @AvgSalary;
    END;
    GO

    -- Running the function in a SELECT statement
    SELECT dbo.GetAverageSalary() AS AvgSalary;

*Using delimiters*
![screenshot](https://github.com/samridhi0/rdbms_2023batch/assets/114128927/72da30d1-49ac-4c94-a7c0-8d41265d0099)



## <p align="left">Ques-10. Creating Packages and applying Triggers

### Creating Packages in PL/SQL:

A PL/SQL package is a collection of related procedures, functions, variables, and other constructs that are grouped together for modularity and reusability. Packages consist of two parts: the package specification and the package body.

*1. Package Specification:*
- Declares the public interface of the package.
- Contains declarations of procedures, functions, variables, types, and constants that are accessible from outside the package.
- Does not contain the implementation details.

*Syntax*

    CREATE OR REPLACE PACKAGE Your_Package_Name AS
    PROCEDURE Procedure_Name;
    FUNCTION Function_Name RETURN NUMBER;
    -- Declare variables, types, etc.
    END Your_Package_Name;
    /

*2. Package Body:*
- Implements the procedures and functions declared in the package specification.
- Contains the actual code for the functionality provided by the package.
- May include private variables and procedures that are not accessible outside the package.

*Syntax*

    CREATE OR REPLACE PACKAGE BODY Your_Package_Name AS
    PROCEDURE Procedure_Name IS
    BEGIN
    -- Procedure logic here
    NULL;
    END;

    FUNCTION Function_Name RETURN NUMBER IS
    BEGIN
    -- Function logic here
    RETURN 0;
    END;
    END Your_Package_Name;
    /
    
### Applying Triggers in PL/SQL:

A PL/SQL trigger is a set of instructions that are automatically executed in response to certain events on a table, such as an INSERT, UPDATE, or DELETE operation.

*1. Creating a Trigger:*
- Defines the trigger name, event (e.g., BEFORE INSERT, AFTER UPDATE), and the table on which the trigger should act.
- Contains the PL/SQL block with the logic to be executed when the trigger is fired.

*Syntax*

    CREATE OR REPLACE TRIGGER Your_Trigger_Name
    BEFORE INSERT ON Your_Table_Name
    FOR EACH ROW
    BEGIN
    Your_Package_Name.Procedure_Name;
    -- Your trigger logic here
    END Your_Trigger_Name;
    /

In this example, the trigger is set to execute before an INSERT operation on Your_Table_Name. The trigger calls the Procedure_Name from Your_Package_Name.

*2. Applying the Trigger:*
- Once the trigger is created, it needs to be associated with a specific table.

*Syntax* 

    ALTER TABLE Your_Table_Name
    ENABLE TRIGGER Your_Trigger_Name;

- This associates the trigger Your_Trigger_Name with the table Your_Table_Name.

*3. Testing the Trigger:*
- You can test the trigger by performing operations on the table that the trigger is associated with.

*Syntax*

    INSERT INTO Your_Table_Name (column1, column2, ...)
    VALUES (value1, value2, ...);

- The trigger will execute its logic before or after the specified event on the table.


## <p align="left">Ques-11. Creating Arrays and Nested Table

### Arrays (Associative Arrays) in PL/SQL:

*1. Declaration:*
- Declare an associative array using the TYPE statement. Specify the data type of the elements and the index type.

*Syntax*

      DECLARE
      TYPE my_array_type IS TABLE OF VARCHAR2(50) INDEX BY PLS_INTEGER;
      my_array my_array_type;

- In this example, my_array_type is a type definition for an associative array that stores strings, and the index is of type PLS_INTEGER.

*2. Initialization:*
- Initialize the array in the DECLARE section or later in the executable section.

*Syntax*

    BEGIN
    my_array(1) := 'First';
    my_array(2) := 'Second';
    my_array(3) := 'Third';
    END;
    
- You can also use the BULK COLLECT feature to initialize the array from a query result.

*Syntax*

    SELECT column_name BULK COLLECT INTO my_array FROM my_table;

*3. Accessing Elements:*
Access elements by their index.

*Syntax*

    DBMS_OUTPUT.PUT_LINE(my_array(2)); -- Prints 'Second'

*4. Dynamic Sizing:*

Associative arrays are dynamic, and you can add elements without specifying the size beforehand.

*Example*

    DECLARE
    -- Declare an associative array type
    TYPE my_array_type IS TABLE OF VARCHAR2(50) INDEX BY PLS_INTEGER;
   
    -- Declare an instance of the array
    my_array my_array_type;
    BEGIN
    -- Initialize the array
    my_array(1) := 'Apple';
    my_array(2) := 'Banana';
    my_array(3) := 'Orange';

    -- Access and print elements
    DBMS_OUTPUT.PUT_LINE('Fruit at index 2: ' || my_array(2)); -- Prints 'Banana'
   
    -- Add a new element dynamically
    my_array(4) := 'Grapes';
   
    -- Access and print the new element
    DBMS_OUTPUT.PUT_LINE('Fruit at index 4: ' || my_array(4)); -- Prints 'Grapes'
    END;
    /


### Nested Tables in PL/SQL:

*1. Declaration:*
- Declare a nested table using the TYPE statement. Specify the data type of the elements.

*Syntax*

      DECLARE
      TYPE nested_table_type IS TABLE OF VARCHAR2(50);
      TYPE my_nested_table_type IS TABLE OF nested_table_type;
      my_nested_table my_nested_table_type;

 - my_nested_table_type is a type definition for a nested table that stores strings.

*2. Initialization:*
- Initialize the nested table similarly to a one-dimensional array.

*Syntax*

    BEGIN
      my_nested_table := my_nested_table_type(
                           nested_table_type('One', 'Two', 'Three'),
                           nested_table_type('Four', 'Five', 'Six'),
                           nested_table_type('Seven', 'Eight', 'Nine')
                       );
    END;

*3. Accessing Elements:*
Access elements using multiple indices.

*Syntax*

        DBMS_OUTPUT.PUT_LINE(my_nested_table(2)(3)); -- Prints 'Six'

*4. Dynamic Sizing:*
Like associative arrays, nested tables are dynamic, and you can add elements without specifying the size beforehand.

*Using Nested Tables in SQL:*
- You can also use nested tables directly in SQL operations.

*Syntax*

    SELECT * FROM TABLE(my_nested_table);

- Manipulate nested tables using SQL functions like MULTISET and CAST.

*Example*

    DECLARE
    -- Declare a nested table type
    TYPE nested_table_type IS TABLE OF VARCHAR2(50);
    TYPE my_nested_table_type IS TABLE OF nested_table_type;
   
    -- Declare an instance of the nested table
    my_nested_table my_nested_table_type;
    BEGIN
    -- Initialize the nested table
    my_nested_table := my_nested_table_type(
                        nested_table_type('John', 'Doe'),
                        nested_table_type('Jane', 'Smith'),
                        nested_table_type('Bob', 'Johnson')
                    );

    -- Access and print an element
    DBMS_OUTPUT.PUT_LINE('Last name of person at index 2: ' || my_nested_table(2)(2)); -- Prints 'Smith'

    -- Add a new element dynamically
    my_nested_table.extend;
    my_nested_table(my_nested_table.last) := nested_table_type('Alice', 'Williams');

    -- Access and print the new element
    DBMS_OUTPUT.PUT_LINE('First name of person at index 4: ' || my_nested_table(4)(1)); -- Prints 'Alice'
    END;
    /




