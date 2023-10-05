Differnce between DDL, DML, DCL Commands


*Data Manipulation Language (DML)* - The Data Manipulation Language is the sublanguage responsible for adding, editing or deleting data from a database. In SQL, this corresponds to the INSERT, UPDATE, and DELETE
*Data Definition Language (DDL) *- The Data Definition Language is the sublanguage responsible for defining the way data is structured in a database. In SQL, this corresponds to manipulating tables through the CREATE TABLE, ALTER TABLE, and DROP TABLE
*Data Control Language (DCL) *- The Data Control Language is the sublanguage responsible for the administrative tasks of controlling the database itself, most notably granting and revoking database permissions for users. In SQL, this corresponds to the GRANT, REVOKE, and DENY commands, among others.

*Data Manipulation Language (DML)* The Data Manipulation Language, or DML for short, is the group of commands responsible for manipulating data in a database; this generally entails inserting, editing, or deleting rows in SQL tables.

The SQL command for inserting a new row in a table is the INSERT command. If we want to add a row to the Accounts table for a user called Evan Johnson with a balance of $3200, we would do something like this:

INSERT INTO Accounts (Name, Balance)
VALUES (‘Evan Johnson’, 3200)
If, at some point in the future, Evan made a withdrawal of $200, we would need to update his balance to $3000. To edit Evan’s bank account record, we need to use the UPDATE command:

UPDATE Accounts SET Balance = 3000
WHERE Name = ‘Evan Johnson’
Finally, if Evan decided to close his account at our bank, we would need to delete his entry in the Accounts table. To accomplish this, we need to use the DELETE command:

DELETE FROM Accounts
WHERE Name = ‘Evan Johnson’

The Data Definition Language, or DDL, is made up of the commands responsible for creating, editing and deleting SQL tables. These commands are CREATE TABLE, ALTER TABLE, and DROP TABLE.

In the examples above, we were working with the Accounts table, which already had a structure and records. But how would we go about creating this table in the first place? We’d need to use the CREATE TABLE command:

CREATE TABLE Accounts (
    ID INT,
    Name VARCHAR(255),
    Balance INT
)
What if we then wanted to edit the table so it had a column storing account holders’ phone numbers? We’d use the ALTER TABLE command:

ALTER TABLE Accounts
ADD Phone VARCHAR(255)
Finally, if we want to delete the Accounts table altogether, we’d use the DROP TABLE command:

DROP TABLE Accounts

Data Control Language (DCL)
The Data Control Language, or DCL for short, is responsible for all sorts of administrative tasks around the database itself. The most notable one is setting permissions for database users, which is done chiefly through the GRANT, REVOKE, and DENY commands.

GRANT is the SQL command responsible for granting permissions to a database user. If we wanted to grant the permission to query the Accounts table to a user named Mark, we’d do something like this:

GRANT SELECT TO ‘mark’@’localhost’
To explicitly deny the permission to query the table for a database user, use the DENY command as follows:

DENY SELECT FROM ‘mark’@’localhost’
Note that explicitly denying a permission prevents it from being granted in the future. If we simply want to reverse a GRANT or DENY command, we should use the REVOKE command:

REVOKE SELECT FROM ‘mark’@’localhost’
The above command reverses any particular GRANT and DENY permissions assigned to the user, essentially resetting them to their default state.
