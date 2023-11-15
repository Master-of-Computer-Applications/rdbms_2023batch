# <p align="center">PRACTICAL FILE OF RDBMS</p>
## <p align="left"> Ques-1. Comparative study of various Database Management Systems.</p>
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

    

## <p align="left"> Ques-2. Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL). </p>
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



## <p align="left"> Ques-3. How to apply Constraints at various levels? </p>

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




![Screenshot from 2023-10-13 21-49-27](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/f2621d3b-20b0-41d2-bb98-68d4a5f7ae8a)
To add data to the tables, you can use the SQL INSERT INTO statement as well.

 python
-- Inserting sample data into the "courses" table
INSERT INTO courses (course_id, course_name)
VALUES
    (1, 'Introduction to Computer Science'),
    (2, 'Calculus I'),
    (3, 'Biology 101'),
    (4, 'History of Art'),
    (5, 'English Composition');

-- Inserting sample data into the "student" table
INSERT INTO student (student_id, first_name, last_name, date_of_birth, email, enrollment_date, major, GPA, course_enrolled)
VALUES
    (1, 'John', 'Doe', '1995-05-15', 'johndoe@example.com', '2023-09-01', 'Computer Science', 3.5, 1),
    (2, 'Jane', 'Smith', '1997-08-20', 'janesmith@example.com', '2023-09-01', 'Mathematics', 3.8, 2),
    (3, 'Alice', 'Johnson', '1998-03-10', 'alicejohnson@example.com', '2023-09-01', 'Biology', 3.2, 3);


![Screenshot from 2023-10-13 22-05-44](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/ad803f68-ce32-4286-aaf4-98f0122506fa)

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

#### *1.SQL Arithmetic Operators*
The Arithmetic Operators perform the mathematical operation on the numerical data of the SQL tables. These operators perform addition, subtraction, multiplication, and division operations on the numerical operands.

Following are the various arithmetic operators performed on the SQL data:
   - SQL Addition Operator (+)
   - SQL Subtraction Operator (-)
   - SQL Multiplication Operator (+)
   - SQL Division Operator (-)
   - SQL Modulus Operator (+)
    
#### *2.SQL Comparison Operators*

The Comparison Operators in SQL compare two different data of SQL table and check whether they are the same, greater, and lesser. The SQL comparison operators are used with the WHERE clause in the SQL queries

Following are the various comparison operators which are performed on the data stored in the SQL database tables:
    - SQL Equal Operator (=)
    - SQL Not Equal Operator (!=)
    - SQL Greater Than Operator (>)
    - SQL Greater Than Equals to Operator (>=)
    - SQL Less Than Operator (<)\
    - SQL Less Than Equals to Operator (<=)

#### *3.SQL Logical Operators*

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

#### *4.SQL Set Operators*

Set operators combine more than one select statement in a single query and return a specific result set.

Following are the various set operators which are performed on the similar data stored in the two SQL database tables:
    - SQL Union Operator
    - SQL Union ALL Operator
    - SQL Intersect Operator
    - SQL Minus Operator
    
#### *5.SQL Bitwise Operators*

The Bitwise Operators in SQL perform the bit operations on the Integer values. To understand the performance of Bitwise operators, you just knew the basics of Boolean algebra.

Following are the two important logical operators which are performed on the data stored in the SQL database tables:
    - Bitwise AND (&)
    - Bitwise OR(|)

#### *6.SQL Unary Operators*

The Unary Operators in SQL perform the unary operations on the single data of the SQL table, i.e., these operators operate only on one operand.

These types of operators can be easily operated on the numeric data value of the SQL table.

Following are the various unary operators which are performed on the numeric data stored in the SQL table:
    - SQL Unary Positive Operator
    - SQL Unary Negative Operator
    - SQL Unary Bitwise NOT Operator

 ### SQL FUNCTIONS
 For doing operations on data SQL has many built-in functions, they are categorized in two categories and further sub-categorized in different seven functions under each category. The categories are: 
   **Aggregate functions**
    These functions are used to do operations from the values of the column and a single value is returned. 
        - AVG()
        - COUNT()
        - FIRST()
        - LAST()
        - MAX()
        - MIN()
        - SUM()
    **Scalar functions:**
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

**Different Types of SQL JOINS**

Here are the different types of the JOINs in SQL:
    - *(INNER) JOIN*: Returns records that have matching values in both tables
    - *LEFT (OUTER) JOIN*: Returns all records from the left table, and the matched records from the right table
    - *RIGHT (OUTER) JOIN*: Returns all records from the right table, and the matched records from the left table
    - *FULL (OUTER) JOIN*: Returns all records when there is a match in either left or right table

    

Let's say you have two tables: employees and departments. The goal is to retrieve information about employees and their corresponding departments.

### Objective:
Retrieve a list of employee names, their department names, and display an indicator if their salary is above a certain threshold.

![Screenshot from 2023-11-11 17-46-39](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/94fadfd1-f6ad-4dbd-93fe-b25fadf9bd16)

### Explanation:

*SELECT Clause:*

CONCAT(first_name, ' ', last_name) AS full_name: Concatenates the first_name and last_name columns into a new column named full_name.
department_name: Selects the department_name from the departments table.
salary: Selects the salary from the employees table.
CASE WHEN salary > 55000 THEN 'Above Threshold' ELSE 'Below Threshold' END AS salary_indicator: Uses a CASE statement to create a new column salary_indicator that indicates whether the salary is above a certain threshold

*FROM Clause:*

FROM employees: Specifies the primary table as employees.
JOIN departments ON employees.department_id = departments.department_id: Performs an INNER JOIN with the departments table based on the department_id column to link the two tables.

*Result:*

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

#### *SYNTAX*

IF condition THEN
   
    -- code to execute if condition is true
END IF;


### IF ELSE IF STATEMENT
This statement is an extension of the IF statement and allows you to specify multiple conditions and corresponding blocks of code to execute.

#### *SYNTAX*

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

#### *SYNTAX*

CASE
WHEN condition1 THEN
        
        -- code to execute if condition1 is true
WHEN condition2 THEN
        
        -- code to execute if condition2 is true
ELSE
        
        -- code to execute if none of the conditions are true
END CASE;

![Screenshot from 2023-11-13 20-59-29](https://github.com/Gurleen0411/rdbms_2023batch/assets/144206226/1b1fdabd-75d0-49ac-890b-bcb50cd569f7)
