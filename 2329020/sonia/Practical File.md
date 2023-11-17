## Experiment:- 1
### Comparative study of various Database Management Systems
###### A comparative study of various Database Management Systems (DBMS) involves analyzing different systems based on several criteria such as performance, scalability, reliability, security, ease of use, and cost. There are various types of DBMS available, including relational, NoSQL, NewSQL, and object-oriented databases. Here's a general overview of how different types of DBMS compare based on these criteria:
###### 1. Relational Database Management Systems (RDBMS)
  ###### Examples: MySQL, PostgreSQL, Oracle, SQL Server
  ##### Advantages
  ###### - Mature technology with a well-defined standard (SQL).
  ######   - ACID transactions ensure data consistency and reliability.
   ######  - Suitable for complex queries and transactions.
   ######  - Support for joins and relationships between tables.
  ##### Disadvantages
   ######  - May not scale well horizontally.
 ######    - Schema changes can be complex.
 #####  Use Cases
   ######  - Business applications requiring complex queries and transactions.
  ######   - Situations where data integrity and consistency are critical.
##### 2. NoSQL Database Management Systems
######   Examples: MongoDB, Cassandra, Redis, Couchbase
 #####  Advantages
######     - Schema flexibility; can handle semi-structured or unstructured data.
 ######    - Horizontal scalability; easy to distribute across multiple nodes.
 ######    - Suitable for large volumes of rapidly changing data.
#####   Disadvantages
###### - Lack of ACID transactions in some cases.
  ######   - Limited support for complex queries.
#####   Use Cases
  ######   - Big data and real-time applications.
  ######   - Content management systems and e-commerce platforms.
######     - IoT applications.
##### 3. NewSQL Database Management Systems
 ######  Examples: Google Spanner, CockroachDB
 #####  Advantages
 ######    - Combines benefits of traditional RDBMS and NoSQL databases.
  ######   - Horizontal scalability with strong consistency.
 #####  Disadvantages
  ######   - Limited adoption and maturity compared to traditional RDBMS.
  ###### Use Cases
   ######  - Applications requiring global distribution and strong consistency.
 ######    - Financial applications and online transaction processing (OLTP) systems.
##### 4. Object-Oriented Database Management Systems (OODBMS)
 ######  Examples   db4o, ObjectDB
  ###### Advantages
  ######    - Store complex data types directly without the need for complex mapping.
  ######    - Support for object-oriented programming concepts.
 #####   Disadvantages
 ######     - Limited support and adoption compared to relational databases.
 ######     - Performance concerns for certain types of queries.
  ######  - Use Cases
 ######     - Object-oriented applications and systems with complex data structures.
 ######     - Applications where objects need to be persisted directly without mapping to tables.
 ###### Comparison Criteria:
 ##### 1. Performance
 ######   - RDBMS: Good for complex queries and transactions.
   ###### - NoSQL: High performance for read and write operations, especially in large-scale applications.
 ######   - NewSQL: Balanced performance for both complex queries and scalable transactions.
 ######   - OODBMS: Performance depends on the complexity of object relationships.
 ##### 2. Scalability
 ######   - RDBMS: Vertical scaling can be a limitation, but some offer limited horizontal scaling.
  ######  - NoSQL: Excellent horizontal scalability across distributed systems.
 ######   - NewSQL: Horizontal scalability with strong consistency.
  ######  - OODBMS: Limited scalability compared to other types.
 ##### 3. Reliability and Consistency
 ######   - RDBMS: ACID transactions ensure data integrity and consistency.
  ######  - NoSQL: Eventual consistency in many cases, but some offer strong consistency options.
  ######  - NewSQL: ACID transactions with horizontal scalability.
  ######  - OODBMS: ACID transactions for object-oriented data.
 ##### 4. Flexibility and Schema Design
  ######  - RDBMS: Schema is fixed and must be defined before data insertion.
  ######  - NoSQL: Flexible schema; can handle semi-structured and unstructured data.
  ######  - NewSQL: Similar to RDBMS with schema definition.
 ######   - OODBMS: Schema flexibility, supports complex object structures.
 ##### 5. Security
 ###### - RDBMS: Mature security features, including role-based access control and encryption.
 ######   - NoSQL: Security features vary; some offer robust security mechanisms.
  ######  - NewSQL: Security features comparable to traditional RDBMS.
  ######  - OODBMS: Security features are usually present but may not be as extensive as RDBMS.
 ##### 6. Ease of Use and Development
  ######  - RDBMS: Mature tools, well-established query language (SQL).
  ######  - NoSQL: Diverse query languages, may require learning different interfaces for different databases.
  ######  - NewSQL: SQL-based interfaces, similar to traditional RDBMS.
 ######   - OODBMS: Object-oriented query languages, suitable for developers familiar with object-oriented programming concepts.
 ##### 7. Community and Support
 ######   - RDBMS: Large, active communities and extensive documentation.
 ######   - NoSQL: Active communities, but support may vary based on the specific database.
  ######  - NewSQL: Smaller communities compared to RDBMS and NoSQL.
 ######   - OODBMS: Smaller communities; limited resources and support compared to RDBMS.
 ##### Conclusion
 ###### - Choose an RDBMS when data integrity, ACID transactions, and complex queries are crucial.
 ###### - Opt for NoSQL databases for flexible schema, horizontal scalability, and handling large volumes of semi-structured/unstructured data.
 ###### - Consider NewSQL databases for applications requiring global distribution and strong consistency.
 ###### - Use OODBMS for applications with complex object structures and a need for direct object persistence.
