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
![rdbms 4 pic](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/711b08d1-7515-4a45-9b48-9716dc0c4a1f)

NOT NULL Constraint:-
When applied to a column, NOT NULL constraint ensure that a column cannot have a NULL value. Following is
the example to create a NOT NULL constraint
![rdbms 5 pic](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/7aebe436-cb9e-4163-a229-1d603882ea23)

UNIQUE Key Constraint:-
When applied to a column, UNIQUE Key constraint ensure that a column accepts only UNIQUE values. Following
is the example to create a UNIQUE Key constraint on column ID. Once this constraint is created, column ID can't be
null and it will accept only UNIQUE values.
![rdbms pic 6](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/20da890b-d8db-4d68-a7ef-710dde11ffee) 

DEFAULT Value Constraint:-
When applied to a column, DEFAULT Value constraint provides a default value for a column when none is
specified. Following is the example to create a DEFAULT constraint on column NAME. Once this constraint is
created, column NAME will set to "Not Available" value if NAME is not set to a value.
![rdbms pic 7](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/aa630441-ce78-4f53-94b7-0968d753b26c) 

PRIMARY Key Constraint:-
When applied to a column, PRIMARY Key constraint ensure that a column accepts only UNIQUE value and there
can be a single PRIMARY Key on a table but multiple columns can constituet a PRIMARY Key. Following is the
example to create a PRIMARY Key constraint on column ID. Once this constraint is created, column ID can't be
null and it will accept only unique values.
![rdbms pic 8](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/f0780c58-366d-4677-be35-a52beafd6d97)

CHECK Value Constraint:-
When applied to a column, CHECK Value constraint works like a validation and it is used to check the validity of
the data entered into the particular column of the table. table and uniquely identifies a row/record in that table.
Following is an example to create a CHECK validation on AGE column which will not accept if its value is below
to 18.
![rdbms pic 9](https://github.com/manvirsinghh/rdbms_2023batch/assets/147043473/41957e43-93b8-4186-bdfe-3053e31573b7)







