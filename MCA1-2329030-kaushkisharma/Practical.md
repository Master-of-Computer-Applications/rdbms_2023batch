**Mysql**
    MySQL is an open-source RDBMS known for its speed and reliability.
    It is widely used in web applications and is known for its ease of use.
    MySQL is available in both open-source and commercial versions.

**PostgreSQL:**

    PostgreSQL is an open-source RDBMS known for its advanced features and extensibility.
    It offers support for various data types, including JSON and spatial data.
    PostgreSQL is highly extensible through user-defined functions and extensions.

**oracle Database:**

    Oracle Database is a commercial RDBMS with a focus on enterprise-level applications.
    It offers high performance, scalability, and advanced features such as partitioning, clustering, and in-memory processing.
    Oracle Database is often used in large organizations for mission-critical applications.

**Microsoft SQL Server:**

    SQL Server is a commercial RDBMS developed by Microsoft.
    It offers tight integration with other Microsoft products and services.
    SQL Server is commonly used for enterprise-level applications on the Windows platform.

**IBM Db2:**

    Db2 is a family of data management products from IBM, including both RDBMS and NoSQL options.
    It is known for its reliability, performance, and support for large-scale databases.
    Db2 is used in a variety of enterprise applications.

**SQLite:**

    SQLite is an embedded database engine that is often used in mobile applications, desktop applications, and lightweight web applications.
    It is a self-contained, serverless, zero-configuration database engine.
    SQLite is not suitable for high-transaction or high-concurrency scenarios but excels in embedded and single-user applications

    ** The advantages of using a DBMS:**

    Data Organization and Structured Storage:
        DBMS provides a structured and organized way to store and manage data, making it easier to locate, access, and update information.

    Data Integrity:
        DBMS enforces data integrity constraints to maintain data accuracy, consistency, and reliability.

    Data Security:
        DBMS offers access control and security features to restrict unauthorized access to data and protect sensitive information.
            Data Redundancy Reduction:
        By centralizing data in a database, redundancy and data duplication are minimized, leading to storage efficiency and consistency.

    Data Scalability:
        DBMS systems are designed to handle large volumes of data and can be scaled to accommodate growing data requirements.

    Concurrent Access and Multi-User Support:
        DBMS manages multiple users or applications accessing data simultaneously, ensuring data consistency and preventing conflicts.

    Data Backup and Recovery:
        DBMS provides tools for data backup, restoration, and disaster recovery, safeguarding data against loss.

    Efficient Data Retrieval:
        Query languages, such as SQL, enable efficient and quick data retrieval for reporting and analysis.

    Data Independence:
        DBMS separates the physical and logical aspects of data, allowing changes to the database structure without affecting data access or application code.

    Data Consistency:
        DBMS enforces referential integrity and consistency rules, ensuring that relationships between data in different tables are maintained.

    Data Redundancy Reduction:
        By centralizing data in a database, redundancy and data duplication are minimized, leading to storage efficiency and consistency.

    Simplified Data Maintenance:
        DBMS simplifies data maintenance tasks, such as adding or deleting records, updating data, and managing data relationships.

    Reporting and Analytics:
        DBMS facilitates data analysis and reporting through the use of queries and reporting tools.

    Scalability and Performance Optimization:
        DBMS can be optimized for high performance through indexing, query optimization, and caching mechanisms.

    Data Recovery:
        In the event of hardware failures or data corruption, DBMS provides mechanisms for data recovery and restoration.

    Data Consistency Across Applications:
        DBMS ensures data consistency and integrity, even when multiple applications access the same data.

    Support for Complex Data Types:
        Many modern DBMS systems support complex data types like spatial data, JSON, XML, and more.
        
**The disadvantages of using a DBMS**

Cost:
 Licensing, hardware, and maintenance costs associated with a DBMS can be substantial, particularly for enterprise-level systems.

Complexity:
 DBMS systems can be complex to set up, configure, and maintain. This complexity may require specialized knowledge and training.

Performance Overhead:
 DBMS systems introduce some level of performance overhead due to their various components and layers, which can impact response times.

Data Privacy and Compliance:
         Organizations need to ensure compliance with data privacy regulations (e.g., GDPR, HIPAA), which can be more complex when using a DBMS.

