1-Difference between DDL, DML and DCL. <br>


| Particular | Data Definition Language| Data Manipulation Language| Data Control Language| 
| :---:       | :---        |:----   |:--- | 
| Fullform | DDL stands for Data Definition Language | DDL stands for Data Manipulation Language | DDL stands for Data Control Language |
| Purpose |It defines the database structure or schema. | It is used to modify or manipulate the data in the database. | It is used to control the access to the data in the database. |
| Usage |DDL commands are typically executed by database administrators or schema designers. | DML commands are used by application developers, analysts, and end-users to interact with and manipulate data. | DCL commands are used by administrators to manage access and permissions. |
| Affects Data vs. Schema |DDL affects the schema of the database, modifying its structure and organization. | DML affects the data within the database, adding, modifying, or removing individual records. | DCL affects who can access what parts of the data and perform specific operations. |
| Transaction Control: |DDL commands are auto-committed and cannot be rolled back within a transaction. | DML commands can be committed (saved) or rolled back (undone) within a transaction. | DCL commands do not impact transaction control directly, as they manage access rather than data changes. |
| Security and Access Control: |DDL does not focus on security or access control but defines the overall structure of the database. | DML can be performed based on the permissions granted to users and roles. | DCL explicitly manages permissions, allowing or denying access to specific database objects for users and roles. |
| Example |  DDL commands are - CREATE, DROP, ALTER, TRUNCATE, COMMENT ,RENAME | DDL commands are - SELECT, INSERT, UPDATE, DELETE, MERGE, CALL | DDL commands are - REVOKE, GRANT |
