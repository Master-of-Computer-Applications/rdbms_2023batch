NAME - Sukhpreet Singh
<br>CRN - 2329021
<br>ASSIGNMENT - 2
<br>QUESTION :- Normalization and Codd's rules for RDBMS

# <p align="left">Normalization</p>
### Normalization
A large database defined as a single relation may result in data duplication. This repetition of data may result in:

* Making relations very large.
* It isn't easy to maintain and update data as it would involve searching many records in relation.
* Wastage and poor utilization of disk space and resources.
* The likelihood of errors and inconsistencies increases.

So to handle these problems, we should analyze and decompose the relations with redundant data into smaller, simpler, and well-structured relations that are satisfy desirable properties. Normalization is a process of decomposing the relations into relations with fewer attributes.

### Types of Normal Forms
![image](https://github.com/sukhlotey/rdbms_2023batch/assets/82471879/4afbe9cf-47ea-4f33-b117-a33bc53c64c1)


| Normal Form   | Description |
| ------------- | ------------- |
|1NF  | A relation is in 1NF if it contains an atomic value.  |
|2NF  | A relation will be in 2NF if it is in 1NF and all non-key attributes are fully functional dependent on the primary key.  |
|3NF  |A relation will be in 3NF if it is in 2NF and no transition dependency exists.  |
|BCNF  | A stronger definition of 3NF is known as Boyce Codd's normal form.  |
|4NF  | A relation will be in 4NF if it is in Boyce Codd's normal form and has no multi-valued dependency.  |
|5NF  | A relation is in 5NF. If it is in 4NF and does not contain any join dependency, joining should be lossless.  |

<hr>

# <p align="left">Codd's Rules For RDBMS</p>
Codd’s rules are proposed by a computer scientist named Dr. Edgar F. Codd and he also invent the relational model for database management. These rules are made to ensure data integrity, consistency, and usability. This set of rules basically signifies the characteristics and requirements of a relational database management system (RDBMS). In this article, we will learn about various Codd’s rules.

### Rule 1: The Information Rule
All information, whether it is user information or metadata, that is stored in a database must be entered as a value in a cell of a table. It is said that everything within the database is organized in a table layout.

### Rule 2: The Guaranteed Access Rule
Each data element is guaranteed to be accessible logically with a combination of the table name, primary key (row value), and attribute name (column value). 

### Rule 3: Systematic Treatment of NULL Values
Every Null value in a database must be given a systematic and uniform treatment. 

### Rule 4: Active Online Catalog Rule
The database catalog, which contains metadata about the database, must be stored and accessed using the same relational database management system.

### Rule 5: The Comprehensive Data Sublanguage Rule
A crucial component of any efficient database system is its ability to offer an easily understandable data manipulation language (DML) that facilitates defining, querying, and modifying information within the database.

### Rule 6: The View Updating Rule
All views that are theoretically updatable must also be updatable by the system.

### Rule 7: High-level Insert, Update, and Delete
A successful database system must possess the feature of facilitating high-level insertions, updates, and deletions that can grant users the ability to conduct these operations with ease through a single query.

### Rule 8: Physical Data Independence
Application programs and activities should remain unaffected when changes are made to the physical storage structures or methods.

### Rule 9: Logical Data Independence 
Application programs and activities should remain unaffected when changes are made to the logical structure of the data, such as adding or modifying tables.

### Rule 10: Integrity Independence
Integrity constraints should be specified separately from application programs and stored in the catalog. They should be automatically enforced by the database system.

### Rule 11: Distribution Independence
The distribution of data across multiple locations should be invisible to users, and the database system should handle the distribution transparently.

### Rule 12: Non-Subversion Rule
If the interface of the system is providing access to low-level records, then the interface must not be able to damage the system and bypass security and integrity constraints.

