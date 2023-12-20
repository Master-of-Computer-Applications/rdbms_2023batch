# <p align="center">Assignment of RDBMS</p>
# <p align="left">1-12 CODD RULES.</p>

Rule 1: Information Rule

The data stored in a database, may it be user data or metadata, must be a value of some table cell. Everything in a database must be stored in a table format.

Rule 2: Guaranteed Access Rule

Every single data element (value) is guaranteed to be accessible logically with a combination of table-name, primary-key (row value), and attribute-name (column value). No other means, such as pointers, can be used to access data.

Rule 3: Systematic Treatment of NULL Values

The NULL values in a database must be given a systematic and uniform treatment. This is a very important rule because a NULL can be interpreted as one the following − data is missing, data is not known, or data is not applicable.

Rule 4: Active Online Catalog

The structure description of the entire database must be stored in an online catalog, known as data dictionary, which can be accessed by authorized users. Users can use the same query language to access the catalog which they use to access the database itself.

Rule 5: Comprehensive Data Sub-Language Rule

A database can only be accessed using a language having linear syntax that supports data definition, data manipulation, and transaction management operations. This language can be used directly or by means of some application. If the database allows access to data without any help of this language, then it is considered as a violation.

Rule 6: View Updating Rule

All the views of a database, which can theoretically be updated, must also be updatable by the system.

Rule 7: High-Level Insert, Update, and Delete Rule

A database must support high-level insertion, updation, and deletion. This must not be limited to a single row, that is, it must also support union, intersection and minus operations to yield sets of data records.

Rule 8: Physical Data Independence

The data stored in a database must be independent of the applications that access the database. Any change in the physical structure of a database must not have any impact on how the data is being accessed by external applications.

Rule 9: Logical Data Independence

The logical data in a database must be independent of its user’s view (application). Any change in logical data must not affect the applications using it. For example, if two tables are merged or one is split into two different tables, there should be no impact or change on the user application. This is one of the most difficult rule to apply.

Rule 10: Integrity Independence

A database must be independent of the application that uses it. All its integrity constraints can be independently modified without the need of any change in the application. This rule makes a database independent of the front-end application and its interface.

Rule 11: Distribution Independence

The end-user must not be able to see that the data is distributed over various locations. Users should always get the impression that the data is located at one site only. This rule has been regarded as the foundation of distributed database systems.

Rule 12: Non-Subversion Rule

If a system has an interface that provides access to low-level records, then the interface must not be able to subvert the system and bypass security and integrity constraints.

# <p align="left"> DIFFERENCE BETWEEN 3NF AND BCNF</p>

3NF | BCNF
|---|---|
It stands for Third Normal Form.	|It stands for Boyce Code Normal Form.
All the relations which are in 3NF may or may not be in BCNF.|All the relations that are in BNCF must be in 3NF.
It is weaker than BCNF.|It is stronger than 3NF.
The amount of redundant data in 3NF is more than that in BCNF.| In comparison to 3NF, the redundancy is very less in BCNF.
There should be no transitive dependency in 3NF.| It means that no non-prime attribute should be transitively dependent on the candidate key.	In BCNF, for any given relation C → D, C should be a super key.
3NF can be achieved without losing the dependency that is already there.| The functional dependency may get lost while achieving BCNF form.


# <p align="left"> DIFFERENCE BETWEEN 4NF AND 5NF</p>
4NF | 5NF
|---|---|
A relation in 4NF must also be in BCNF(Boyce Codd Normal Form).	|A relation in 5NF must also be in 4NF(Fourth Normal Form).
A relation in 4NF must not have any multi-valued dependency.|A relation in 5NF must not have any join dependency.
A relation in 4NF may or may not be in 5NF.|A relation in 5NF is always in 4NF
Fourth Normal Form is less stronger in comparison to Fifth Normal form.|Fifth Normal form is more stronger than Fourth Normal Form.
If a relation is in Fourth Normal Form then it will have more redundancy. | f a relation is in Fifth Normal Form then it will less redundancy.
If a relation is in Fourth Normal Form then it may be decomposed further into sub-relations.|If a relation is in Fifth Normal Form then it cannot be decomposed further into sub-relations without any modification in meaning or facts.

