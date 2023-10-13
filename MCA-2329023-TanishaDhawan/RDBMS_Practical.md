#<p align="center">**Practical File**</p>
1.<p align="left">*Comparative study of various Database Management Systems*</p>

<br>
#<p align="center">**My SQL**</p>
  <br>
MySQL is one of the most popular relational database systems. Originally an open-source solution, MySQL is now owned by Oracle Corporation. Today, MySQL is a pillar of LAMP application software. That means it’s a part of Linux, Apache, MySQL, and Perl/PHP/Python stack. Having C and C++ under the hood, MySQL works well with such system platforms as Windows, Linux, MacOS, IRIX, and others.

**Pros of MySQL:-**
<br>
**Simple syntax and mild complexity**. MySQL’s structure and style are very plain. Developers even consider MySQL a database with a human-like language. MySQL is often used in tandem with the PHP programming language. Because they share a gentle learning curve, it’s much easier to form a team to manage your database. Also, MySQL is easy to use. For instance, most of the tasks can be executed right in the command line, reducing development steps.
<br>
**Cloud compatibility**. Business-oriented by nature and originally developed for the web, MySQL is supported by the most popular cloud providers. It’s available on leading platforms like Amazon, Microsoft, and others. This makes MySQL even more attractive and gives businesses room for growth.
<br>
**Cons of MySQL:-**
<br>
**Scalability challenges**. MySQL was not built with scalability in mind, which is inherent in its code. Theoretically, you can scale MySQL, but it will need more engineering effort than any of the NoSQL databases. So, if you expect one day your database will increase substantially, keep this limitation in mind or choose another DBMS option.
<br>
**Limited compliance with SQL standards**. Structured Query Language has specific standards. MySQL doesn’t completely follow them, i.e., MySQL provides no support for some standard SQL features. On the other hand, MySQL has some extensions and distinct features that don’t match the Structured Query Language standards. It’s not a big deal for small web applications. The issues may appear when you have to shift to other databases, which will likely happen when your business starts growing.
<br>
#<p align="center">**MariaDB**</p>
MariaDB, an open-source fork from MySQL, is a great SQL database example with commercial support. It works under a GNU General Public License and has similar commands, APIs, and libraries to MySQL.
<br>

**Pros of MariaDB:-**
<br>
**Encryption**. For MariaDB, open source doesn’t mean insecure. In addition to internal security and password check, MariaDB provides such features as PAM and LDAP authentication, Kerberos, and user roles.
<br>
**Broad functionality.** MariaDB has introduced a lot of new features in the last few years. For instance, GIS support suggests smooth coordinate storage and location data queries. Dynamic columns allow a single DBMS to provide both SQL and NoSQL data handling for different needs.
<br>
**High performance**. Although MariaDB originates from the MySQL engine, it’s gotten very far in terms of performance. Extensive optimization features improve thread pool management and data processing. Thus, when rows from the table are deleted, the operating system immediately accesses the free space, eliminating gaps in the tablespace.
<br>
**Cons of MariaDB:-**
<br>
**High cost**. Though the Oracle database has free editions, they are very limited in terms of functionality. Standard Edition, which doesn’t include all available features, costs $17,500 per unit. The Enterprise Edition is over $47,000 per unit.
<br>
**Resource-consuming technology**. The Oracle database needs powerful infrastructure. Not only does installation require a lot of disk space, but you’ll also have to consider constant hardware updates if you deploy it on-premises.
<br.
**Hard learning curve**. Oracle database is not a system to start using right away. It’s better to have certified Oracle DB engineers to run it. Oracle’s documentation, while covering many issues, can sometimes be overwhelming and even confusing. So, to install and run an Oracle database, you’ll have to consider hiring dedicated experts.
<br>
#<p align="center">**Oracle**</p>
<br>
Oracleis a relational database management system created and run by the Oracle Corporation. Among all the types of SQL databases, Oracle stands out. Currently, it supports multiple data models like document, graph, relational, and key-value within a single database. In its latest releases, it refocused on cloud computing. Oracle database engine licensing is fully proprietary, with both free and paid options available.
<br.
**Pros of Oracle:-**
<br>
**Innovations for daily workflow**. Starting with the Oracle 12c release, when the software entered the hybrid cloud era, new cloud computing technologies appeared regularly. With every new release, Oracle tries to keep up with the innovation pace while focusing on information security, including active data guard, partitioning, improved backup, and recovery.
<br>
**Strong tech support and documentation**. Oracle ensures decent customer support and provides comprehensive tech documentation across multiple resources. So, you’ll likely find solutions to any issues that appear. You may also expect some community support.
<br>
**Large capacity**. Oracle’s multi-model solution allows for accommodating and processing a vast amount of data. Thanks to the recently released multi-tenancy feature, the database architecture now simplifies packing many databases and manages them smoothly. In combination with in-memory data processing capabilities, it creates a strong engine for synchronous data processing.
<br>
**Cons of Oracle:-**
<br>
**High cost**. Though the Oracle database has free editions, they are very limited in terms of functionality. Standard Edition, which doesn’t include all available features, costs $17,500 per unit. The Enterprise Edition is over $47,000 per unit.
<br>
**Resource consuming technology**. The Oracle database needs powerful infrastructure. Not only does installation require a lot of disk space, but you’ll also have to consider constant hardware updates if you deploy it on-premises.
<br.
**Hard learning curve.** Oracle database is not a system to start using right away. It’s better to have certified Oracle DB engineers to run it. Oracle’s documentation, while covering many issues, can sometimes be overwhelming and even confusing. So, to install and run an Oracle database, you’ll have to consider hiring dedicated experts.
#<p align="center">**Redis**</p>
<br>
An open-source, NoSQL, in-memory data structure store, Redis can also be used as a cache. Instead of documents, it uses key-value pairs. Its distinct feature is that there are several options for data structuring, such as lists, sets, and hashes.

