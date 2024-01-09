# <p align="center">PRACTICAL FILE OF RDMBS</p>

## <p align="left"> Ques-1. Comparative study of various Database Management Systems</p>
A Database Management System (DBMS) is a software application or system that facilitates the creation, organization, storage, retrieval, and management of data in a structured and efficient manner. It serves as an intermediary between users or applications and the underlying database, providing tools and functionalities for data storage, access, security, and data integrity. DBMS systems are essential for effectively managing and manipulating data in various domains, including business, research, and software development.

There are numerous Database Management Systems (DBMS) available, each with its own features and strengths. Here are some of the well-known DBMS:

### Relational Database Management Systems (RDBMS):
1. MySQL
2. PostgreSQL
3. Oracle Database
4. Microsoft SQL Server
5. SQLite
6. Maria DB
7. IBM Db2

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

---

## <p align="left"> Ques-2. Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL) </p>
### DDL (Data Definition Language):
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
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.| Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT

---

## <p align="left"> Ques-3. How to apply Constraints at various levels. </p>

Constraints in the context of a relational database management system (RDBMS) are rules and conditions that are applied to the data in a database to ensure data integrity, accuracy, and consistency. They define the limitations and requirements for the data stored in database tables, helping to maintain the quality and reliability of the data. Constraints can be applied at various levels in a database, such as table level, column level, and database level. 

Some common types of constraints include:

### **Primary Key Constraint:**
Ensures that a column or a set of columns contains unique values, and no two rows can have the same values in the primary key column(s). It uniquely identifies each row in a table.
### **Unique Key**
Ensures that the values in a column or a set of columns are unique, but it doesn't necessarily require the uniqueness to identify each row. Multiple rows can have the same value as long as it's unique within the specified column(s).
### **Check Constraint**
Defines a condition or expression that must be true for data to be inserted or updated in a column. It allows you to enforce specific business rules or data validation.
### **Foreign Key**
Maintains referential integrity by linking a column in one table to the primary key of another table. This ensures that values in the foreign key column exist in the referenced table's primary key column.
### **Not Null**
Requires that a column cannot have a null (empty) value. It enforces the presence of data in the specified column.
### **Check Constraint**
Defines a condition that must be satisfied for data to be valid in a column. For example, you can use this constraint to enforce minimum or maximum values, data formats, or any custom business rules.

To apply constraints on a table named "student," you would typically use SQL statements. Here's an example of how you can create a "student" table with various constraints. Certainly, you can apply a foreign key constraint in the "student" table to establish a relationship with another table, such as a "courses" table. This relationship can represent the courses that each student is enrolled in. Here's an example of how to add a foreign key constraint to the "student" table:

``` python
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
```
![Screenshot from 2023-10-12 23-38-46](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/76064e56-dc30-4956-8e9d-60daf1240e3d)

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
![Screenshot from 2023-10-13 00-01-38](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/373107a5-2811-45ca-94fc-2321357a13d5)
![Screenshot from 2023-10-13 00-34-13](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/3039663b-3ff9-40db-b967-36bd7e0b985c)

---

## <p align="left"> Ques-4. View data in the required form using Operators, Functions and Joins. </p>
Structured Query Language is a computer language that we use to interact with a relational database. 

## SQL Operators
In simple operator can be defined as an entity used to perform operations in a table.

Operators are the foundation of any programming language. We can define operators as symbols that help us to perform specific mathematical and logical computations on operands. In other words, we can say that an operator operates the operands. SQL operators have three different categories.

### Types of SQL Operators:
1. Arithmetic Operators
2. Comparsion Operators
3. Logical Operators

### 1. Arithmetic Operators
We can use various arithmetic operators on the data stored in the tables. Arithmetic Operators are:

| Operator  | Description                                                                                         |
|-----------| -----------                                                                                         |
| +         | The addition is used to perform an addition operation on the data values.                           |
| _         | This operator is used for the subtraction of the data values.                                       | 
| /         | This operator works with the ‘ALL’ keyword and it calculates division operations.                   |
| *         | This operator is used for multiplying data values.This operator is used for multiplying data values.| 
| %         | Modulus is used to get the remainder when data is divided by another.                               | 