## Experiment:- 2
#### Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL)
##### What is SQL?
###### SQL is a database language designed for the retrieval and management of data in a relational database. SQL is the standard language for database management. All the RDBMS systems like MySQL, MS Access, Oracle, Sybase, Postgres, and SQL Server use SQL as their standard database language. SQL programming language uses various commands for different operations. We will learn about the like DCL, TCL, DQL, DDL and DML
###### Brief History of SQL
###### Here, are important landmarks from the history of SQL:
* 	1970 – Dr. Edgar F. “Ted” Codd described a relational model for databases.
* 	1974 – Structured Query Language appeared.
*	1978 – IBM released a product called System/R.
*	1986 – IBM developed the prototype of a relational database, which is standardized by ANSI.
*	1989- First ever version launched of SQL
*	1999 – SQL 3 launched with features like triggers, object-orientation, etc.
*	SQL2003- window functions, XML-related features, etc.
*	SQL2006- Support for XML Query Language
*	SQL2011-improved support for temporal databases
##### Types of SQL
###### Here are five types of widely used SQL queries.
* Data Definition Language (DDL)
*	Data Manipulation Language (DML)
*	Data Control Language(DCL)
##### What is DDL?
###### Data Definition Language helps you to define the database structure or schema. Let’s learn about DDL commands with syntax.
###### Five types of DDL commands in SQL are:
###### CREATE
###### CREATE statements is used to define the database structure schema:
##### Syntax:
```CREATE TABLE TABLE_NAME (COLUMN_NAME DATATYPES[,....]);```
##### For example:
```Create database university;``` <br>
``` Create table students; ``` <br>
```Create view for_students;``` <br>
###### DROP
###### Drops commands remove tables and databases from RDBMS.
##### Syntax
``` DROP TABLE ; ```
 ##### For example:
```Drop object_type object_name;``` <br>
``` Drop database university; ``` <br>
```Drop table student;```<br>
###### ALTER
###### Alters command allows you to alter the structure of the database.
##### Syntax:
###### To add a new column in the table
```ALTER TABLE table_name ADD column_name COLUMN-definition;``` 
###### To modify an existing column in the table:
```ALTER TABLE MODIFY(COLUMN DEFINITION....);  ```
##### For example:
```Alter table guru99 add subject varchar;``` 
##### TRUNCATE
###### This command used to delete all the rows from the table and free the space containing the table.
##### Syntax:
```TRUNCATE TABLE table_name; ``` 
##### Example:
```TRUNCATE table students;```
##### What is Data Manipulation Language?
###### Data Manipulation Language (DML) allows you to modify the database instance by inserting, modifying, and deleting its data. It is responsible for performing all types of data modification in a database.
###### There are three basic constructs which allow database program and user to enter data and information are:
###### Here are some important DML commands in SQL:
*	INSERT
*	UPDATE
*	DELETE
       * INSERT
###### This is a statement is a SQL query. This command is used to insert data into the row of a table.
##### Syntax:
```INSERT INTO TABLE_NAME  (col1, col2, col3,.... col N)```  
```VALUES (value1, value2, value3, .... valueN);```  
 ###### OR
```INSERT INTO TABLE_NAME```    
```VALUES (value1, value2, value3, .... valueN);```    
##### For example:
```INSERT INTO students (RollNo, FIrstName, LastName) VALUES ('60', 'Tom', Erichsen');```
##### UPDATE
##### This command is used to update or modify the value of a column in the table.
###### Syntax:
```UPDATE table_name SET [column_name1= value1,...column_nameN = valueN] [WHERE CONDITION] ```  
##### For example:
```UPDATE students```    
```SET FirstName = 'Jhon', LastName= 'Wick'``` 
```WHERE StudID = 3;```
  ##### DELETE
