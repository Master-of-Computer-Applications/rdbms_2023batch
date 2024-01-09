                            Experiment-3:
  How to apply constraints at various levels:
SQL Constraints:-
SQL Constraints are the rules applied to a data columns or the complete table to limit the type of data that can go
into a table. When you try to perform any INSERT, UPDATE, or DELETE operation on the table, RDBMS will
check whether that data violates any existing constraints and if there is any violation between the defined constraint
and the data action, it aborts the operation and returns an error.

We can define a column level or a table level constraints. The column level constraints are applied only to one
column, whereas the table level constraints are applied to the whole table.

SQL Create Constraints:-
We can create constraints on a table at the time of a table creation using the CREATE TABLE statement, or after the
table is created, we can use the ALTER TABLE statement to create or delete table constraints.


NOT NULL Constraint:-
When applied to a column, NOT NULL constraint ensure that a column cannot have a NULL value. Following is
the example to create a NOT NULL constraint


![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/2b014f0b-22a4-4cef-a50d-2ec40806e38d)


UNIQUE Key Constraint:-
When applied to a column, UNIQUE Key constraint ensure that a column accepts only UNIQUE values. Following
is the example to create a UNIQUE Key constraint on column ID. Once this constraint is created, column ID can't be
null and it will accept only UNIQUE values.


![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/d94aedbd-cb3b-4858-9509-860d9e62fb9f)


DEFAULT Value Constraint:-
When applied to a column, DEFAULT Value constraint provides a default value for a column when none is
specified. Following is the example to create a DEFAULT constraint on column NAME. Once this constraint is
created, column NAME will set to "Not Available" value if NAME is not set to a value.

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/38f93d00-e153-4e60-ad2b-869ffd2952f9)


PRIMARY Key Constraint:-
When applied to a column, PRIMARY Key constraint ensure that a column accepts only UNIQUE value and there
can be a single PRIMARY Key on a table but multiple columns can constituet a PRIMARY Key. Following is the
example to create a PRIMARY Key constraint on column ID. Once this constraint is created, column ID can't be
null and it will accept only unique values.

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/2265f29b-bb85-4b71-9e7a-779be6eb8c49)

CHECK Value Constraint:-
When applied to a column, CHECK Value constraint works like a validation and it is used to check the validity of
the data entered into the particular column of the table. table and uniquely identifies a row/record in that table.
Following is an example to create a CHECK validation on AGE column which will not accept if its value is below
to 18.

![image](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/86ab27b0-ab82-451b-b191-fcff7167eaed)