**Examples-**
![Screenshot from 2023-11-14 21-02-03](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/a5f2731e-d1b2-4004-936b-c8a7957f206c)
![Screenshot from 2023-11-14 21-02-29](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/5d126455-0264-4dbf-868b-1127772aee8a)
**Query-** SELECT * FROM student WHERE first_name LIKE 'J%';
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/a02f5ef0-6bab-401e-b30d-607e2bf9168e)

### 2. Comparsion Operators
Another important operator in SQL is a comparison operator, which is used to compare one expression’s value to other expressions. SQL supports different types of comparison operator, which is described below:

| Operator  | Description                                                                                                                       |
|-----------| -----------                                                                                                                       |
| =         | It checks if two operands values are equal or not, if the values are equal then condition becomes true.                           |
| >         | It checks if the left operand value is greater than right operand value, if yes then condition becomes true.                      | 
| <         | It checks if the left operand value is less than right operand value, if yes then condition becomes true.                         |
| >=        | It checks if the left operand value is less than or equal to the right operand value, if yes then condition becomes true.         | 
| <=        | It checks if the left operand value is less than or equal to the right operand value, if yes then condition becomes true.         | 
| <>        | It checks if two operands values are equal or not, if values are not equal then condition becomes true.                           | 
| !=        | It checks if two operands values are equal or not, if values are not equal then condition becomes true.                           | 

**Examples-**
![comparison op1](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/0393e9c4-e9a5-44d4-9858-d15ece75bc5b)
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/d4d52ecf-b7c8-42c6-b2c7-4557aa3f2f8d)

### 3. Logical Operators
There is the list of logical operator used in SQL:

| Operator  | Description                                                   |
|-----------| -----------                                                   |
| AND       | TRUE if all the conditions separated by AND is TRUE.          |
| OR        | TRUE if any of the conditions separated by OR is TRUE.        | 
| NOT       | Displays a record if the condition(s) is NOT TRUE             |
| LIKE      | TRUE if the operand matches a pattern                         | 
| BETWEEN   | TRUE if the operand is within the range of comparisons        |
| ALL       | TRUE if all of the subquery values meet the condition         | 
| ANY       | TRUE if any of the subquery values meet the condition         | 
 
**Examples-**
![logical op1](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/88bab023-e324-4512-816e-d41f8aad0205)
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/feb95493-d0fe-4f4b-8393-2e28847cbf80)

## SQL Functions
SQL functions are predefined operations that perform a specific action or computation on the data. Here are some common types of SQL functions:

### 1. Aggregate Functions:
Aggregate functions are used to perform calculations on a set of values and return a single result. Some of the most commonly used aggregate functions in SQL include −

- **COUNT():** Counts the number of rows in a result set.
- **SUM():** Calculates the sum of values in a numeric column.
- **AVG():** Computes the average of values in a numeric column.
- **MIN():** Finds the minimum value in a column.
- **MAX():** Finds the maximum value in a column.

### 2. Scalar Functions:
Scalar functions are used to perform calculations on a single value and return a single result. Some examples of scalar functions in SQL include −

- **UPPER(), LOWER():** Convert text to uppercase or lowercase.
- **CONCAT():** Concatenates two or more strings.
- **SUBSTRING():** Extracts a substring from a string.
- **ROUND(), CEIL(), FLOOR():** Rounds a numeric value.

### 3. Date and Time Functions:
SQL also provides a number of functions for working with date and time values. Some examples of date and time functions in SQL include −

- **NOW():** Retrieve the current date and time.
- **CURRENT_DATE, CURRENT_TIME:** Returns the current date and time.
- **YEAR(), MONTH(), DAY():** Extract parts of a date.

### 4. Mathematical Functions:

- **ABS():** Returns the absolute value of a numeric expression.
- **SQRT():** Calculates the square root of a numeric expression.
- **POWER():** Raises a numeric expression to the power of another.

**Examples:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/836660f5-412b-4931-b7b6-3bb595c43515)

## SQL Joins
The SQL Join clause is used to combine data from two or more tables in a database. When the related data is stored across multiple tables, joins help you to retrieve records combining the fields from these tables using their foreign keys.

Consider the two tables (courses and student) below as follows: 
![joins](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/71450d50-2951-489a-a731-519e2fb4a30a)
 
### Types of SQL Joins

SQL provides various types of Joins that are categorized based on the way data across multiple tables are joined together. They are listed as follows −

