# <p align="center">Assignment 1 of RDMBS</p>
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
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 # <p align="center">Assignment 2 </p>

 # <p align="center">1-Codd Rules.</p>                                                           
 Rule 0: The Foundation Rule:-
The database must be in relational form. So that the system can handle the database through its relational capabilities.

Rule 1: Information Rule:-
A database contains various information, and this information must be stored in each cell of a table in the form of rows and columns.

Rule 2: Guaranteed Access Rule:-
Every single or precise data (atomic value) may be accessed logically from a relational database using the combination of primary key value, table name, and column name.

Rule 3: Systematic Treatment of Null Values:-
This rule defines the systematic treatment of Null values in database records. The null value has various meanings in the database, like missing the data, no value in a cell, inappropriate information, unknown data and the primary key should not be null.

Rule 4: Active/Dynamic Online Catalog based on the relational model:-
It represents the entire logical structure of the descriptive database that must be stored online and is known as a database dictionary. It authorizes users to access the database and implement a similar query language to access the database.

Rule 5: Comprehensive Data SubLanguage Rule:-
The relational database supports various languages, and if we want to access the database, the language must be the explicit, linear or well-defined syntax, character strings and supports the comprehensive: data definition, view definition, data manipulation, integrity constraints, and limit transaction management operations. If the database allows access to the data without any language, it is considered a violation of the database.

Rule 6: View Updating Rule:-
All views table can be theoretically updated and must be practically updated by the database systems.

Rule 7: Relational Level Operation (High-Level Insert, Update and delete) Rule:-
A database system should follow high-level relational operations such as insert, update, and delete in each level or a single row. It also supports union, intersection and minus operation in the database system.

Rule 8: Physical Data Independence Rule:-
All stored data in a database or an application must be physically independent to access the database. Each data should not depend on other data or an application. If data is updated or the physical structure of the database is changed, it will not show any effect on external applications that are accessing the data from the database.

Rule 9: Logical Data Independence Rule:-
It is similar to physical data independence. It means, if any changes occurred to the logical level (table structures), it should not affect the user's view (application). For example, suppose a table either split into two tables, or two table joins to create a single table, these changes should not be impacted on the user view application.

Rule 10: Integrity Independence Rule:-
A database must maintain integrity independence when inserting data into table's cells using the SQL query language. All entered values should not be changed or rely on any external factor or application to maintain integrity. It is also helpful in making the database-independent for each front-end application.

Rule 11: Distribution Independence Rule:-
The distribution independence rule represents a database that must work properly, even if it is stored in different locations and used by different end-users. Suppose a user accesses the database through an application; in that case, they should not be aware that another user uses particular data, and the data they always get is only located on one site. The end users can access the database, and these access data should be independent for every user to perform the SQL queries.

Rule 12: Non Subversion Rule:-
The non-submersion rule defines RDBMS as a SQL language to store and manipulate the data in the database. If a system has a low-level or separate language other than SQL to access the
database system, it should not subvert or bypass integrity to transform data.


                                                       ANOMALIES IN DATABASE
Anomaly means inconsistency in the pattern from the normal form. In Database Management System (DBMS), anomaly means the inconsistency occurred in the relational table during the operations performed on the relational table.

There can be various reasons for anomalies to occur in the database. For example, if there is a lot of redundant data present in our database then DBMS anomalies can occur. If a table is constructed in a very poor manner then there is a chance of database anomaly. Due to database anomalies, the integrity of the database suffers.

The other reason for the database anomalies is that all the data is stored in a single table. So, to remove the anomalies of the database, normalization is the process which is done where the splitting of the table and joining of the table (different types of join) occurs.

We will see the anomalies present in a table:-
There can be three types of an anomaly in the database:

Updation / Update Anomaly:-
When we update some rows in the table, and if it leads to the inconsistency of the table then this anomaly occurs. This type of anomaly is known as an updation anomaly. In the above table, if we want to update the address of Ramesh then we will have to update all the rows where Ramesh is present. If during the update we miss any single row, then there will be two addresses of Ramesh, which will lead to inconsistent and wrong databases.

Insertion Anomaly:-
If there is a new row inserted in the table and it creates the inconsistency in the table then it is called the insertion anomaly. For example, if in the above table, we create a new row of a worker, and if it is not allocated to any department then we cannot insert it in the table so, it will create an insertion anomaly.

Deletion Anomaly:-
If we delete some rows from the table and if any other information or data which is required is also deleted from the database, this is called the deletion anomaly in the database. For example, in the above table, if we want to delete the department number ECT669 then the details of Rajesh will also be deleted since Rajesh's details are dependent on the row of ECT669. So, there will be deletion anomalies in the table.

To remove this type of anomalies, we will normalize the table or split the table or join the tables. There can be various normalized forms of a table like 1NF, 2NF, 3NF, BCNF etc. we will apply the different normalization schemes according to the current form of the table.

                                                               NORMAL FORMS:-
Normalization is the process of minimizing redundancy from a relation or set of relations. Redundancy in relation may cause insertion, deletion, and update anomalies. So, it helps to minimize the redundancy in relations. Normal forms are used to eliminate or reduce redundancy in database tables.

Normalization of DBMS:-
In database management systems (DBMS), normal forms are a series of guidelines that help to ensure that the design of a database is efficient, organized, and free from data anomalies. There are several levels of normalization, each with its own set of guidelines, known as normal forms.

 # <p align="center">Differences Between 3NF AND BCNF.</p>

   3NF  |  BCNF  
   |  -----  |  -----|
   It stands for Third Normal Form.|	It stands for Boyce Code Normal Form, .                                               
   It is weaker than BCNF.	|It is stronger than 3NF.
   All the relations which are in 3NF may or may not be in BCNF.|	All the relations that are in BNCF must be in 3NF.
   3NF can be achieved without losing the dependency that is already there.|	The functional dependency may get lost while achieving BCNF form.

   
# <p align="center">Differences Between 4NF AND 5NF.</p>
 4NF |  5NF  
   |   -----   |   -----|
   A relation in 4NF must also be in BCNF.|	A relation in 5NF must also be in 4NF.
   A relation in 4NF must not have any multi-valued dependency.|	A relation in 5NF must not have any join dependency.
   A relation in 4NF may or may not be in 5NF.|	A relation in 5NF is always in 4NF.
   4NF is less stronger in comparison to 5NF.|	5NF is more stronger than 4NF.
   If a relation is in Fourth Normal Form then it will have more redundancy.|	If a relation is in Fifth Normal Form then it will less redundancy.
