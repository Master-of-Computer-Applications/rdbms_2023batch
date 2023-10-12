# <p align="center">Guru Nanak Dev Engineering College, Ludhiana</p>
![front](https://user-images.githubusercontent.com/82715927/121130621-4a076380-c84c-11eb-85e0-81619d36d244.png)

### <p align="center">Practical File</p>
### <p align="center">Of</p>
### <p align="center">Relational Database Management Systems Lab</p>
### <p align="center">Course Code: "PGCA- 2208"</p>
### <p><h3 align="left">Submitted to :</br>Mr.Satinderpal Singh</h3><h3 align="right">Submitted by: </br>Puneet Jain</br>(MCA 1st sem.)</br>CRN:-2029014</h3></p>

Sr no|  Experiment Name |  Remarks|   
|---|---|---|
|  1| Comparative study of various Database Management Systems.  |   |   
|  2|Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL).   |   |   
|  3|How to apply Constraints at various levels. |   |   
|  4|View data in the required form using Operators, Functions and Joins.  |  |
|  5|Creating different types of Views for tailored presentation of data.  |  |
|  6|How to apply Conditional Controls in PL/SQL.   |  |
|  7|Error Handling using Internal Exceptions and External Exceptions.   |  |
|  8|Using various types of Cursors   |  |
|  9|How to run Stored Procedures and Functions.   |  |
|  10|Creating Packages and applying Triggers.   |  |
|  11|Creating Arrays and Nested Tables.  |  |

## *1. Comparative study of various Database Management Systems.*
***Database Management System:***
A Database Management System (DBMS) is a specialized software designed to store, retrieve, and manipulate data. It acts as a mediator between the database, applications, and user interfaces to manage and organize data effectively. The system provides a comprehensive suite of tools to govern databases, ensuring data security, consistency, and integrity.

A DBMS supports various applications, from simple storage and retrieval tasks to complex data-driven systems, by implementing efficient data access and management practices. Additionally, the system can handle concurrent users, maintain transactional consistency, and provide robust backup and recovery options, making it an essential component in any data-centric environment.

**Types of databases:**
</br>(1)MySQL </br>(2)MariaDB </br>(3)Oracle </br>(4)PostgreSQL </br>(5)SQLite 

## ***(1)MySQL***-
MySQL is one of the most popular relational database systems. Originally an open-source solution, MySQL is now owned by Oracle Corporation. Today, MySQL is a pillar of LAMP application software. That means it’s a part of Linux, Apache, MySQL, and Perl/PHP/Python stack. Having C and C++ under the hood, MySQL works well with such system platforms as Windows, Linux, MacOS, IRIX, and others.

### **Pros of MySQL:**

**(i) Free installation**-The community edition of MySQL is free to download. With a basic set of tools for individual use, MySQL community edition is a good option, to begin with. Of course, there are other, prepaid versions for Enterprise or Cluster purposes with richer functionality. Nevertheless, if your company is too small to pay for one of them, the free-to-download model is the most suitable for a fresh start.

**(ii) Simple syntax and mild complexity**-MySQL’s structure and style are very plain. Developers even consider MySQL a database with a human-like language. MySQL is often used in tandem with the PHP programming language. Because they share a gentle learning curve, it’s much easier to form a team to manage your database. Also, MySQL is easy to use. For instance, most of the tasks can be executed right in the command line, reducing development steps.

**(iii) Cloud compatibility**-Business-oriented by nature and originally developed for the web, MySQL is supported by the most popular cloud providers.  It’s available on leading platforms like Amazon, Microsoft, and others. This makes MySQL even more attractive and gives businesses room for growth.

### **Cons of MySQL:**

**(i) Scalability challenges**-MySQL was not built with scalability in mind, which is inherent in its code. Theoretically, you can scale MySQL, but it will need more engineering effort than any of the NoSQL databases. So, if you expect one day your database will increase substantially, keep this limitation in mind or choose another DBMS option.

**(ii)Partial open-source support**-Although MySQL has an open-source part, it’s mostly under Oracle’s license. This limits the MySQL community in terms of improving the DBMS. Why do you care? Because when you have completely open-source support, you expect many problem-specific implementations and community assistance. This is not the case when the software belongs to corporate owners, and you have to pay for support.

**(iii)Limited compliance with SQL standards**-Structured Query Language has specific standards. MySQL doesn’t completely follow them, i.e., MySQL provides no support for some standard SQL features. On the other hand, MySQL has some extensions and distinct features that don’t match the Structured Query Language standards. It’s not a big deal for small web applications. The issues may appear when you have to shift to other databases, which will likely happen when your business starts growing.

## ***(2)MariaDB***-
MariaDB, an open-source fork from MySQL, is a great SQL database example with commercial support. It works under a GNU General Public License and has similar commands, APIs, and libraries to MySQL.

### **Pros of MariaDB:**