###### This command is used to remove one or more rows from a table.
##### Syntax:
###### DELETE FROM table_name [WHERE condition];  
###### For example:
```DELETE FROM students``` 
```WHERE FirstName = 'Jhon';```
##### What is DCL?
###### DCL (Data Control Language) includes commands like GRANT and REVOKE, which are useful to give “rights & permissions.” Other permission controls parameters of the database system.
###### Examples of DCL commands
###### Commands that come under DCL:
*	Grant
*	Revoke
##### Grant
###### This command is use to give user access privileges to a database.
##### Syntax:
```GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER; ``` 
###### For example:
```GRANT SELECT ON Users TO'Tom'@'localhost;```
##### Revoke
###### It is useful to back permissions from the user.
##### Syntax:
```REVOKE privilege_nameON object_nameFROM {user_name |PUBLIC |role_name}```
###### For example:
```REVOKE SELECT, UPDATE ON student FROM BCA, MCA;  ```
##### Summary
*	SQL is a database language designed for the retrieval and management of data in a relational database.
*	It helps users to access data in the RDBMS system
*	In the year 1974, the term Structured Query Language appeared
*	Five types of SQL queries are 1) Data Definition Language (DDL) 2) Data Manipulation Language (DML) 3) Data Control Language(DCL) 4) Transaction Control Language(TCL) and, 5) Data Query Language (DQL)
*	Data Definition Language(DDL) helps you to define the database structure or schema.
*	Data Manipulation Language (DML) allows you to modify the database instance by inserting, modifying, and deleting its data.
*	DCL (Data Control Language) includes commands like GRANT and REVOKE, which are useful to give “rights & permissions.”
*	Transaction control language or TCL commands deal with the transaction within the database.
*	Data Query Language (DQL) is used to fetch the data from the database.
## Experiment:- 3
### How to apply Constraints at various levels.
###### Constraints in SQL
###### Constraints in SQL means we are applying certain conditions or restrictions on the database. This further means that before inserting data into the database, we are checking for some conditions. If the condition we have applied to the database holds true for the data which is to be inserted, then only the data will be inserted into the database tables.
##### Constraints in SQL can be categorized into two types:
 ######   1. Column Level Constraint:
##### Column Level Constraint is used to apply a constraint on a single column.
  ###### 2. Table Level Constraint:
###### Table Level Constraint is used to apply a constraint on multiple columns.
###### Constraints available in SQL are:
######    1. NOT NULL
######    2. UNIQUE
######    3. PRIMARY KEY
######    4. FOREIGN KEY
######    5. CHECK
######    6. DEFAULT
######    7. CREATE INDEX
###### Now let us try to understand the different constraints available in SQL in more detail with the help of examples. We will use MySQL database for writing all the queries.
##### 1. NOT NULL
    * NULL means empty, i.e., the value is not available.
    * Whenever a table's column is declared as NOT NULL, then the value for that column cannot be empty for any of the table's records.
    * There must exist a value in the column to which the NOT NULL constraint is applied.