Vendor Lock-In:
 Some DBMS systems may lead to vendor lock-in, making it challenging to switch to a different system without significant effort and cost.

Resource Intensive:
   DBMS systems require significant computational and memory resources, which can be demanding on hardware infrastructure.
 
Data Security Concerns:
 While DBMS systems offer security features, they are not immune to security breaches. Protecting the database from 
 unauthorized access remains a significant challenge.

 
## 1 write cosnstraints of sql
_CODE:_
```sql
Create table Student
    -> (
    -> sid int,
    -> Name varchar(30),
    -> rollno int,
    -> city varchar(50),
    -> fees decimal(18.2)
    -> );


```
![Screenshot from 2023-10-12 15-43-52](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/0a6fd2e1-895b-461a-b0dd-72f41938a6d7)

### i) Default Constraint - The DEFAULT constraint is used to set a default value for a column.The default value will be added to all new records, if no other value is specified.

_CODE:_
```sql
CREATE TABLE Colleges(
   ->    college_id INT PRIMARY KEY,
    ->   college_code VARCHAR(20),
    ->   college_country VARCHAR(20) DEFAULT 'US'
    -> );
INSERT INTO Colleges (college_id, college_code)
    -> VALUES (1, 'ARP76');
INSERT INTO Colleges (college_id, college_code, college_country)
    -> VALUES (2, 'JWS89', 'INDIA');
```

![DEFAULT CONSTRAINT](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/2eed8229-2f12-4767-8e75-a9c943ddd8a9)




ii) **NOT NULL** -The NOT NULL constraint enforces a column to NOT accept NULL values. This enforces a field to always contain  constraint]a value, which means that you cannot insert a new record, or update a record without adding a value to this field.


![NOT NULL constraint](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/26a30270-aeb9-4e04-9793-4d972d58930b)





iii) **PRIMARY CONSTRAINT** - The PRIMARY KEY constraint uniquely identifies each record in a table.Primary keys must contain UNIQUE values, and cannot contain NULL values.A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).

![primary constraint](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/56623791-42b1-4144-87ba-5ffda5cfe02a)





iv) **UNIQUE CONSTRAINT**- The UNIQUE constraint ensures that all values in a column are different.Both the UNIQUE and PRIMARY KEY constraints provide a guarantee for uniqueness for a column or set of columns.

![unique constraint](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/f34049cd-7839-4784-a870-afb30fa2befd)




### 2 **OPERATORS** - An operator is a keyword in SQL that helps us to access the data and returns the result based on the operator's functionality.

i) **AIRTHMETIC OPERATOR** - The SQL Addition Operator performs the addition on the numerical columns in the table. 
    
_CODE:_
```sql
SELECT empsalary + 20000 as empnew_salary FROM emp;
```

![airth operator](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/2b3cd6ba-f554-49ab-a0db-5a75f827afbe)





II) **COMPARISON OPERATOR** - The comparison operator compare two different data whether they are greater , same or lesser and uses WHERE clause

_CODE:_
```sql
`select empsalary * 2 as emp_new_salary from  emp;
```


![compare operator](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/2f21857f-a89e-42cc-a5b9-a727cdc57fe5)




iii) **DIVIDE OPERATOR** - The SQL Division operator divides the numerical values of one column by the numerical values of another column.
_CODE:_
```Sql
SELECT Car_Price / Car_Amount AS One_Car_Price FROM Cars;  
```
![f divide op](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/b47f63c3-e9a5-40ae-8f1e-82d269a9b1a2)





IV) **MULTIPLICATION OPERATOR** - The multiplication operator (*) can also be used with the WHERE clause in the SELECT query. 

_CODE:_
```sql
  select empsalary * 2 as emp_new_salary from  emp;
```

![multply operator](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/41572c75-77b4-44ce-a67d-734b29d5766c)






### B) JOINS  - A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

I) **EQUI JOIN**-  When two tables joined togethet using equality of values.

_CODE:_
```sql
select students.admission_no , name , fees.course, fees.amount_paid from students INNER JOIN fees ON students.admission_no = fees.admission_no;