### 1. Inner Join

An INNER JOIN is the default join which retrieves the intersection of two tables. It compares each row of the first table with each row of the second table. If the pairs of these rows satisfy the join-predicate, they are joined together.

**Syntax:**

```python
SELECT table1.column1,table1.column2,table2.column1,....
FROM table1 
INNER JOIN table2
ON table1.matching_column = table2.matching_column;


table1: First table.
table2: Second table
matching_column: Column common to both the tables.
``` 

![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/65111c75-4126-4132-9fa1-190923d60343)

### 2. Outer Join
An Outer Join retrieves all the records in two tables even if there is no counterpart row of one table in another table, unlike Inner Join. Outer join is further divided into three subtypes - Left Join, Right Join and Full Join.

Following are the different types of outer Joins −

- **LEFT JOIN:** returns all rows from the left table, even if there are no matches in the right table.
- **RIGHT JOIN:** returns all rows from the right table, even if there are no matches in the left table.
- **FULL JOIN:** returns rows when there is a match in one of the tables.

![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/6254e318-e9f3-4e5c-a36a-bdfea1685a31)

### 3. Other Joins
In addition to these there are two more joins −

- **SELF Join:** is used to join a table to itself as if the table were two tables, temporarily renaming at least one table in the SQL statement.
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/378fef38-736c-4359-bb86-5e0ef0955cfe)

- **CROSS Join:** returns the Cartesian product of the sets of records from the two or more joined tables.
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/fbb128e9-1273-4ab8-acb1-3abd96c2c9bc)

---

## <p align="left"> Ques-5. Creating different types of Views for tailored presentation of data. </p>
Views in SQL are kind of virtual tables. A view also has rows and columns as they are in a real table in the database. We can create a view by selecting fields from one or more tables present in the database. A View can either have all the rows of a table or specific rows based on certain condition. In this article we will learn about creating , deleting and updating Views. 

**CREATE VIEW Syntax:** 
```python
CREATE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition; 
```
**CREATE OR REPLACE VIEW Syntax:**
```python
CREATE OR REPLACE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition; 
```
**DROP VIEW Syntax:**
```python
DROP VIEW view_name;
```
### Types of Views
**1. Simple View:** A view based on only a single table, which doesn't contain GROUP BY clause and any functions. simple view in SQL is a virtual table based on the result of a SELECT query from one table. Here's an example of creating a simple view:

**Example:** 
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/f9a4ac7f-d3ca-498e-8478-854065329d68)

**2. Complex View:** A view based on multiple tables, which contain GROUP BY clause and functions. A complex view in SQL involves multiple tables, joins, and potentially other SQL operations. Here's an example of creating a complex view that involves a join between two tables:

**Example:** 
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/bdc20bcd-ac6e-4f89-8216-f44d336ca9a7)

**3. Inline  View:** A view based on a subquery in FROM Clause, that subquery creates a temporary table and simplifies the complex query. An inline view, also known as a derived table or subquery in the FROM clause, is a construct in SQL where you use a SELECT statement to create a temporary set of data within the context of a larger query. Inline views are often used to simplify complex queries or to perform operations on a subset of data before joining it with other tables or performing further operations.

**Example:** 
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/3c96844f-cc4d-4994-b66b-5959bc88ab3d)

**4. Materialized View:** A view that stores the definition as well as data. It creates replicas of data by storing it physically. A materialized view in SQL is a database object that contains the results of a query, which is stored on disk as a physical table. Unlike a regular (non-materialized) view, a materialized view is precomputed and stored, which can improve query performance in certain scenarios.Materialized view replicates the retrieved data physically. This replicated data can be reused without executing the view again. This type of view is also known as "SNAPSHOTS". Materialized view reduce the processing time to regenerate the whole data. It helps remote users to replicate data locally and improve query performance. The challenging part here is to synchronize the changes in materialized views underlying tables.

---

## <p align="left"> Ques-6. How to apply Conditional Controls in PL/SQL. </p>
<p>PL/SQL (Procedural Language/Structured Query Language) is a programming language designed specifically for interacting with Oracle Database. It is a procedural language extension to SQL and provides a way to execute SQL statements seamlessly within its procedural constructs. PL/SQL is used to create stored procedures, functions, triggers, packages, and more, allowing you to write powerful and efficient database-centric applications.</p>
Decision making statements are those statements which are in charge of executing a statement out of multiple given statements based on some condition. The condition will return either true or false. Based on what the condition returns, the associated statement is executed.

