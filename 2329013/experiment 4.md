                                           Experiment:-4
                         View data in the required form using Operators, Functions and Joins 
Structured Query Language is a computer language that we use to interact with a relational database.
In this article we will see all types of SQL operators. 
In simple operator can be defined as an entity used to perform operations in a table.
Operators are the foundation of any programming language. We can define operators as symbols that help us to perform specific mathematical and logical computations on operands. In other words, we can say that an operator operates the operands. SQL operators have three different categories.
 
Arithmetic Operators:-
We can use various arithmetic operators on the data stored in the tables. Arithmetic Operators are:
Operator	Description:-
+	The addition is used to perform an addition operation on the data values.
–	This operator is used for the subtraction of the data values.
/	This operator works with the ‘ALL’ keyword and it calculates division operations.
*	This operator is used for multiplying data values.
%	Modulus is used to get the remainder when data is divided by another.

Example Query:

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/37966a33-5f1a-48d5-8206-be8f81e82119)

Comparison Operators:-
Another important operator in SQL is a comparison operator, which is used to compare one expression’s value to other expressions. SQL supports different types of comparison operator, which is described below:
Operator	Description
=	Equal to.
>	Greater than.
<	Less than.
>=	Greater than equal to.
<=	Less than equal to.
<>	Not equal to.


Example Query:

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/8fe180ad-1f28-46e8-9ddf-f360b70eb0db)

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/924f29e1-e34b-4e05-82b8-a47d299103af)


Logical Operators:-
The Logical operators are those that are true or false. They return true or false values to combine one or more true or false values.
Operator	Description
AND:-
Logical AND compares two Booleans as expressions and returns true when both expressions are true.
OR:-
Logical OR compares two Booleans as expressions and returns true when one of the expressions is true.
NOT:-
Not takes a single Boolean as an argument and change its value from false to true or from true to false.

Example query:-


![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/bac402a7-6061-439a-928f-043350dc6d65)


Special Operators
Operators              	Description 
ALL 
ALL is used to select all records of a SELECT STATEMENT. It compares a value to every value in a list of results from a query. The ALL must be preceded by the comparison operators and evaluated to TRUE if the query returns no rows.
ANY
ANY compares a value to each value in a list of results from a query and evaluates to true if the result of an inner query contains at least one row.
BETWEEN
The SQL BETWEEN operator tests an expression against a range. The range consists of a beginning, followed by an AND keyword and an end expression.
IN
The IN operator checks a value within a set of values separated by commas and retrieves the rows from the table that match.
EXISTS
The EXISTS checks the existence of a result of a subquery. The EXISTS subquery tests whether a subquery fetches at least one row. When no data is returned then this operator returns ‘FALSE’.  
SOME
SOME operator evaluates the condition between the outer and inner tables and evaluates to true if the final result returns any one row. If not, then it evaluates to false.
Example Query:

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/da9904f5-4cd6-4bc4-be10-151ec1d32f2c)

SQL | Functions (Aggregate and Scalar Functions)
For doing operations on data SQL has many built-in functions, they are categorized in two categories and further sub-categorized in different seven functions under each category. The categories are: 
1.	Aggregate functions: 
These functions are used to do operations from the values of the column and a single value is returned. 
1.	AVG()
2.	COUNT()
3.	FIRST()
4.	LAST()
5.	MAX()
6.	MIN()
7.	SUM()
2.	Scalar functions: 
These functions are based on user input, these too returns single value. 
1.	UCASE()
2.	LCASE()
3.	MID()
4.	LEN()
5.	ROUND()
6.	NOW()
7.	FORMAT()

   
![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/1460029b-239f-4e5c-8404-c04819bab821)

•	AVG(): It returns the average value after calculating from values in a numeric column. 

Syntax: 

SELECT AVG(column_name) FROM table_name;
Queries: 
•	Computing average marks of students. 

SELECT AVG(MARKS) AS AvgMarks FROM s_Details

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/cfd20006-ed36-4f5d-93d7-449ae2bb999b)

COUNT(): It is used to count the number of rows returned in a SELECT statement. It can’t be used in MS ACCESS. 
Syntax: 
SELECT COUNT(column_name) FROM table_name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/629f1738-533d-4bee-8054-19634f271892)

MAX(): The MAX() function returns the maximum value of the selected column. 

Syntax: 
SELECT MAX(column_name) FROM table_name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/51701097-093c-4ad2-a711-631e895545f1)

MIN(): The MIN() function returns the minimum value of the selected column. 

Syntax: 
SELECT MIN(column_name) FROM table_name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/30b2fa49-1b8e-4a03-b563-80ffa95eb151)


SUM(): The SUM() function returns the sum of all the values of the selected column.
 Syntax: 
SELECT SUM(column_name) FROM table_name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/ae648f78-5a01-4522-827e-1f58031ef4ed)

LEN(): The LEN() function returns the length of the value in a text field. 

Syntax: 
SELECT LENGTH(column_name) FROM table_name;

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/a98a1c51-57bd-4004-8bdb-a50b7cd7bd1f)

SQL Join:- SQL Join statement is used to combine data or rows from two or more tables based on a common field between them. Different types of Joins are as follows: 
•	INNER JOIN
•	LEFT JOIN
•	RIGHT JOIN
•	FULL JOIN
•	NATURAL JOIN 
SQL JOIN Syntax
The syntax of the SQL JOIN statement is:
SELECT columns_ from _both_ tables
FROM table1
JOIN table2
ON table1.column1 = table2.column



 SQL JOIN
 
 ![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/c22528e2-d79e-4a34-b61f-7ca74ea09a6b)


![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/1484d211-aeaf-4003-98b6-d7f88d541256)


-![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/8b6fdca0-2804-4ba1-9e34-95b0e65ebf2f)

