**(i)Encryption**-For MariaDB, open source doesn’t mean insecure. In addition to internal security and password check, MariaDB provides such features as PAM and LDAP authentication, Kerberos, and user roles. Combined with encrypted tablespaces, tables, and logs, it creates a robust protective layer for data. Beyond that, MariaDB publishes related releases on each security update, keeping the security patches totally transparent.

**(ii)Broad functionality**-MariaDB has introduced a lot of new features in the last few years. For instance, GIS support suggests smooth coordinate storage and location data queries. Dynamic columns allow a single DBMS to provide both SQL and NoSQL data handling for different needs. You can also extend its functionality with plugins that are available at MySQL via 3rd parties only. MariaDB is shipped with storage engines for NoSQL backend, legacy database migration tools, sharding options, and much more.

**(iii)High performance**-Although MariaDB originates from the MySQL engine, it’s gotten very far in terms of performance. Extensive optimization features improve thread pool management and data processing. Thus, when rows from the table are deleted, the operating system immediately accesses the free space, eliminating gaps in the tablespace. On top of that, the database management system suggests engine-independent table statistics. This feature enhances the optimizer’s performance, accelerates query processing, and helps customize data analysis.

### **Cons of MariaDB:**

**(i)Still a growing community**-Although MariaDB has substantial open-source contribution, its community has yet to grow much. Since this database management system was established not so long ago, the number of professionals involved is relatively small.

**(ii)Gaps between MySQL and MariaDB update versions**-Though the MariaDB team is constantly merging its code with MySQL’s, it’s already not that simple to keep them in line. Given the currently existing differences between MariaDB 10.6 and MySQL 8.0.32, further deviations are yet to come. Additionally, MySQL engineers introduced some native features to the code that are only available to commercial MySQL users. This can create compatibility issues or data migration problems from MariaDB back to MySQL.

## ***(3)Oracle***-
Oracle is a relational database management system created and run by the Oracle Corporation. Among all the types of SQL databases, Oracle stands out. Currently, it supports multiple data models like document, graph, relational, and key-value within a single database. In its latest releases, it refocused on cloud computing. Oracle database engine licensing is fully proprietary, with both free and paid options available.

## **Pros of Oracle:**

**(i)Innovations for daily workflow**-Starting with the Oracle 12c release, when the software entered the hybrid cloud era, new cloud computing technologies appeared regularly. With every new release, Oracle tries to keep up with the innovation pace while focusing on information security, including active data guard, partitioning, improved backup, and recovery.

**(ii)Large capacity**-Oracle’s multi-model solution allows for accommodating and processing a vast amount of data. Thanks to the recently released multi-tenancy feature, the database architecture now simplifies packing many databases and manages them smoothly. In combination with in-memory data processing capabilities, it creates a strong engine for synchronous data processing.

## **Cons of Oracle:**

**(i)High cost**-Though the Oracle database has free editions, they are very limited in terms of functionality. Standard Edition, which doesn’t include all available features, costs $17,500 per unit. The Enterprise Edition is over $47,000 per unit.

**(ii)Resource-consuming technology**-The Oracle database needs powerful infrastructure. Not only does installation require a lot of disk space, but you’ll also have to consider constant hardware updates if you deploy it on-premises.

**(iii)Hard learning curve**-Oracle database is not a system to start using right away. It’s better to have certified Oracle DB engineers to run it. Oracle’s documentation, while covering many issues, can sometimes be overwhelming and even confusing. So, to install and run an Oracle database, you’ll have to consider hiring dedicated experts.

## ***(4)PostgreSQL***- 
The PostgreSQL database management system shares its popularity with MySQL. This is an object-relational DBMS where user-defined objects and table approaches are combined to build more complex data structures. Besides that, PostgreSQL has a lot of similarities with MySQL. It’s aimed at strengthening the standards of compliance and extensibility. Consequently, it can process any workload, for both single-machine products and complex applications. Owned and developed by PostgreSQL Global Development Group, it still remains completely open-source. This DBMS is available for use with platforms like Microsoft, iOS, Android, and many more.

## **Pros of PostgreSQL:**

**(i)Great scalability**-Vertical scalability is a hallmark of PostgreSQL. Considering that almost any custom software solution tends to grow, resulting in database extension, this particular option certainly supports business growth and development.

**(ii)Support for custom data types**-PostgreSQL natively supports many data types by default, such as JSON, XML, H-Store, and others. PostgreSQL takes advantage of it, being one of the few relational databases with strong support for NoSQL features. Additionally, it allows users to define their own data types. As your software business model may need different types of databases throughout its existence for better performance or application comprehensiveness, this option brings improved flexibility to the table.

**(iii)Easily-integrated third-party tools**-The PostgreSQL database management system has the strong support of additional tools, both free and commercial. The scope of these includes extensions to improve many aspects. For example, ClusterControl provides impressive assistance in managing, monitoring, and scaling SQL and NoSQL open-source databases. To make data comparison and synchronization more effective, consider using DB Data Directive. In case you’re going to scale up your data to heavy workloads, the pgBackRest backup and restore system will be a nice option to choose from.