Allowing for data replication and supporting transactions, Redis executes commands in a queue instead of setting it one at a time.
<br>
**Pros of Redis:-**
<br>
**Rapid solution**. Due to its replication and transaction features, Redis processes the data really fast. The absence of dependencies and in-memory data store type makes Redis a worthy competitor even among simple SQL alternatives.
<br>
**Massive data processing.** From the data perception and refining perspective, Redis can be considered a colossus. It can easily upload up to 1GB of data for one entry. Add built-in data caching and you get a powerhouse data machine.
<br>
**Cons of Redis:-**
<bbr>
**Dependency on the application memory**. Total reliance and dependency on the application memory is a real drawback. That is to say, your database will crash if its size exceeds the size of available memory.
<br>
**No support for query language or joins**. Regarding compatibility with other dataset types, Redis lags behind. Given that at some time your business may need scaling and using other data formats, having rapid entries as a single option leaves this issue open.
<br>
#<p align="center">**MongoDB**</p>
<br>
A free, open-source, non-relational DBMS, MongoDB also includes a commercial version. Although MongoDB wasn’t initially intended for structured data processing, it can be employed for applications that use both structured and unstructured data. In MongoDB, databases are connected to applications via database drivers. They are widely available within the database management system. Multiple data types are processed simultaneously and use the internal cache for this purpose.
<br>
**Pros of MongoDB:-**
<br>
**Simple data access, storage, input, and retrieval**. One of the benefits of MongoDB derived from its NoSQL nature is the fast and easy data operation. That is to say, data can be entered, stored, and withdrawn from the database quickly and without any additional confirmation. As with any other non-relational database, it places emphasis on RAM usage, so the records can be manipulated really fast and without any consequences to data integrity.
<br>
**Easy compatibility with other data models**. MongoDB is easily combined with different database management systems, both SQL and NoSQL types. Besides that, it has pluggable storage engine APIs. To make a long story short, this option allows third parties to build their own data storage engines for MongoDB. From a commercial point of view, it creates extra value for business software.
<br>
**Horizontally scalable solution.** Scalability – where data is spread out across a distributed network of manageable servers – is a facet of MongoDB’s fundamental nature. It becomes even more important for enterprises operating big data applications. Additionally, the database can allocate data across a cluster of machines. How can that help you? The data is distributed faster and equally, free of bulkiness. As it leads to faster data processing, the application performance is accelerated too.
<br>
**Cons of MongoDB:-**
**Extensive memory consumption.** The denormalization process, when previously normalized data in a database is grouped to increase performance, usually results in high memory consumption. Also, this DBMS keeps in memory all key names for each value pair. Beyond that, because there is no support for joins, Mongo databases have data oversupply, resulting in big memory waste and lower application performance.
<br>
**Data insecurity**. With a focus on fast data operation, MongoDB, like any other NoSQL DBMS, lacks data security. As user authentication isn’t a default Mongo option, and higher protection is available with a commercial edition only, you can’t consider it totally secure. Additionally, there are constant MongoDB update releases, with no guarantee that all amendments or data changes will work as they did before. Keep in mind that all manipulations should be formed around these updates, being covered with additional tests.
<br>
**Complicated process to interpret into other query languages**. As MongoDB wasn’t initially developed to deal with relational data models, the performance may slow down in these cases. Besides, the translation of SQL to MongoDB queries takes additional action to use the engine, which may delay the development and deployment.
<br>






