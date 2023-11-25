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
