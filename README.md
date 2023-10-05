# <p align="center">Assignment of RDBMS</p>
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
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.
