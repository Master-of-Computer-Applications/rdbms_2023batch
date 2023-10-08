Experiment-3:
How to apply constraints at various levels:

SQL Constraints

SQL Constraints are the rules applied to a data columns or the complete table to limit the type of data that can go into a table. When you try to perform any INSERT, UPDATE, or DELETE operation on the table, RDBMS will check whether that data violates any existing constraints and if there is any violation between the defined constraint and the data action, it aborts the operation and returns an error.
We can define a column level or a table level constraints. The column level constraints are applied only to one column, whereas the table level constraints are applied to the whole table.

SQL Create Constraints

We can create constraints on a table at the time of a table creation using the CREATE TABLE statement, or after the table is created, we can use the ALTER TABLE statement to create or delete table constraints.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/d0e05c8f-a6b9-4291-bf31-6162ee7fc696)

NOT NULL Constraint

When applied to a column, NOT NULL constraint ensure that a column cannot have a NULL value. Following is the example to create a NOT NULL constraint:

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/ff329c97-0084-4cc2-9226-0b055b929aa5)

UNIQUE Key Constraint

When applied to a column, UNIQUE Key constraint ensure that a column accepts only UNIQUE values. Following is the example to create a UNIQUE Key constraint on column ID. Once this constraint is created, column ID can't be null and it will accept only UNIQUE values.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/1bff6769-4d69-4098-92ff-b166d8ab2918)

DEFAULT Value Constraint

When applied to a column, DEFAULT Value constraint provides a default value for a column when none is specified. Following is the example to create a DEFAULT constraint on column NAME. Once this constraint is created, column NAME will set to "Not Available" value if NAME is not set to a value.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/f7210730-6073-4e59-b061-e9dd6912b84b)

PRIMARY Key Constraint

When applied to a column, PRIMARY Key constraint ensure that a column accepts only UNIQUE value and there can be a single PRIMARY Key on a table but multiple columns can constituet a PRIMARY Key. Following is the example to create a PRIMARY Key constraint on column ID. Once this constraint is created, column ID can't be null and it will accept only unique values.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/c0dd0234-b39a-482a-815b-adee9c1ec784)

CHECK Value Constraint

When applied to a column, CHECK Value constraint works like a validation and it is used to check the validity of the data entered into the particular column of the table. table and uniquely identifies a row/record in that table. Following is an example to create a CHECK validation on AGE column which will not accept if its value is below to 18.

![image](https://github.com/AjaypalSinghMahal/rdbms_2023batch/assets/79219246/f9c4b85c-4805-4f38-9d1c-10548c4aa886)
[Experiment-3(AJAYPAL).md](https://github.com/AjaypalSinghMahal/rdbms_2023batch/files/12840108/Experiment-3.AJAYPAL.md)
