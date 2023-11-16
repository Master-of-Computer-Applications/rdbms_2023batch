# <p align="center">ASSIGNMENT 2 OF RDMBS</p>
## NORMALIZATION OF RDBMS
<p> Normaliion is the process of minimizing redundancy from a relation or set of relations. Redundancy in relation may cause insertion, deletion, and update anomalies. So, it helps to minimize the redundancy in relations.
The main goal of normalization is to structure the database in a way that minimizes data anomalies and anomalies that can occur during data insertion, updating, and deletion.

Normalization is typically achieved by dividing a database into a set of related tables and establishing relationships between these tables. The process is usually divided into several normal forms, each with specific rules and criteria. </p>

Normal forms are used to eliminate or reduce redundancy in database tables.There are several levels of normalization, each with its own set of guidelines, known as normal forms. These are -

1. First Normal Form (1NF)
2. Second Normal Form (2NF)
3. Third Normal Form (3NF)
4. Boyce-Codd Normal Form (BCNF)
5. Fourth Normal Form (4NF)
6. Fifth Normal Form (5NF)

### **Advantages of Normalization:**
- Normalization helps to minimize data redundancy.
- Greater overall database organization.
- Data consistency within the database.
- Much more flexible database design.
- Enforces the concept of relational integrity.

## First Normal Form (1NF)
- A relation will be 1NF if it contains an atomic value.
- It states that an attribute of a table cannot hold multiple values. It must hold only single-valued attribute.
- First normal form disallows the multi-valued attribute, composite attribute, and their combinations.
  
**Example:** Relation EMPLOYEE is not in 1NF because of multi-valued attribute EMP_PHONE.

| EMP_ID      | EMP_NAME    | EMP_PHONE               | EMP_STATE|
| :---        |    :----:   |          :---:          |    :---: |
| 12          | Bob         | 7272826385, 9064738238  | Mumbai   |
| 21          | James       | 8574783832              |Kerala    |
| 18          | Daniel      | 7390372389, 8589830302  |Bangalore |

The decomposition of the EMPLOYEE table into 1NF has been shown below:

| EMP_ID      | EMP_NAME    | EMP_PHONE               | EMP_STATE|
| :---        |    :----:   |          :---:          |    :---: |
| 12          | Bob         | 7272826385              | Mumbai   |
| 12          | Bob         | 9064738238              | Mumbai   |
| 21          | James       | 8574783832              |Kerala    |
| 18          | Daniel      | 7390372389              |Bangalore |
| 18          | Daniel      | 8589830302              |Bangalore |

## Second Normal Form (2NF)
- The table must already be in 1NF.
- All non-key attributes (columns) must be functionally dependent on the entire primary key, not just part of it.
- This typically involves creating new tables to eliminate partial dependencies.

**Example:** Let's assume, a school can store the data of teachers and the subjects they teach. In a school, a teacher can teach more than one subject.

| TEACHER_ID  | SUBJECT     | TEACHER_AGE     |
| :---        |    :----:   |          :--- |
| 25          | IM          | 31            |
| 25          | OOPS        | 31            |
| 27          | RDBMS       | 43            |
| 29          | ASE         | 35            |
| 29          | TC          | 35            |

In the given table, non-prime attribute TEACHER_AGE is dependent on TEACHER_ID which is a proper subset of a candidate key. That's why it violates the rule for 2NF.

To convert the given table into 2NF, we decompose it into two tables:

**TEACHER_DETAIL table:**

| TEACHER_ID  |  TEACHER_AGE  |
| :---        |          :--- |
| 25          | 31            |
| 27          | 43            |
| 29          | 35            |

**TEACHER_SUBJECT table:**

| TEACHER_ID  | SUBJECT     | 
| :---        |    :----:   |
| 25          | IM          |
| 25          | OOPS        | 
| 27          | RDBMS       | 
| 29          | ASE         | 
| 29          | TC          | 

