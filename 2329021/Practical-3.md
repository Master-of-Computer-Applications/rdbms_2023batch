NAME - Sukhpreet Singh
<br>CRN - 2329021
<br>PRACTICAL - 3
<br>QUESTION :- How to apply Constraints at various levels.

# Introduction
<p>
  SQL constraints can be at a column or a table level. Column level constraints apply to specific columns in a table and do not specify a column name except the check constraints. They refer to the column that they follow. The names are specified by the Table-level constraints of the columns to which they apply.
</p>

## The available constraints in SQL are: 

* <b>NOT NULL:</b> This constraint tells that we cannot store a null value in a column. That is, if a column is specified as NOT NULL then we will not be able to store null in this particular column any more.
* <b>UNIQUE:</b> This constraint when specified with a column, tells that all the values in the column must be unique. That is, the values in any row of a column must not be repeated.
* <b>PRIMARY KEY:</b> A primary key is a field which can uniquely identify each row in a table. And this constraint is used to specify a field in a table as primary key.
* <b>FOREIGN KEY:</b> A Foreign key is a field which can uniquely identify each row in a another table. And this constraint is used to specify a field as Foreign key.
* <b>CHECK: </b> This constraint helps to validate the values of a column to meet a particular condition. That is, it helps to ensure that the value stored in a column meets a specific condition.
* <b>DEFAULT:</b> This constraint specifies a default value for the column when no value is specified by the user.

### Syntax:
<p>
  Below is the syntax to create constraints using CREATE TABLE statement at the time of creating the table. 
</p>

CREATE TABLE sample_table
<br>(
<br>column1 data_type(size) constraint_name,
<br>column2 data_type(size) constraint_name,
<br>column3 data_type(size) constraint_name,
<br>....
<br>);

sample_table: Name of the table to be created.
<br>data_type: Type of data that can be stored in the field.
<br>constraint_name: Name of the constraint. for example- NOT NULL, UNIQUE, PRIMARY KEY etc. 