This can be logically implemented in PL/SQL block using decision making statements. In PL/SQL, you can use conditional controls to execute different blocks of code based on specified conditions. The primary conditional control structures in PL/SQL are:

### 1. IF Statement:
The if statement, or the if...then statement can be used when there is only a single condition to be tested. If the result of the condition is TRUE then certain specified action will be performed otherwise if it is FALSE then no action is taken and the control of program will just move out of the if code block.

**Syntax:** 
```python
if <test_condition> then
	body of action
end if;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/6e24dbec-878c-42c0-8724-e65cd911687d)

### 2. IF-THEN-ELSE Statement:
The IF-THEN-ELSE statement extends the IF statement by providing an alternative block of code to execute when the condition is not true.
Using this statement group we can specify two statements or two set of statements, dependent on a condition such that when the condition is true then one set of statements is executed and if the condition is false then the other set of statements is executed. 

**Syntax:** 
```python
if <test_condition> then
	statement 1/set of statements 1
else
	statement 2/set of statements 2
end if;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/4fbe436b-c234-44d9-b255-1d300b8e913b)

### 3. ELSIF Clause:
You can use the ELSIF clause in an IF statement to check multiple conditions sequentially. It is used to check multiple conditions. Sometimes it is required to test more than one condition in that case if...then...else statement cannot be used. For this purpose, ELSIF Clause is suitable in which all the conditions are tested one by one and whichever condition is found to be TRUE, that block of code is executed. And if all the conditions result in FALSE then the else part is executed.

**Syntax:** 
```python
if <test_condition1> then
	body of action
elsif <test_condition2>then
	body of action
...
...
else
	body of action
end if;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/ef394bd9-aa1d-46f8-b3dc-df0126834d38)

### 4. CASE Statement:
The CASE statement allows you to perform a series of conditional checks in a more structured way. If we try to describe the case statement in one line then, then we can say means "one out of many". It is a decision making statement that selects only one option out of the multiple available options.

**Syntax:** 
```python
CASE selector
	when value1 then Statement1;
	when value2 then Statement2;
	...
	...
	else statement;
end CASE;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/0a25423b-754b-4742-b819-2523c0f5beb8)

---

## <p align="left"> Ques-7. Error Handling using Internal Exceptions and External Exceptions. </p>
An exception is an error which disrupts the normal flow of program instructions. Exceptions are runtime errors or unexpected events that occur during the execution of a PL/SQL code block. PL/SQL provides us the exception block which raises the exception thus helping the programmer to find out the fault and resolve it. 

**Syntax to write an exception:**
```python
WHEN exception THEN 
    statement;
```

**Types of exceptions defined in PL/SQL:**
1. User defined (Internal) exceptions.
2. System defined (External) exceptions.

### 1. User defined (Internal) exceptions:
In any program, there is a possibility that a number of errors can occur that may not be considered as exceptions by oracle. In that case, an exception can be defined by the programmer while writing the code such type of exceptions are called User-defined exception.

User defined exceptions are in general defined to handle special cases where our code can generate exception due to our code logic.

Also, in your code logic, you can explicitly specify to genrate an exception using the RAISE keyword and then handle it using the EXCEPTION block.

### 2. System defined (External) exceptions:
In order to handle common exceptions that occur while running PL/SQL code, there are two types of exception handlers in oracle:
1. Named Exception Handler
2. Numbered Exception Handler

**Named Exception Handling:** Such exceptions are the predefined names given by oracle for those exceptions that occur most commonly.

**Numbered Exception Handling:** In oracle, some of the pre-defined exceptions are numbered in the form of four integers preceded by a hyphen symbol. To handle such exceptions we should assign a name to them before using them.
This can be done by using the Pragma exception technique in which a numbered exception handler is bound to a name. 