######   CREATE TABLE TableName (ColumnName1 datatype NOT NULL, ColumnName2 datatype,…., ColumnNameN datatype);
##### Example:
###### Create a student table and apply a NOT NULL constraint on one of the table's column while creating a table.
<b>```1.CREATE TABLE student(StudentID INT NOT NULL, Student_FirstName VARCHAR(20), Student_LastName VARCHAR(20), Student_PhoneNumber VARCHAR(20), Student_Email_ID VARCHAR(40));```</b>  
<img src="Screenshot from 2023-11-16 15-05-06.png">
![Screenshot from 2023-11-16 15-05-06](https://github.com/Soniasharma8/Practice/assets/144365209/7e668a52-c4fe-4782-8328-565b70346599)
To verify that the not null constraint is applied to the table's column and the student table is created successfully, we will execute the following query:
   ##### 1. mysql> DESC student;  
  ![Screenshot from 2023-11-16 15-07-40](https://github.com/Soniasharma8/Practice/assets/144365209/75a185d5-b15c-483e-9166-1b34c083dc8d)
##### 2. UNIQUE
    * Duplicate values are not allowed in the columns to which the UNIQUE constraint is applied.
    * The column with the unique constraint will always contain a unique value.
    * This constraint can be applied to one or more than one column of a table, which means more than one unique constraint can exist on a single table.
    * Using the UNIQUE constraint, you can also modify the already created tables.
##### Syntax to apply the UNIQUE constraint on a single column:
   <b> ```1. CREATE TABLE TableName (ColumnName1 datatype UNIQUE, ColumnName2 datatype,…., ColumnNameN datatype);``` </b>  
##### Example:
##### Create a student table and apply a UNIQUE constraint on one of the table's column while creating a table.
##### 1.mysql> CREATE TABLE student(StudentID INT UNIQUE, Student_FirstName VARCHAR(20), Student_LastName VARCHAR(20), Student_PhoneNumber VARCHAR(20), Student_Email_ID VARCHAR(40));  
    ![Screenshot from 2023-11-16 17-16-15](https://github.com/Soniasharma8/Practice/assets/144365209/6d9c18b2-a20c-4720-9f52-58e5ecf591e6)
To verify that the unique constraint is applied to the table's column and the student table is created successfully, we will execute the following query:
   ##### 1. mysql> DESC student;  
    ![Screenshot from 2023-11-16 17-18-56](https://github.com/Soniasharma8/Practice/assets/144365209/cd4bc291-ae0b-4305-a542-3a1188ab2233)
##### 3. PRIMARY KEY
    * PRIMARY KEY Constraint is a combination of NOT NULL and Unique constraints.
    * NOT NULL constraint and a UNIQUE constraint together forms a PRIMARY constraint.
    * The column to which we have applied the primary constraint will always contain a unique value and will not allow null values.
##### Syntax of primary key constraint during table creation:
  <b>  ```1. CREATE TABLE TableName (ColumnName1 datatype PRIMARY KEY, ColumnName2 datatype,…., ColumnNameN datatype);``` </b>  
###### Example:
###### Create a student table and apply the PRIMARY KEY constraint while creating a table.
<b> ```1.mysql> CREATE TABLE student(StudentID INT PRIMARY KEY, Student_FirstName VARCHAR(20), Student_LastName VARCHAR(20), Student_PhoneNumber VARCHAR(20), Student_Email_ID VARCHAR(40));``` </b>  
##### 4. FOREIGN KEY
    * A foreign key is used for referential integrity.
    * When we have two tables, and one table takes reference from another table, i.e., the same column is present in both the tables and that column acts as a primary key in one table. That particular column will act as a foreign key in another table.
Syntax to apply a foreign key constraint during table creation:
<b> ```CREATE TABLE tablename(ColumnName1 Datatype(SIZE) PRIMARY KEY, ColumnNameN Datatype(SIZE), FOREIGN KEY( ColumnName ) REFERENCES PARENT_TABLE_NAME(Primary_Key_ColumnName));``` </b>  
##### Example:
###### Create an employee table and apply the FOREIGN KEY constraint while creating a table.
###### To create a foreign key on any table, first, we need to create a primary key on a table.
  <b> ``` mysql> CREATE TABLE employee (Emp_ID INT NOT NULL PRIMARY KEY, Emp_Name VARCHAR (40), Emp_Salary VARCHAR (40)); ``` </b>
##### 5. CHECK
    * Whenever a check constraint is applied to the table's column, and the user wants to insert the value in it, then the value will first be checked for certain conditions before inserting the value into that column.
    * For example: if we have an age column in a table, then the user will insert any value of his choice. The user will also enter even a negative value or any other invalid value. But, if the user has applied check constraint on the age column with the condition age greater than 18. Then in such cases, even if a user tries to insert an invalid value such as zero or any other value less than 18, then the age column will not accept that value and will not allow the user to insert it due to the application of check constraint on the age column.
Syntax to apply check constraint on a single column:
 <b>  ``` 1. CREATE TABLE TableName (ColumnName1 datatype CHECK (ColumnName1 Condition), ColumnName2 datatype,…., ColumnNameN datatype);``` </b>  
##### Example:
##### Create a student table and apply CHECK constraint to check for the age less than or equal to 15 while creating a table.
    <b> ```1. mysql> CREATE TABLE student(StudentID INT, Student_FirstName VARCHAR(20), Student_LastName VARCHAR(20), Student_PhoneNumber VARCHAR(20), Student_Email_ID VARCHAR(40), Age INT CHECK( Age <= 15));``` </b>
   ##### 6. DEFAULT
###### Whenever a default constraint is applied to the table's column, and the user has not specified the value to be inserted in it, then the default value which was specified while applying the default constraint will be inserted into that particular column.
###### Syntax to apply default constraint during table creation:
  <b> ```  1. CREATE TABLE TableName (ColumnName1 datatype DEFAULT Value, ColumnName2 datatype,…., ColumnNameN datatype);  ``` </b>
##### Example:
###### Create a student table and apply the default constraint while creating a table.
<b>```mysql> CREATE TABLE student(StudentID INT, Student_FirstName VARCHAR(20), Student_LastName VARCHAR(20), Student_PhoneNumber VARCHAR(20), Student_Email_ID VARCHAR(40) DEFAULT "anuja.k8@gmail.com");``` </b>
##### 7. CREATE INDEX
###### CREATE INDEX constraint is used to create an index on the table. Indexes are not visible to the user, but they help the user to speed up the searching speed or retrieval of data from the database.
###### Syntax to create an index on single column:
   ##### 1. CREATE INDEX IndexName ON TableName (ColumnName 1);  
###### Example:
###### Create an index on the student table and apply the default constraint while creating a table.
 <b>```1. mysql> CREATE INDEX idx_StudentID ON student (StudentID);```</b>  
## Experiment:- 4
### View data in the required form using Operators, Functions and Joins.
###### An SQL operator is a reserved word or a character used primarily in an SQL statement's WHERE clause to perform operation(s), such as comparisons and arithmetic operations. These Operators are used to specify conditions in an SQL statement and to serve as conjunctions for multiple conditions in a statement.

###### An SQL operator can be either a unary or binary operator. A unary operator (example unary + or unary - ) uses only one operand to perform the unary operation, whereas the binary operator (example + or - etc) uses two operands to perform the binary operation.

##### SQL supports following types of operators:

* Arithmetic operators
* Comparison operators
* Logical operators

<b>SQL Arithmetic Operators</b>
###### SQL Arithmetic Operators are used to perform mathematical operations on the numerical values. SQL provides following operators to perform mathematical operations.

###### Here is a list of all the arithmetic operators available in SQL.
|Operator	| Description	 | Example     |
|:-------:|:------------:|:-----------:|
|+        |Addition	     |10 + 20 = 30 |
|-        |Subtraction	 |20 - 30 = -10|
|*	      |Multiplication|10 * 20 = 200|
|/      	|Division	     |20 / 10 = 2  |
|%	      |Modulus	     |5 % 2 = 1    |

#### SQL Comparison Operators
##### SQL Comparison Operators test whether two given expressions are the same or not. These operators are used in SQL conditional statements while comparing one expression with another and they return a Boolean value which can be either TRUE or FALSE. The result of an SQL comparison operation can be UNKNOWN when one or another operand has it's value as NULL.

##### Here is a list of all the comparison operators available in SQL.

|Operator  | Description	            | Example           |
|:--------:|:------------------------:|:-----------------:|
| =	       |Equal to	                |5 = 5 returns TRUE |
| !=	     | Not equal	              |5 != 6 returns TRUE|
| <>       |Not equal	                |5 <> 4 returns TRUE|
| >	       |Greater than	            |4 > 5 returns FALSE|
| <        |Less than	                |4 < 5 returns TRUE |
| >=       |Greater than or equal to  |4 >= 5 returns FALSE|
| <=       |Less than or equal to	    |4 <= 5 returns TRUE|
| !<       |Not less than	            |4 !< 5 returns FALSE|
| !>       |Not greater than        	|4 !> 5 returns TRUE

##### SQL Logical Operators
##### SQL Logical Operators are very similar to comparison operators and they test for the truth of some given condition. These operators return a Boolean value which can be either a TRUE or FALSE. The result of an SQL logical operation can be UNKNOWN when one or another operand has it's value as NULL.

##### Here is a list of all the logical operators available in SQL.

|Operator |	Description	|
|:-------:|:-----------:|
|ALL |	TRUE if all of a set of comparisons are TRUE.	|
|AND |	TRUE if all the conditions separated by AND are TRUE.|	
|ANY |TRUE if any one of a set of comparisons are TRUE.	|
|BETWEEN	|TRUE if the operand lies within the range of comparisons. |
|EXISTS	|TRUE if the subquery returns one or more records	|
|IN	|TRUE if the operand is equal to one of a list of expressions. |	
|LIKE|	TRUE if the operand matches a pattern specially with wildcard. |	
|NOT	|Reverses the value of any other Boolean operator.	|
|OR	|TRUE if any of the conditions separated by OR is TRUE	|
|IS |NULL	TRUE if the expression value is NULL.	|
|SOME	|TRUE if some of a set of comparisons are TRUE. |	
|UNIQUE|	The UNIQUE operator searches every row of a specified table for uniqueness (no duplicates). |	

<b>SQL | Join (Inner, Left, Right and Full Joins)</b>
##### SQL Join statement is used to combine data or rows from two or more tables based on a common field between them. Different types of Joins are as follows: 

* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* FULL JOIN
* NATURAL JOIN 
##### Consider the two tables below as follows: 
##### Student
##### Student
![table1-3](https://github.com/Soniasharma8/Practice/assets/144365209/10cfc3fa-91c8-43cc-95cd-14f448be71d2)

##### StudentCourse 
![table5](https://github.com/Soniasharma8/Practice/assets/144365209/0b80b48e-495a-432e-a168-f93bc2de9a4e)
##### The simplest Join is INNER JOIN. 
#### A. INNER JOIN
##### The INNER JOIN keyword selects all rows from both the tables as long as the condition is satisfied. This keyword will create the result-set by combining all rows from both the tables where the condition satisfies i.e value of the common field will be the same. 

##### Syntax: 

```SELECT table1.column1,table1.column2,table2.column1,....```
```FROM table1 ```<br>
```INNER JOIN table2```<br>
```ON table1.matching_column = table2.matching_column;```<br>


```table1: First table.```<br>
```table2: Second table```
##### matching_column: Column common to both the tables.
![6a0120a85dcdae970b012877702708970c-pi](https://github.com/Soniasharma8/Practice/assets/144365209/911ca39e-c956-4806-9619-c7d50a9f5120)
##### Example Queries(INNER JOIN)

##### This query will show the names and age of students enrolled in different courses.  
```SELECT StudentCourse.COURSE_ID, Student.NAME, Student.AGE FROM Student```
```INNER JOIN StudentCourse```
```ON Student.ROLL_NO = StudentCourse.ROLL_NO;```
##### Output:  
![table22](https://github.com/Soniasharma8/Practice/assets/144365209/c5ee097c-fb4f-4c89-822e-acf54a77b832)
![Screenshot from 2023-10-24 20-21-40](https://github.com/Soniasharma8/Practice/assets/144365209/4f892515-92a1-4caa-a89b-d9d6809c18f4)

#### B. LEFT JOIN
##### This join returns all the rows of the table on the left side of the join and matches rows for the table on the right side of the join. For the rows for which there is no matching row on the right side, the result-set will contain null. LEFT JOIN is also known as LEFT OUTER JOIN.

##### Syntax: 

```SELECT table1.column1,table1.column2,table2.column1,....```
```FROM table1 ```<br>
```LEFT JOIN table2```<br>
```ON table1.matching_column = table2.matching_column;```<br>


```table1: First table.```<br>
```table2: Second table```
##### matching_column: Column common to both the tables.
![VkAT5](https://github.com/Soniasharma8/Practice/assets/144365209/4e5306d9-0284-47dd-b0a9-4852672eba2f)
##### Example Queries(LEFT JOIN): 

```SELECT Student.NAME,StudentCourse.COURSE_ID ```
```FROM Student```<br>
```LEFT JOIN StudentCourse ```<br>
```ON StudentCourse.ROLL_NO = Student.ROLL_NO;```<br>
##### Output: 
![table31](https://github.com/Soniasharma8/Practice/assets/144365209/d31c6946-8495-46fe-b4ee-5a2f02319e4a)

![Screenshot from 2023-10-24 20-34-18](https://github.com/Soniasharma8/Practice/assets/144365209/49a8f3d3-fc50-4ff6-91fa-47c6b21111e9)

#### C. RIGHT JOIN
##### RIGHT JOIN is similar to LEFT JOIN. This join returns all the rows of the table on the right side of the join and matching rows for the table on the left side of the join. For the rows for which there is no matching row on the left side, the result-set will contain null. RIGHT JOIN is also known as RIGHT OUTER JOIN. 
##### Syntax: 
```SELECT table1.column1,table1.column2,table2.column1,....```
```FROM table1``` <br>
```RIGHT JOIN table2```<br>
```ON table1.matching_column = table2.matching_column;```<br>
```table1: First table.```<br>
```table2: Second table```<br>
##### matching_column: Column common to both the tables.
![join](https://github.com/Soniasharma8/Practice/assets/144365209/30ba7fe0-b31a-46fd-9b70-0a7ca6c93b3b)
##### Example Queries(RIGHT JOIN):

```SELECT Student.NAME,StudentCourse.COURSE_ID ```
```FROM Student```<br>
```RIGHT JOIN StudentCourse ```<br>
```ON StudentCourse.ROLL_NO = Student.ROLL_NO;```<br>
##### Output: 

![table6](https://github.com/Soniasharma8/Practice/assets/144365209/4febab2e-b60d-48ba-9549-d96bf878c07f)
![Screenshot from 2023-10-24 21-52-21](https://github.com/Soniasharma8/Practice/assets/144365209/facf94c1-f712-4b7f-b013-9b70f55705ea)

#### D. FULL JOIN
##### FULL JOIN creates the result-set by combining results of both LEFT JOIN and RIGHT JOIN. The result-set will contain all the rows from both tables. For the rows for which there is no matching, the result-set will contain NULL values.
![3Ll1h](https://github.com/Soniasharma8/Practice/assets/144365209/12658f30-76b4-4641-a87b-52b7cccd568f)
##### Syntax:  

```SELECT table1.column1,table1.column2,table2.column1,....```
```FROM table1 ```<br>
```FULL JOIN table2```<br>
```ON table1.matching_column = table2.matching_column;```<br>


```table1: First table.```<br>
```table2: Second table```<br>
```matching_column: Column common to both the tables. ```
## Experiment:- 5
#### 1. SIMPLE view: - Simple views are the most basic type of view in MariaDB. They are created by selecting a subset of columns from one or more tables.
    IMAGE
  #### 2. JOIN view: - Join views allow you to combine data from multiple tables and present it as a single view. You can create views that perform joins on underlying tables to simplify complex queries.
  IMAGE

  ## EXPERIMENT:- 6
  #### How to apply Conditional Controls in Pl/SQL
  ##### In this chapter, we will discuss conditions in PL/SQL. Decision-making structures require that the programmer specify one or more conditions to be evaluated or tested by the program, along with a statement or statements to be executed if the condition is determined to be true, and optionally, other statements to be executed if the condition is determined to be false.

##### Following is the general form of a typical conditional (i.e., decision making) structure found in most of the programming languages −
![decision_making](https://github.com/Soniasharma8/Practice/assets/144365209/04f2c84a-4bdc-428e-88ca-daf6ee02c476)

#####  1. IF Statement: - You can use the IF statement to execute different SQL statements based on a condition.
![Screenshot from 2023-11-17 00-06-41](https://github.com/Soniasharma8/Practice/assets/144365209/f1d20f4d-d411-4513-83b8-343e139f8be7)
##### 2. CASE Statement: - The CASE statement allows you to perform conditional logic within SQL queries. You can use it to return different values based on specific conditions.
IMAGE
 ## EXPERIMENT:- 7
 #### Error Handling using Internal Exceptions and External Exceptions.
##### MariaDB supports error handling through both internal exceptions and external exceptions. Internal exceptions are typically used within stored procedures, while external exceptions are errors that can be caught in the client application that calls the database.
##### 1. Internal Exception (in Stored Procedures): -
![Screenshot from 2023-11-17 08-59-32](https://github.com/Soniasharma8/Practice/assets/144365209/eb8b9b30-e1fe-4e85-83d8-9b0f1e5da5eb)

##### 2. External Exception (in Stored Procedure): -
Image
 ## EXPERIMENT:- 8
 #### Using various types of Cursors
 ##### A Cursor is a temporary memory that is allocated by the database server at the time of performing the Data Manipulation Language operations on a table, such as INSERT, UPDATE and DELETE etc. It is used to retrieve and manipulate data stored in the SQL table.
#### Properties of Cursors

##### Following are the properties of MySQL Cursors −

```* READ ONLY − We cannot update or modify any records in the table using the MySQL cursors. We can just fetch and process data from a table.```

 ```  * Non-Scrollable − We can retrieve records from a table in a single direction, i.e. from the first record or the last. We cannot move backward or jump to a specific position within the result set.```

 ```  * Asensitive Cursor − An asensitive cursor operates directly on the actual data in the database, it does not create a copy of the data. If any change is made to the data by other connections, it can affect the data that the cursor is working with.```
#### Life Cycle of the Cursor

##### There are four steps to manage these cursors. Following diagram illustrates the lifecycle of an SQL cursor −
![cursor_lifecycle](https://github.com/Soniasharma8/Practice/assets/144365209/0198f91d-579e-41ed-b3ac-9677cecf115e)
#### Declare Cursor Statement

##### In MySQL we can declare a cursor using the DECLARE statement and associate it with a SELECT statement to retrieve records from a database table.

##### However, this SELECT statement associated with a cursor does not use the INTO clause, as it's purpose is to fetch and process rows rather than assigning values to variables.
#### Syntax

##### Following is the syntax to declare a cursor in MySQL database −
```DECLARE cursor_name CURSOR FOR select_statement;```

#### Open Cursor Statement

##### After declaring a cursor in MySQL, the next step is to open the cursor using the OPEN statement. It initializes the result-set, allowing us to fetch and process rows from the associated SELECT statement in the cursor.
#### Syntax

##### Following is the syntax to open a cursor in MySQL database −

```OPEN cursor_name;```

#### Fetch Cursor Statement

##### Then, we can use the FETCH statement to retrieve the current row pointed by the cursor, and with each FETCH, the cursor moves to the next row in the result set. This allows us to process each row one by one.
#### Syntax

##### Following is the syntax to fetch a cursor in MySQL database −

```FETCH cursor_name INTO variable_list;```
#### Close Cursor Statement

##### Once all the rows are fetched, we must close the cursor to release the memory associated with it. We can do this using the CLOSE statement.
#### Syntax

##### Following is the syntax to close a cursor in MySQL database −

```CLOSE cursor_name;```

##### Example

##### In this example, let us see how to manage a cursor in a stored procedure.

##### Assume we have created a table with the name CUSTOMERS using the CREATE TABLE statement as follows −
![Screenshot from 2023-11-17 08-45-09](https://github.com/Soniasharma8/Practice/assets/144365209/521f8e56-fc7e-4191-864b-d31e0606aea5)
##### Now, let us insert some records into the CUSTOMERS table using the INSERT statement as follows −
![Screenshot from 2023-11-17 08-46-43](https://github.com/Soniasharma8/Practice/assets/144365209/4c71c9db-7f1e-4312-8ade-0b511446f26c)
##### Now, we will create a backup table named 'CUSTOMERS_BACKUP' to store customer data −
![Screenshot from 2023-11-17 08-47-44](https://github.com/Soniasharma8/Practice/assets/144365209/705e8155-bc4f-40bb-9468-56f8ac780e5d)
##### Here, we are creating a stored procedure named FetchCustomers to fetch customer names from the CUSTOMERS table and inserting them one by one into the BACKUP table. We are using a cursor to iterate through the rows and a handler to detect the end of the result-set, ensuring all names are processed − 
![Screenshot from 2023-11-17 08-49-48](https://github.com/Soniasharma8/Practice/assets/144365209/2d5be718-3698-4e56-b9e8-97915fce4293)
##### Once we create the procedure successfully, we can execute it using the CALL statement as shown below −
## EXPERIMENT:- 9
#### How to run Stored Procedures and Functions
##### 1. STORED PROCEDURE: - You can create stored procedures in MariaDB to encapsulate conditional logic and reuse it in multiple queries or applications. Here's an example of a simple stored procedure with conditional logic:
![Screenshot from 2023-11-17 08-23-15](https://github.com/Soniasharma8/Practice/assets/144365209/d63805b9-b64e-43d3-a6b8-65ac175c9b1d)

##### 2. STORED FUNCTION: - In MariaDB, a function is a stored program that you can pass parameters into and then return a value.
![Screenshot from 2023-11-17 08-29-16](https://github.com/Soniasharma8/Practice/assets/144365209/6e120fbe-4e45-4e60-b102-937ec5ff93d4)


## EXPERIMENT:- 10
#### Creating Packages and applying Triggers
##### Trigger is invoked by Oracle engine automatically whenever a specified event occurs.Trigger is stored into database and invoked repeatedly, when specific condition match.

##### Triggers are stored programs, which are automatically executed or fired when some event occurs.

##### Triggers are written to be executed in response to any of the following events.

  * A database manipulation (DML) statement (DELETE, INSERT, or UPDATE).
  * A database definition (DDL) statement (CREATE, ALTER, or DROP).
   * A database operation (SERVERERROR, LOGON, LOGOFF, STARTUP, or SHUTDOWN).
Advantages of Triggers

*  Trigger generates some derived column values automatically
* Enforces referential integrity
*   Event logging and storing information on table access
*  Auditing
*   Synchronous replication of tables
*    Imposing security authorizations
*   Preventing invalid transactions
IMAGE
## EXPERIMENT:- 11
#### Creating Arrays and Nested Tables.
##### 1. Arrays: - An array is an ordered set of elements of a single built-in data type. An array can have an associated user-defined array type, or it can be the result of an SQL operation that returns an array value without an associated user-defined array type.
![Screenshot from 2023-11-17 07-25-57](https://github.com/Soniasharma8/Practice/assets/144365209/8bab4972-03e7-40bd-b994-6cd1f3e9f60a)
![Screenshot from 2023-11-17 07-29-02](https://github.com/Soniasharma8/Practice/assets/144365209/8e49c96a-588d-47ab-87ac-d4feba9c4850)
##### 2. Nested Tables: - Nested tables are single-dimensional, unbounded collections of homogeneous elements. First, a nested table is single-dimensional, meaning that each row has a single column of data like a one-dimension array. Second, a nested table is unbounded. It means that the number of elements of a nested table is predetermined. Third, homogeneous elements mean that all elements of a nested table have the same data type.
![Screenshot from 2023-11-17 07-35-47](https://github.com/Soniasharma8/Practice/assets/144365209/2d71dfa0-5930-43f7-a4f5-918c8e16d469)
![Screenshot from 2023-11-17 07-41-55](https://github.com/Soniasharma8/Practice/assets/144365209/65c8c3e7-6750-40c0-a748-31249853717f)
![Screenshot from 2023-11-17 07-44-42](https://github.com/Soniasharma8/Practice/assets/144365209/2b850d60-2f63-443b-ad67-39751ff1290d)
