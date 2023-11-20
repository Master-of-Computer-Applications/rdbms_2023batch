# <p align="center">Assignment of RDBMS </p>
### <p align="left"> Ques1:- Write down the Codd's rules in Rdbms? <p>
 **Ans:-** Codd’s rules are proposed by a computer scientist named Dr. Edgar F. Codd and he also invent the relational model for database management. These rules are made to ensure data integrity, consistency, and usability. This set of rules basically signifies the characteristics and requirements of a relational database management system (RDBMS).

<ins> ***Codd’s Rules in DBMS:-***

**Rule 1: The Information Rule**<br>
All information, whether it is user information or metadata, that is stored in a database must be entered as a value in a cell of a table. It is said that everything within the database is organized in a table layout.

**Rule 2: The Guaranteed Access Rule**<br>
Each data element is guaranteed to be accessible logically with a combination of the table name, primary key (row value), and attribute name (column value). 

**Rule 3: Systematic Treatment of NULL Values**<br>
Every Null value in a database must be given a systematic and uniform treatment. 

**Rule 4: Active Online Catalog Rule**<br>
The database catalog, which contains metadata about the database, must be stored and accessed using the same relational database management system.

**Rule 5: The Comprehensive Data Sublanguage Rule**<br>
A crucial component of any efficient database system is its ability to offer an easily understandable data manipulation language (DML) that facilitates defining, querying, and modifying information within the database.

**Rule 6: The View Updating Rule**<br>
All views that are theoretically updatable must also be updatable by the system.

**Rule 7: High-level Insert, Update, and Delete**<br>
A successful database system must possess the feature of facilitating high-level insertions, updates, and deletions that can grant users the ability to conduct these operations with ease through a single query.

**Rule 8: Physical Data Independence**<br>
Application programs and activities should remain unaffected when changes are made to the physical storage structures or methods.

**Rule 9: Logical Data Independence**<br>
Application programs and activities should remain unaffected when changes are made to the logical structure of the data, such as adding or modifying tables.

**Rule 10: Integrity Independence**<br>
Integrity constraints should be specified separately from application programs and stored in the catalog. They should be automatically enforced by the database system.

**Rule 11: Distribution Independence**<br>
The distribution of data across multiple locations should be invisible to users, and the database system should handle the distribution transparently.

**Rule 12: Non-Subversion Rule**<br>
If the interface of the system is providing access to low-level records, then the interface must not be able to damage the system and bypass security and integrity constraints.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align="left"> Ques2:- Explain anomalies in database? <p>
**Ans:-** Anomalies in the relational model refer to inconsistencies or errors that can arise when working with relational databases, specifically in the context of data insertion, deletion, and modification. There are different types of anomalies that can occur in referencing and referenced relations.

**These anomalies can be categorized into three types:-**

   *1) Insertion Anomalies*<br>
   *2) Deletion Anomalies*<br>
   *3) Update Anomalies.*<br>

**1) Insertion anomaly:-** If a tuple is inserted in referencing relation and referencing attribute value is not present in referenced attribute, it will not allow insertion in referencing relation. <br>
Example: If we try to insert a record in STUDENT_COURSE with STUD_NO =7, it will not allow it. 

**2) Deletion and Updation anomaly:-** If a tuple is deleted or updated from referenced relation and the referenced attribute value is used by referencing attribute in referencing relation, it will not allow deleting the tuple from referenced relation.<br>
Example: If we want to update a record from STUDENT_COURSE with STUD_NO =1, We have to update it in both rows of the table. If we try to delete a record from STUDENT with STUD_NO =1, it will not allow it. <br>

**Accurance of anomalies:-**

   **1) Insertion Anomalies:-** These anomalies occur when it is not possible to insert data into a database because the required fields are missing or because the data is incomplete. For example, if a database requires that every record has a primary key, but no value is provided for a particular record, it cannot be inserted into the database.<br>
   
   **2) Deletion anomalies:-** These anomalies occur when deleting a record from a database and can result in the unintentional loss of data. For example, if a database contains information about customers and orders, deleting a customer record may also delete all the orders associated with that customer.<br>
   
   **3) Update anomalies:-**  These anomalies occur when modifying data in a database and can result in inconsistencies or errors. For example, if a database contains information about employees and their salaries, updating an employee’s salary in one record but not in all related records could lead to incorrect calculations and reporting.<br>

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align="left"> Ques3:- Explain Normal forms in rdbms? <p>
**Ans:-** **<ins>Normalization of DBMS:-**

In database management systems (DBMS), normal forms are a series of guidelines that help to ensure that the design of a database is efficient, organized, and free from data anomalies. There are several levels of normalization, each with its own set of guidelines, known as normal forms.

**1) First Normal Form (1NF):-** This is the most basic level of normalization. In 1NF, each table cell should contain only a single value, and each column should have a unique name. The first normal form helps to eliminate duplicate data and simplify queries.<br>

**2) Second Normal Form (2NF):** 2NF eliminates redundant data by requiring that each non-key attribute be dependent on the primary key. This means that each column should be directly related to the primary key, and not to other columns.<br>