**Example:**
```python
DELIMITER //
 CREATE PROCEDURE ADD_DETAIL (IN course_id VARCHAR(25), IN course_name VARCHAR(27))
BEGIN
DECLARE NOT_NULL1 INT DEFAULT 0;
BEGIN
DECLARE EXIT HANDLER FOR 1048 SET NOT_NULL1 = 1;
INSERT INTO courses (course_id, course_name) VALUES (course_id, course_name);
SELECT 'SUCCESSFUL INSERT';
 END; 
IF NOT_NULL1 = 1 THEN
SELECT 'UNSUCCESSFUL INSERT DUE TO NULL VALUE';
END IF;
END;
//
```
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/a15647ea-a8f7-4804-b78c-038bc29b5113)
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/8830f6e9-72a0-409a-be91-c20bae3fd543)

---

## <p align="left"> Ques-8. Using various types of Cursors. </p>
<p> In SQL, a cursor is a database object that allows you to interact with individual rows returned by a query. Cursors are often used when you need to process one row at a time, rather than fetching the entire result set at once. There are several types of cursors in SQL, and their usage depends on the specific requirements of your application. </p>

### Types of Cursors:

### 1. Static Cursor: 
- A static cursor is not sensitive to changes made by other users to the data while the cursor is open.
- It fetches a snapshot of the data at the time the cursor is opened.

**Syntax:**
```python
    DECLARE cursor_name CURSOR STATIC FOR
    SELECT column1, column2, ...
    FROM your_table;
```

### 2. Dynamic Cursor:
- A dynamic cursor reflects changes made by other users to the data while the cursor is open.
- It does not fetch a snapshot but rather retrieves the current data each time a fetch is made.
    
**Syntax:**
```python
    DECLARE cursor_name CURSOR DYNAMIC FOR
    SELECT column1, column2, ...
    FROM your_table;
```

### 3. Forward-Only Cursor:
- A forward-only cursor only allows fetching rows in a forward direction (from the first to the last row).
- It is the most lightweight and performs better in terms of resource usage.

**Syntax:**
```python
    DECLARE cursor_name CURSOR FORWARD_ONLY FOR
    SELECT column1, column2, ...
    FROM your_table;
```

### 4. Scroll Cursor:
- A scroll cursor allows fetching rows in both forward and backward directions.
- It provides more flexibility but may be less efficient than forward-only cursors.

**Syntax:**
```python
      DECLARE cursor_name CURSOR SCROLL FOR
      SELECT column1, column2, ...
      FROM your_table;
```
  
### 5. Keyset Cursor:
- A keyset cursor is similar to a dynamic cursor but is more optimized as it only retrieves the key values of the rows.
- It is sensitive to changes in the data but doesn't retrieve the actual data until a fetch is made.

**Syntax:**
```python
    DECLARE cursor_name CURSOR KEYSET FOR
    SELECT column1, column2, ...
    FROM your_table;
```

**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/e83cfd5a-6c5c-418f-ae4b-60aa722b987e)
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/b5627313-8f39-4f15-abcc-f2e0662be687)

---

## <p align="left"> Ques-9. How to run Stored Procedures and Functions. </p>
<p>Stored Procedures and Functions are database objects in SQL that contain a set of precompiled SQL statements. They are designed to perform specific tasks and can be reused, making database development more efficient. Both stored procedures and functions enhance code modularity, improve security, and allow for better performance optimization.</p>

### Stored Procedures:

**1. Purpose:**
- Procedural Logic: Stored procedures contain a series of SQL statements and procedural logic, allowing for complex operations to be encapsulated in a single unit.

**2. Execution:**
-  Call Statement: Stored procedures are typically executed using a CALL or EXEC statement.

**3. Parameters:**
- Input/Output Parameters: Stored procedures can take input parameters, perform operations, and return results. They may also have output parameters.

**4. Transaction Control:**
- Transaction Management: Stored procedures can include transaction management commands (COMMIT and ROLLBACK) to control the scope of transactions.

