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

•	In this example we will create a View named s_detailsView from the table s_details

Query:

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/3363cef9-5185-42f5-a1aa-3bc979e02fc7)
Creating View from multiple tables: In this example we will create a View named MarksView from two tables StudentDetails and StudentMarks. To create a View from multiple tables we can simply include multiple tables in the SELECT statement.

SQL Updating a View
A view can be updated with the CREATE OR REPLACE VIEW statement.
SQL CREATE OR REPLACE VIEW
 Syntax:-
CREATE OR REPLACE VIEW  view_ name AS
SELECT column1,  column2, ...
FROM  table_ name
WHERE condition;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/dfdc6bb1-f383-40a5-90d5-32f549722123)
Dropping a view:-
Syntax:- DROP VIEW  view _ name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/7c5c4c1f-a186-4a36-b362-08fdc33a4d51)

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

The query is follows:-
SELECT MAX(salary) AS max_salary
FROM(SELECT salary
FROM employee_details) AS max_salary;
After executing above query ;

Max_salary
45000.00
OUTPUT IS:
Max_salary
45000.00


















