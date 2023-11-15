                                  Experiment:-7
            Error handling using Internal Exceptions and External Exceptions

An exception is an error which disrupts the normal flow of program instructions.
PL/SQL provides us the exception block which raises the exception thus helping the programmer to find out the fault and resolve it.
There are two types of exceptions defined in PL/SQL
1.	User defined exception.
2.	System defined exceptions.

Syntax to write an exception:-

WHEN exception THEN 

    statement;

DECLARE

declarations section;

BEGIN

executable command(s);

EXCEPTION

WHEN exception1 THEN

statement1;

WHEN exception2 THEN

statement2;

[WHEN others THEN]



END;

Exception Types:-
UDFs and SPs raise exceptions when errors occur during execution.
Unhandled exceptions generate an exception message and a stack trace that is returned to the client.

Two kinds of exceptions can be raised:

•	An internal exception, which is a predefined exception generated by SingleStoreDB Cloud
•	A user-defined exception, which is defined by the user in a UDF or SP
Exception Handling Syntax:-

If you want to catch an exception, you can use a Statement Block containing an exception handling section beginning with the EXCEPTION keyword. Here is the syntax for statement blocks that can use EXCEPTION:

statement_block:

  [ DECLARE variable_list ] [ ...n ]
  
  BEGIN
  
    statement_list
    
  [ EXCEPTION
    when_clause_list ]

    
  END;

when_clause_list:

  when_clause [ ...n ]

when_clause:

  WHEN exception_type THEN statement_list
exception_type
An exception_type is the name of a built-in server error type. There is currently no published list of all the different error names, but the error name will always appear in the call stack displayed for an uncaught exception.
The keyword OTHERS can also be used as an exception_type. OTHERS will match all exceptions.
statement_list
A list of one or more statements terminated by semicolons.
Internal Exceptions:-

Internal exceptions are defined by SingleStoreDB Cloud, and they are raised when a function or procedure errors under a wide variety of conditions. These exception types encompass SQL syntax errors, insertion errors, connection errors, and so on.
Here are some possible internal exceptions:
|Exception Name|	Description|	Scenario When Exception is Thrown|
|-----|-----|------|
ER_SCALAR_BUILTIN_NO_ROWS_CODE	|The Scalar function did not return any value.|	This exception is thrown when a SCALAR function does not return any row (value).
ER_BAD_FIELD_ERROR	|Column name does not exist.|	A column that does not exist in a table is referenced in a query.
ER_TABLE_EXISTS_ERROR|	Table already exists.	|While creating a table, a table with the same name already exists.
ER_BAD_TABLE_ERROR	|Table does not exist.	|A table that does not exist is referenced in a query.
ER_NO_SUCH_TABLE|	Table does not exist.|	A table that does not exist is referenced in a query.
ER_DUP_ENTRY_WITH_KEY_NAME|	Duplicate key error.| The error message contains the key name as well.	A duplicate value is entered for a column with a key constraint.
ER_WRONG_VALUE_COUNT_ON_ROW|	Column count does not match value count.	|The number of columns in a table and the number of values specified in the query are not the same. For example, INSERT query.
ER_PARSE_ERROR|	Issue with parsing dynamic SQL.|	There is an error in the SQL statement.
ER_FILE_NOT_FOUND|	Cannot find file, usually in LOAD DATA statements.|	Either the file does not exist or the file path is incorrect.


Consider the following example, where table t contains two entries and id is defined as a PRIMARY KEY:
CREATE TABLE t(id INT PRIMARY KEY, str VARCHAR(255));
CREATE TABLE t_errors(dt DATETIME, id INT, str VARCHAR(255));

INSERT t VALUES (0, "foo"), (1, "bar");
The following procedure attempts to insert a row with a duplicate primary key, which raises the ER_DUP_ENTRY exception.
This exception triggers the procedure’s exception-handling behavior, where the row with a duplicate primary key is written to a t_ errors table instead:
DELIMITER //
CREATE OR REPLACE PROCEDURE insert_ handle_ exception(

  id INT, str VARCHAR(255)) AS
  
  BEGIN
  
    START TRANSACTION;
    
    INSERT INTO t VALUES (1, str);
    
    COMMIT;

    EXCEPTION
    
      WHEN ER_DUP_ENTRY THEN
      
        ROLLBACK;
        
        START TRANSACTION;
        
        INSERT INTO t_ errors VALUES (current_ timestamp(), id, str);
        
        COMMIT;
  END //


The use of START TRANSACTION, COMMIT, and ROLLBACK above is not really necessary in this simple example, but it does illustrate how you can use transaction control statements in conjunction with exception handling. For example, it may be necessary to roll back a transaction when you catch an exception, to make sure partial work is not committed.

User-Generated Exceptions:-

Users can generate their own exceptions through the RAISE USER_EXCEPTION() statement. USER_EXCEPTION() is a function that takes a string argument. You can pass any string expression as the USER_EXCEPTION argument. This statement will raise an ER_USER_RAISE exception.
The RAISE keyword by itself can only be used inside of an EXCEPTION block, and it re-raises the currently caught exception.
When in an EXCEPTION block, the EXCEPTION_MESSAGE() function can be used to get the message that was passed into USER_EXCEPTION for the currently caught exception. Here’s an example that shows a possible use of EXCEPTION_MESSAGE()
DELIMITER //

CREATE OR REPLACE PROCEDURE attemptWithRetry() AS

DECLARE i INT;

BEGIN

  WHILE true LOOP
  
    BEGIN
    
      START TRANSACTION;
      
      CALL attempt();

    EXCEPTION
      WHEN ER_USER_RAISE THEN
        ROLLBACK;
        IF exception_message() = "retry" THEN
          i = sleep(1);
          CONTINUE;
        ELSIF exception_message() = "abort" THEN
          RAISE;
        END IF;
      WHEN OTHERS THEN
        ROLLBACK;
        RAISE user_exception("other exception");
        -- i = sleep(1);
    END;

    COMMIT;
    EXIT;
  END LOOP;
END //
DELIMITER ;

DELIMITER //

CREATE OR REPLACE PROCEDURE attempt() AS

DECLARE i INT; j INT NOT NULL = 0;

BEGIN

  i = now() % 10;
  
  IF i >= 7 THEN
  
    RAISE user_exception("abort");
    
  ELSIF i <= 3  THEN
  
    j = NULL; -- force an exception by assigning NULL to a NOT NULL type
    
  END IF;
  
  RAISE user_exception("retry");
  
END //

DELIMITER ;

This example illustrates the use of OTHERS to catch exceptions not explicitly named in a WHEN clause. When i <= 3 (about 30% of the time) in attempt(), the assignment j = NULL is tried, and it will always fail because j is declared as NOT NULL. That will generate a system exception, which will be caught at WHEN OTHERS.
Now, when we call attemptWithRetry(), you can see that either the abort user exception or the other exception user exception was raised. This may take anywhere from 0 to a few seconds depending on what time it is when the procedure is first called.