**Running Stored Procedures:-** Before you can run a stored procedure, you need to create it. Use the CREATE PROCEDURE statement to define a stored procedure
```python  
CREATE PROCEDURE procedure_name
AS
BEGIN
-- SQL statements for the procedure
END;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/ca30c02f-2fb3-4678-927d-3879129b5549)

### Functions:

**1. Purpose:**
- Return Value: Functions are designed to return a single value or a table result, making them suitable for use in expressions or queries.

**2. Execution:**
- Select Statement: Functions are typically used within SELECT statements or as part of an expression.

**3. Parameters:**
- Input Parameters: Functions may accept input parameters, but they cannot have output parameters.

**4. Transaction Control:**
- No Transaction Management: Functions cannot contain transaction management commands like COMMIT or ROLLBACK.

**Running Functions:-** Use the CREATE FUNCTION statement to define a function. Functions return a value and can be used in SQL queries.
```python  
CREATE FUNCTION function_name
RETURNS data_type
AS
BEGIN
-- SQL statements for the function
RETURN value;
END;
```
**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/36a95e45-ba87-468b-b9e2-73eb7af13154)

---

## <p align="left"> Ques-10. Creating Packages and applying Triggers. </p>

### Creating Packages in PL/SQL:

A PL/SQL package is a collection of related procedures, functions, variables, and other constructs that are grouped together for modularity and reusability. Packages consist of two parts: the package specification and the package body.

**1. Package Specification:**
- Declares the public interface of the package.
- Contains declarations of procedures, functions, variables, types, and constants that are accessible from outside the package.
- Does not contain the implementation details.

**Syntax**
```python  
CREATE OR REPLACE PACKAGE Your_Package_Name AS
PROCEDURE Procedure_Name;
FUNCTION Function_Name RETURN NUMBER;
-- Declare variables, types, etc.
END Your_Package_Name;
```

**2. Package Body:**
- Implements the procedures and functions declared in the package specification.
- Contains the actual code for the functionality provided by the package.
- May include private variables and procedures that are not accessible outside the package.

**Syntax**
```python  
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
```

### Applying Triggers in PL/SQL:

A PL/SQL trigger is a set of instructions that are automatically executed in response to certain events on a table, such as an INSERT, UPDATE, or DELETE operation.

**1. Creating a Trigger:**
- Defines the trigger name, event (e.g., BEFORE INSERT, AFTER UPDATE), and the table on which the trigger should act.
- Contains the PL/SQL block with the logic to be executed when the trigger is fired.

**Syntax**
```python  
CREATE OR REPLACE TRIGGER Your_Trigger_Name
BEFORE INSERT ON Your_Table_Name
FOR EACH ROW
BEGIN
Your_Package_Name.Procedure_Name;
-- Your trigger logic here
END Your_Trigger_Name;
/
```

In this example, the trigger is set to execute before an INSERT operation on Your_Table_Name. The trigger calls the Procedure_Name from Your_Package_Name.

**2. Applying the Trigger:**
- Once the trigger is created, it needs to be associated with a specific table.

**Syntax** 
```python 
ALTER TABLE Your_Table_Name
ENABLE TRIGGER Your_Trigger_Name;
```

- This associates the trigger Your_Trigger_Name with the table Your_Table_Name.

**3. Testing the Trigger:**
- You can test the trigger by performing operations on the table that the trigger is associated with.

**Syntax**
```python 
INSERT INTO Your_Table_Name (column1, column2, ...)
VALUES (value1, value2, ...);
```
**Exampel:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/b6601b12-71bd-44f7-a895-681badc752d4)

---

## <p align="left"> Ques-11. Creating Arrays and Nested Tables. </p>

### Arrays
<p> An array is an ordered set of elements of a single built-in data type. An array can have an associated user-defined array type, or it can be the result of an SQL operation that returns an array value without an associated user-defined array type. You can declare a column to be of an array type, allowing you to store multiple values in a single column.You can perform various operations on arrays, such as indexing, slicing, and searching. Keep in mind that while arrays can be useful, they might not always be the most efficient solution for complex data structures.</p>

1. **Declaration:** Declare an associative array using the TYPE statement. Specify the data type of the elements and the index type.
2. **Initialization:** Initialize the array in the DECLARE section or later in the executable section.
3. **Accessing Elements:** Access elements by their index.

### Nested Tables
<p>Nested tables are single-dimensional, unbounded collections of homogeneous elements. First, a nested table is single-dimensional, meaning that each row has a single column of data like a one-dimension array. Second, a nested table is unbounded. It means that the number of elements of a nested table is predetermined. Third, homogeneous elements mean that all elements of a nested table have the same data type.</p>

**Example:**
![image](https://github.com/harmeet-811/rdbms_2023batch/assets/144206256/21f57fc0-0966-46f7-9c92-9249d8411952)

---

# <p align="center">THANKS</p>