```

![inner join](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/0fc3e4e7-8a7e-4e7d-9272-40027f4700dd)




 ii)  **LEFT OUTER JOIN** - The LEFT JOIN keyword returns all records from the left table (table1), and the matching records from the right table (table2). The result is 0 records from the right side, if there is no match.

_CODE:_
```sql
select students.admission_no , name , fees.course, fees.amount_paid from students LEFTOUTER JOIN fees ON students.admission_no = fees.admission_no;
```

![left outer join](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/9c63480a-7fb9-43eb-b21c-2d84009841ac)






iii) **RIGHT OUTER JOIN**- The RIGHT JOIN keyword returns all records from the right table (table2), and the matching records from the left table (table1). The result is 0 records from the left side, 

_CODE:_
```sql
select students.admission_no , name , fees.course, fees.amount_paid from students RIGHT  OUTER JOIN fees ON students.admission_no = fees.admission_no;
```

![RIHGHT JOIN](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/7b5f99ae-d190-4798-a7cd-11af12c650bb)





iv) **CROSS JOIN** - A cross join returns the Cartesian product of rows from the rowsets in the join. 

_CODE:_
```sql
select students.admission_no , name , fees.course, fees.amount_paid from students CROSS JOIN fees WHERE students.admission_no = fees.admission_no;
```
![cross join](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/7aad0219-47c7-4d61-a8e1-61b8b7e01fe4)






### 3  VIEW - In SQL, a view is a virtual table based on the result-set of an SQL statement. A view contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

_CODE:_
```sql
 create view emp_view as select * from emp;
       select * from emp_view;
```

![views](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/85c05289-4c0e-4b60-90ee-112f88f3dc9a)





ii) **JOIN VIEW**
    _CODE:_
```sql
select * from Orders;
select * from Customers ;
CREATE VIEW Customer_Vi AS Select DISTINCT first_name FROM Customers c INNER JOIN Orders  ON Order_id = id;
select * from Customer_Vi;
```

![JOIN_VIEW](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/dbc20d80-b312-49da-8ac6-ccf3d3ceca14)




### 4 PL/SQL - The purpose of PL/SQL is to combine database language and procedural programming language. The basic unit in PL/SQL is called a block and is made up of three parts: a declarative part, an executable part and an exception-building part.

![IF PL SQL](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/4f98f80a-7ce5-40ad-9a18-ea263a245f91)





ii) **IF-THEN-ELSE IF**
    
![nested if plsq](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/487d8463-fe43-4bfe-acf3-16b3b2c2df14)




### 5) EXCEPTION HANDLING - An exception is a PL/SQL error that is raised during program execution, either implicitly by TimesTen or explicitly by your program. Handle an exception by trapping it with a handler or propagating it to the calling environment.

![exception ](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/26a30d71-f683-4ff9-bf6a-41b4a5096e46)





### 6) CURSORS - A cursor is a structure that allows you to go over records sequentially, and perform processing based on the result.Cursors are created with a DECLARE CURSOR statement and opened with an OPEN statement. Rows are read with a FETCH statement before the cursor is finally closed with a CLOSE statement.When FETCH is issued and there are no more rows to extract, the following error is produced.


![CURSORS](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/fca1ebc6-9c8d-4fef-8b8f-60719d9fabfa)





### 6) STORED PROCEDURE - A stored procedure is a set of Structured Query Language (SQL) statements with an assigned name, which are stored in a relational database management system (RDBMS) as a group, so it can be reused and shared by multiple programs.



![procedure 1](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/e97b9444-ced5-495b-921b-bd4a9222ce8e)




 ii) FUNCTIONS - MySQL Functions ; MySQL String Functions · ASCII, Returns the ASCII value for the specific character. CHAR_LENGTH.

 ![FUNCTION](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/2bc50f1b-a53e-4bdf-867e-990616cb8135)
 
 



 
 ### 7) TRIGGERS -  An SQL trigger is a database object that is associated with a table and automatically executes a set of SQL statements when a specific event occurs on that table. 

 ![TRIGGER](https://github.com/kaushkis/rdbms_2023batch/assets/147362653/6dea14fc-a9f3-48f1-a193-939b04dd5be9)




