                                 Experiment:-5
                 Creating different types of views for tailored presentation of data
 VIEWS:-Views in SQL are kind of virtual tables. A view also has rows and columns as they are in a real table in the database. 
 We can create a view by selecting fields from one or more tables present in the database. 
 A View can either have all the rows of a table or specific rows based on certain condition
CREATING VIEWS:-
We can create View using CREATE VIEW statement. A View can be created from a single table or multiple tables.

 Syntax:

CREATE VIEW view_name AS
SELECT column1, column2.....
FROM table_name
WHERE condition;
view_name: Name for the View

table_name: Name of the table

condition: Condition to select rows

Examples:

Creating View from a single table:

••	In this example we will create a View named Student123 from the table Student1

Query:

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/eaf78211-2bdf-4bb4-997d-a2992b74459a)

Creating View from multiple tables:  To create a View from multiple tables we can simply include multiple tables in the SELECT statement.

SQL Updating a View
A view can be updated with the CREATE OR REPLACE VIEW statement.
SQL CREATE OR REPLACE VIEW
 Syntax:-
CREATE OR REPLACE VIEW  view_ name AS
SELECT column1,  column2, ...
FROM  table_ name
WHERE condition;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/819c8aa9-4e3e-4760-9b7d-9b0c68b362fa)

Dropping a view:-
Syntax:- DROP VIEW  view _ name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/0827bd68-9b6e-4fc3-999b-403a79fb95c4)


 Types of View:-
 Simple View: A view based on only a single table, which doesn't contain GROUP BY clause and any functions. 
 Complex View: A view based on multiple tables, which contain GROUP BY clause and functions.
 Inline View: A view based on a subquery in FROM Clause, that subquery creates a temporary table and simplifies the complex query.
 Materialized View: A view that stores the definition as well as data. It creates replicas of data by storing it physically
 
INLINE VIEW:-Inline view is select statement in another select statement of from clause. 
Inline view is used to reduce complexity  in queries without using join.


SYNTAX:-
SELECT column1,column2,……. FROM(INLINEVIEW);
QUERY:-
selecting  rows from employee_details by using inline view .

SELECT column1,column2,……. FROM(INLINEVIEW);

MATERIALIZED VIEW:-
A materialized view specifies a cluster that is tasked with keeping its results up-to-date, but can be referenced in any cluster. This allows you to effectively decouple the computational resources used for view maintenance from the resources used for query serving.
Syntax:-
Create materialized view View_Name

Build [Immediate/Deffered]

Refresh [Fast/Complete/Force]

on [Commit/Demand]

as Select ..........;

COMPLEX VIEW:-
When the view is created based on multiple tables then it is known as a complex view in SQL Server. The most important point that we need to remember is, on a complex view in SQL Server, we may or may not perform the DML operations and more ever the complex view may not update the data correctly on the underlying database tables.




