**(iv)Open-source and community-driven support**-Postgres is completely open-source and supported by its community, strengthening it as a complete ecosystem. Additionally, developers can always expect free and prompt community assistance.

## **Cons of PostgreSQL:**

**(i)Inconsistent documentation**-While PostgreSQL has a large community and strongly supports its participants, the documentation still lacks consistency and completeness. As the PostgreSQL community is rather distributed, the documentation doesn’t follow uniform standards for all Postgre features.

**(ii)Lack of reporting and auditing instruments**-A significant shortcoming of PostgreSQL is the absence of revising tools that would show the current condition of a database. You have to continuously check if something goes wrong. There’s always a risk that DB engineers will notice a failure too late.

## ***(5)SQLite***- 
SQLite is a self-sufficient, serverless, and no-configuration-required database management system. Frequently utilized as an embedded database, it is popular for small-scale mobile and desktop applications.

## **Pros of SQLite:**

**(i)Small in size and easily portable**-SQLite is a streamlined database engine that operates without a separate server process. The entire database is contained within a single cross-platform disk file, enhancing its portability and simplifying its integration into applications.

**(ii)Minimal resource consumption**-SQLite is engineered for optimal memory and disk space efficiency, making it an ideal choice for applications with constrained resources, such as those found in mobile and IoT devices.

**(iii)Reliable and user-friendly**-SQLite is an ACID-compliant database, ensuring the integrity and consistency of data. Additionally, it is simple to set up and demands minimal configuration.

## **Cons of SQLite:**

**(i)Restricted concurrency**-SQLite employs file-based locking, limiting its capacity to manage multiple concurrent write operations. This makes it less appropriate for applications with high write concurrency or multiple users accessing the database simultaneously.

**(ii)Absence of advanced features**-SQLite lacks some of the sophisticated features found in other database management systems, such as stored procedures, triggers, or user-defined functions.

**(iii)Restricted scalability**-Owing to its serverless structure, SQLite is not tailored for extensive applications or distributed settings. Its performance may diminish when handling substantial datasets or elevated levels of concurrent access.


## *2. Data Definition Language (DDL), Data Manipulation Language (DML), and Data Control Language (DCL).*
***Differences Between DDL, DML,and DCL:***
**DDL Commands**:

DDL commands are SQL commands used to modify or alter the structure of the database. The following is the list of DDL commands in SQL:

1-The CREATE command creates database objects, tables, and triggers.
2-ALTER command alters the database structure by adding, deleting, and modifying columns of the already existing tables, like renaming and changing the data type and size of the columns.
3-The DROP command deletes the defined table with all the table data, associated indexes, constraints, triggers, and permission specifications.
4-The TRUNCATE command deletes all the data and records from an existing table, including the allocated spaces for the records. Unlike the DROP command, it does not delete the table from the database. It works similarly to the DELETE statement without a WHERE clause.
5-The RENAME command changes the table name when the user or administrator wants to give a more relevant name to it.


DDL | DML | DCL
|---|---|---|
DDL stands for Data Definition Language.|DML stands for Data Manipulation Language.|DCL stands for Data Control Language.
It helps us to define the structure of the database.|It helps us to manage the data.|t helps us to control the access and permission of the database.
It affects the entire table data.|It only affects the specified row(s) of the table.|It applies to the complete table.
Changes are permanent.|We can roll back our changes in the DML language.|We can roll back the changes in the DCL language.
It helps in defining the fields or columns of the tables.|It helps us to define rows or records of the tables.|It helps us to control access to the information in the database.
They are auto-committed (changes made are permanent).|They are not auto-committed (changes are not permanent).|They are not auto-committed (changes are not permanent). 
They don't have further classification.|They are of two types procedural and non-procedural.|They don't have any further classification.
Commands used: CREATE, ALTER, TRUNCATE, RENAME, DROP.|Commands used: SELECT, UPDATE, DELETE, INSERT.|Commands used: REVOKE, GRANT.


## *3. How to apply Constraints at various levels.*
SQL constraints are used to specify rules for the data in a table.

Constraints are used to limit the type of data that can go into a table. This ensures the accuracy and reliability of the data in the table. If there is any violation between the constraint and the data action, the action is aborted.

Constraints can be column level or table level. Column level constraints apply to a column, and table level constraints apply to the whole table.

The following constraints are commonly used in SQL:

  (1) NOT NULL - Ensures that a column cannot have a NULL value(/br)
  (2) UNIQUE - Ensures that all values in a column are different
  (3) PRIMARY KEY - A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table
  (4) FOREIGN KEY - Prevents actions that would destroy links between tables
  (5) CHECK - Ensures that the values in a column satisfies a specific condition
  (6) DEFAULT - Sets a default value for a column if no value is specified
  (7) CREATE INDEX - Used to create and retrieve data from the database very quickly