## Third Normal Form (3NF)
- The table must already be in 2NF.
- There should be no transitive dependencies, where a non-key attribute depends on another non-key attribute.
- A relation is in third normal form if it holds atleast one of the following conditions for every non-trivial function dependency X → Y.
  1. X is a super key.
  2. Y is a prime attribute, i.e., each element of Y is part of some candidate key.

**Example:**

**EMPLOYEE_DETAIL table:**

| EMP_ID      | EMP_NAME    | EMP_ZIP           | EMP_STATE| EMP_COUNTRY |
| :---        |    :----:   |      :---:        |    :---: |    :---:    |
| 212         | Bob         | 6385              |Mumbai    | India       |
| 312         | Kathie      | 8238              |UP        | India       |
| 421         | James       | 3832              |Kerala    | India       |
| 218         | Joe         | 7238              |Punjab    | India       |
| 518         | Daniel      | 0302              |Bangalore | India       |

**Super key in the table above:** {EMP_ID}, {EMP_ID, EMP_NAME}, {EMP_ID, EMP_NAME, EMP_ZIP}....so on

**Candidate key:** {EMP_ID}

**Non-prime attributes:** In the given table, all attributes except EMP_ID are non-prime.

Here, EMP_STATE & EMP_CITY dependent on EMP_ZIP and EMP_ZIP dependent on EMP_ID. The non-prime attributes (EMP_STATE, EMP_CITY) transitively dependent on super key(EMP_ID). It violates the rule of third normal form.

That's why we need to move the EMP_CITY and EMP_STATE to the new <EMPLOYEE_ZIP> table, with EMP_ZIP as a Primary key.

**EMPLOYEE table:**

| EMP_ID      | EMP_NAME    | EMP_ZIP           |
| :---        |    :----:   |      :---:        |
| 212         | Bob         | 6385              |
| 312         | Kathie      | 8238              |
| 421         | James       | 3832              |
| 218         | Joe         | 7238              |
| 518         | Daniel      | 0302              |

**EMPLOYEE_ZIP table:**

| EMP_ZIP           | EMP_STATE| EMP_COUNTRY |
|      :---:        |    :---: |    :---:    |
| 6385              |Mumbai    | India       |
| 8238              |UP        | India       |
| 3832              |Kerala    | India       |
| 7238              |Punjab    | India       |
| 0302              |Bangalore | India       |

## Boyce Codd normal form (BCNF)
- BCNF is the advance version of 3NF. It is stricter than 3NF.
- A table is in BCNF if every functional dependency X → Y, X is the super key of the table.
- For BCNF, the table should be in 3NF, and for every FD, LHS is super key.

**Example:** Let's assume there is a company where employees work in more than one department.

**EMPLOYEE table:**

| EMP_ID      | EMP_COUNTRY | EMP_DEPT_NO       | EMP_DEPT  | DEPT_TYPE   |
| :---        |    :----:   |      :---:        |    :---:  |    :---:    |
| 212         | India       | 6385              |Designing  | D345        |
| 212         | India       | 8238              |Testing    | D345        |
| 421         | US          | 3832              |Stores     | D567        |
| 421         | US          | 7238              |Developing | D567        |

In the above table Functional dependencies are as follows:

EMP_ID  →  EMP_COUNTRY  
EMP_DEPT_NO  →   {EMP_DEPT ,DEPT_TYPE}  

**Candidate key:** {EMP-ID, EMP-DEPT_NO}

The table is not in BCNF because neither EMP_DEPT nor EMP_ID alone are keys. To convert the given table into BCNF, we decompose it into three tables:

**EMP_COUNTRY table:**

| EMP_ID      | EMP_COUNTRY |
| :---        |    :----:   |
| 212         | India       | 
| 421         | US          |

**EMP_DEPT table:**

| EMP_DEPT_NO       | EMP_DEPT  | DEPT_TYPE   |
|      :---:        |    :---:  |    :---:    |
| 6385              |Designing  | D345        |
| 8238              |Testing    | D345        |
| 3832              |Stores     | D567        |
| 7238              |Developing | D567        |