# <p align="left"> NORMALIZATION</p>

Normalization is the process of minimizing redundancy from a relation or set of relations. Redundancy in relation may cause insertion, deletion, and update anomalies. So, it helps to minimize the redundancy in relations. Normal forms are used to eliminate or reduce redundancy in database tables.

Normalization of DBMS
In database management systems (DBMS), normal forms are a series of guidelines that help to ensure that the design of a database is efficient, organized, and free from data anomalies. There are several levels of normalization, each with its own set of guidelines, known as normal forms.

Important Points Regarding Normal Forms in DBMS
First Normal Form (1NF): This is the most basic level of normalization. In 1NF, each table cell should contain only a single value, and each column should have a unique name. The first normal form helps to eliminate duplicate data and simplify queries.
Second Normal Form (2NF): 2NF eliminates redundant data by requiring that each non-key attribute be dependent on the primary key. This means that each column should be directly related to the primary key, and not to other columns.
Third Normal Form (3NF): 3NF builds on 2NF by requiring that all non-key attributes are independent of each other. This means that each column should be directly related to the primary key, and not to any other columns in the same table.
Boyce-Codd Normal Form (BCNF): BCNF is a stricter form of 3NF that ensures that each determinant in a table is a candidate key. In other words, BCNF ensures that each non-key attribute is dependent only on the candidate key.
Fourth Normal Form (4NF): 4NF is a further refinement of BCNF that ensures that a table does not contain any multi-valued dependencies.
Fifth Normal Form (5NF): 5NF is the highest level of normalization and involves decomposing a table into smaller tables to remove data redundancy and improve data integrity.
Normal forms help to reduce data redundancy, increase data consistency, and improve database performance. However, higher levels of normalization can lead to more complex database designs and queries. It is important to strike a balance between normalization and practicality when designing a database.

Advantages of Normal Form
Reduced data redundancy: Normalization helps to eliminate duplicate data in tables, reducing the amount of storage space needed and improving database efficiency.
Improved data consistency: Normalization ensures that data is stored in a consistent and organized manner, reducing the risk of data inconsistencies and errors.
Simplified database design: Normalization provides guidelines for organizing tables and data relationships, making it easier to design and maintain a database.
Improved query performance: Normalized tables are typically easier to search and retrieve data from, resulting in faster query performance.
Easier database maintenance: Normalization reduces the complexity of a database by breaking it down into smaller, more manageable tables, making it easier to add, modify, and delete data.

Applications of Normal Forms in DBMS
Data consistency: Normal forms ensure that data is consistent and does not contain any redundant information. This helps to prevent inconsistencies and errors in the database.
Data redundancy: Normal forms minimize data redundancy by organizing data into tables that contain only unique data. This reduces the amount of storage space required for the database and makes it easier to manage.
Response time: Normal forms can improve query performance by reducing the number of joins required to retrieve data. This helps to speed up query processing and improve overall system performance.
Database maintenance: Normal forms make it easier to maintain the database by reducing the amount of redundant data that needs to be updated, deleted, or modified. This helps to improve database management and reduce the risk of errors or inconsistencies.
Database design: Normal forms provide guidelines for designing databases that are efficient, flexible, and scalable. This helps to ensure that the database can be easily modified, updated, or expanded as needed.

Some Important Points about Normal Forms
BCNF is free from redundancy caused by Functional Dependencies.
If a relation is in BCNF, then 3NF is also satisfied.
 If all attributes of relation are prime attribute, then the relation is always in 3NF.
A relation in a Relational Database is always and at least in 1NF form.
Every Binary Relation ( a Relation with only 2 attributes ) is always in BCNF.
If a Relation has only singleton candidate keys( i.e. every candidate key consists of only 1 attribute), then the Relation is always in 2NF( because no Partial functional dependency possible).
Sometimes going for BCNF form may not preserve functional dependency. In that case go for BCNF only if the lost FD(s) is not required, else normalize till 3NF only.
There are many more Normal forms that exist after BCNF, like 4NF and more. But in real world database systems it’s generally not required to go beyond BCNF.