**3) Third Normal Form (3NF):** 3NF builds on 2NF by requiring that all non-key attributes are independent of each other. This means that each column should be directly related to the primary key, and not to any other columns in the same table.<br>

**4) Boyce-Codd Normal Form (BCNF):-** BCNF is a stricter form of 3NF that ensures that each determinant in a table is a candidate key. In other words, BCNF ensures that each non-key attribute is dependent only on the candidate key.<br>

**5) Fourth Normal Form (4NF):-** 4NF is a further refinement of BCNF that ensures that a table does not contain any multi-valued dependencies.<br>

**6) Fifth Normal Form (5NF):** 5NF is the highest level of normalization and involves decomposing a table into smaller tables to remove data redundancy and improve data integrity.

**<ins>Applications of Normal Forms in DBMS:-**

  **1) Data consistency:-** Normal forms ensure that data is consistent and does not contain any redundant information. This helps to prevent inconsistencies and errors in the database.<br>
  
  **2) Data redundancy:-** Normal forms minimize data redundancy by organizing data into tables that contain only unique data. This reduces the amount of storage space required for the database and makes it easier to manage.<br>
   
  **3) Response time:-** Normal forms can improve query performance by reducing the number of joins required to retrieve data. This helps to speed up query processing and improve overall system performance.<br>
   
  **4) Database maintenance:-** Normal forms make it easier to maintain the database by reducing the amount of redundant data that needs to be updated, deleted, or modified. This helps to improve database management and reduce the risk of errors or inconsistencies.<br>
   
  **5) Database design:-** Normal forms provide guidelines for designing databases that are efficient, flexible, and scalable. This helps to ensure that the database can be easily modified, updated, or expanded as needed.<br>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### <p align="left"> Ques4:- Difference between 3NF and BCNF? <p>
**Ans:-** *1. Third Normal Form (3NF) :-* A relation is said to be in Third Normal Form (3NF), if it is in 2NF and when no non key attribute is transitively dependent on the primary key i.e., there is no transitive dependency. 3NF is used to reduce data duplication and to attain data integrity. 

Also it should satisfy one of the below given conditions. For the function dependency C->D:-<br>
   A) C should be a super key and,<br>
   B) D should be a prime attribute i.e, D should be a part of the candidate key. 

**Example:-** For the relation R(L, M, N, O, P) with functional dependencies as {L->M, MN->P, PO->L}:

The candidate keys will be : {LNO, MNO, NOP}<br>
      as the closure of LNO = {L, M, N, O, P}<br>
             closure of MNO = {L, M, N, O, P}<br>
             closure of NOP = {L, M, N, O, P}

This relation is in 3NF as it is already in 2NF and has no transitive dependency. Also there is no non prime attribute that is deriving a non prime attribute. 

*2. Boyce-Codd Normal Form (BCNF) :-*  BCNF stands for Boyce-Codd normal form and was made by R.F Boyce and E.F Codd in 1974.BCNF is an extension of 3NF and it is has more strict rules than 3NF. Also, it is considered to be more stronger than 3NF. 

A functional dependency is said to be in BCNF if these properties hold:-<br>
A) It should already be in 3NF.<br>
B) For a functional dependency say P->Q, P should be a super key.

**Example:-** for the relation R(A, B, C, D) with functional dependencies as {A->B, A->C, C->D, C->A}:

The candidate keys will be : {A, C}<br>
      as the closure of A = {A, B, C, D}<br> 
             closure of C = {A, B, C, D} 

This relation is in BCNF as it is already in 3Nf (there is no prime attribute deriving no prime attribute) and on the left hand side of the functional dependency there is a candidate key. 

**<ins>Difference between 3NF and BCNF :-**
|S.NO. |	3NF |	BCNF|
|--|--|--|
|1. |	3NF stands for Third Normal Form. |	BCNF stands for Boyce Codd Normal Form. |
|2. |	In 3NF there should be no transitive dependency that is no non prime attribute should be transitively dependent on the candidate key. |	In BCNF for any relation A->B, A should be a super key of relation.|
|3. |	It is less stronger than BCNF. |	It is comparatively more stronger than 3NF.|
|4. |	In 3NF the functional dependencies are already in 1NF and 2NF. |	In BCNF the functional dependencies are already in 1NF, 2NF and 3NF.|
|5. |	The redundancy is high in 3NF. |	The redundancy is comparatively low in BCNF.|
|6. |	In 3NF there is preservation of all functional dependencies. |	In BCNF there may or may not be preservation of all functional dependencies.|
|7. |	It is comparatively easier to achieve. |	It is difficult to achieve.|
|8. |	Lossless decomposition can be achieved by 3NF.| 	Lossless decomposition is hard to achieve in BCNF.|
|9. |	The table is in 3NF if it is in 2NF and for each functional dependency X->Y at least following condition hold: (i) X is a super key, (ii) Y is prime attribute of table.| The table is in BCNF if it is in 3rd normal form and for each relation X->Y X should be super key.|
|10.| 	3NF can be obtained without sacrificing all dependencies. |	Dependencies may not be preserved in BCNF.|
|11.|	3NF can be achieved without losing any information from the old table. |	For obtaining BCNF we may lose some information from old table.|