**EMP_DEPT_MAPPING table:**


| EMP_ID      |EMP_DEPT_NO       |
| :---        |     :---:        |
| 212         |6385              |
| 212         |8238              |
| 421         |3832              |
| 421         |7238              |

**Candidate keys:**

**For the first table:** EMP_ID

**For the second table:** EMP_DEPT_NO

**For the third table:** {EMP_ID, EMP_DEPT_NO}

Now, this is in BCNF because left side part of both the functional dependencies is a key.

## Fourth normal form (4NF)
- A relation will be in 4NF if it is in Boyce Codd normal form and has no multi-valued dependency.
- For a dependency A → B, if for a single value of A, multiple values of B exists, then the relation will be a multi-valued dependency.

**Example:**

**STUDENT table**

| STU_ID      | COURSE      | HOBBY         |
| :---        |    :----:   |         :---: |
| 21          | IM          | Dancing       |
| 21          | OOPS        | Singing       |
| 25          | RDBMS       | Cricket       |
| 27          | ASE         | Hockey        |

The given STUDENT table is in 3NF, but the COURSE and HOBBY are two independent entity. Hence, there is no relationship between COURSE and HOBBY.

In the STUDENT relation, a student with STU_ID, *21* contains two courses, *IM* and *OOPS* and two hobbies, *Dancing* and *Singing*. So there is a Multi-valued dependency on STU_ID, which leads to unnecessary repetition of data.

So to make the above table into 4NF, we can decompose it into two tables:

**STUDENT_COURSE table**

| STU_ID      | COURSE      |
| :---        |    :----:   |
| 21          | IM          |
| 21          | OOPS        |
| 25          | RDBMS       |
| 27          | ASE         |

**STUDENT_HOBBY table**

| STU_ID      |HOBBY         |
| :---        |        :---: |
| 21          |Dancing       |
| 21          |Singing       |
| 25          |Cricket       |
| 27          |Hockey        |


## Fifth normal form (5NF)
- A relation is in 5NF if it is in 4NF and not contains any join dependency and joining should be lossless.
- 5NF is satisfied when all the tables are broken into as many tables as possible in order to avoid redundancy.
- 5NF is also known as Project-join normal form (PJ/NF).

**EXAMPLE:**

| SUBJECT     | LECTURER      | SEMSTER    |
| :---:       |    :----:     |      :---  |
| Computer    | Isha          | 1          |
| Computer    | John          | 1          |
| Maths       | John          | 1          | 
| Maths       | Deepti        | 2          |
| Chemistry   | Prakash       | 1          |

In the above table, John takes both Computer and Math class for Semester 1 but he doesn't take Math class for Semester 2. In this case, combination of all these fields required to identify a valid data.

Suppose we add a new Semester as Semester 3 but do not know about the subject and who will be taking that subject so we leave Lecturer and Subject as NULL. But all three columns together acts as a primary key, so we can't leave other two columns blank.

So to make the above table into 5NF, we can decompose it into three relations P1, P2 & P3:

**P1 table**

| SUBJECT     | SEMSTER    |
| :---:       |      :---  |
| Computer    | 1          |
| Maths       | 1          | 
| Maths       | 2          |
| Chemistry   | 1          |

**P2 table**

| SUBJECT     | LECTURER      |
| :---:       |    :----:     |
| Computer    | Isha          |
| Computer    | John          |
| Maths       | John          |
| Maths       | Deepti        |
| Chemistry   | Prakash       | 

**P3 table**

| LECTURER      | SEMSTER    |
|    :----:     |      :---  |
| Isha          | 1          |
| John          | 1          |
| Deepti        | 2          |
| Prakash       | 1          |

<p>In conclusion, normalization forms in RDBMS provide a structured approach to designing databases that promote data integrity, efficiency, and flexibility. However, it's essential to carefully consider the specific requirements of your application and strike a balance between normalization and denormalization to achieve the best performance and maintainability for your database.</p>
