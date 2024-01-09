# <p align="center">Assignment 2 of DBMS</p>
## Definition of Normalization
### Normalization is the process of minimizing redundancy from a relation or set of relations. Redundancy in relation may cause insertion, deletion, and update anomalies. So, it helps to minimize the redundancy in relations. Normal forms are used to eliminate or reduce redundancy in database tables.
# Important points regarding Normal Forms
### First Normal Form (1NF) : This is the most basic level of normalization. In 1NF, each table cell should contain only a single value, and each column should have a unique name. The first normal form helps to eliminate duplicate data and simplify queries.<br>
### Second Normal Form (2NF): 2NF eliminates redundant data by requiring that each non-key attribute be dependent on the primary key. This means that each column should be directly related to the primary key, and not to other columns.<br>
### Third Normal Form (3NF): 3NF builds on 2NF by requiring that all non-key attributes are independent of each other. This means that each column should be directly related to the primary key, and not to any other columns in the same table.<br>
### Boyce-Codd Normal Form (BCNF): BCNF is a stricter form of 3NF that ensures that each determinant in a table is a candidate key. In other words, BCNF ensures that each non-key attribute is dependent only on the candidate key.<br>
### Fourth Normal Form (4NF): 4NF is a further refinement of BCNF that ensures that a table does not contain any multi-valued dependencies.<br>
### Fifth Normal Form (5NF): 5NF is the highest level of normalization and involves decomposing a table into smaller tables to remove data redundancy and improve data integrity.<br>
# Frist Form of Normalization
### l form if it does not contain any composite or multi-valued attribute. A relation is in first normal form if every attribute in that relation is singled valued attribute.

### Example 1 – Relation STUDENT in table 1 is not in 1NF because of multi-valued attribute STUD_PHONE. Its decomposition into 1NF has been shown in table 2.<br>

![form_1](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/3afb94a1-4507-45c1-a4dc-63297e0e66ac)<br>

# Second Normal Form
### To be in second normal form, a relation must be in first normal form and relation must not contain any partial dependency. A relation is in 2NF if it has No Partial Dependency, i.e., no non-prime attribute (attributes which are not part of any candidate key) is dependent on any proper subset of any candidate key of the table. Partial Dependency – If the proper subset of candidate key determines non-prime attribute, it is called partial dependency.<br>
![form_2](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/039a689c-1466-42bf-90b4-3631318a95fa)
# Third Normal Form
### A relation is in third normal form, if there is no transitive dependency for non-prime attributes as well as it is in second normal form.
### A relation is in 3NF if at least one of the following condition holds in every non-trivial function dependency X –> Y:
### 1. X is a super key.
### 2. Y is a prime attribute (each element of Y is part of some candidate key).
### Example:
### EMPLOYEE_DETAIL table:
![Selection_001](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/6af4b595-e1e0-4935-98ee-c2afde96e33e)
### Super key in the table above:

#### {EMP_ID}, {EMP_ID, EMP_NAME}, {EMP_ID, EMP_NAME, EMP_ZIP}....so on  
#### Candidate key: {EMP_ID}
### Non-prime attributes: In the given table, all attributes except EMP_ID are non-prime.
### Here, EMP_STATE & EMP_CITY dependent on EMP_ZIP and EMP_ZIP dependent on EMP_ID. The non-prime attributes (EMP_STATE, EMP_CITY) transitively dependent on super key(EMP_ID). It violates the rule of third normal form.
### That's why we need to move the EMP_CITY and EMP_STATE to the new <EMPLOYEE_ZIP> table, with EMP_ZIP as a Primary key.
### EMPLOYEE tablee:
![Selection_002](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/69544149-3925-4dc7-ad4e-4e935a847378)
### EMPLOYEE_ZIP table:
![Selection_003](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/5d3a924f-9671-4480-aadd-f55d23cf653f)
# Boyce Codd Normal Form
### BCNF (Boyce Codd Normal Form) is the advanced version of 3NF. A table is in BCNF if every functional dependency X->Y, X is the super key of the table. For BCNF, the table should be in 3NF, and for every FD. LHS is super key.

## Example
### Consider a relation R with attributes (student, subject, teacher).
![Selection_004](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/0064e788-56ae-4568-bd5b-743859466d44)
### F: { (student, Teacher) -> subject
### (student, subject) -> Teacher
### Teacher -> subject}
### Candidate keys are (student, teacher) and (student, subject).
### The above relation is in 3NF [since there is no transitive dependency]. A relation R is in BCNF if for every non-trivial FD X->Y, X must be a key.
### The above relation is not in BCNF, because in the FD (teacher->subject), teacher is not a key. This relation suffers with anomalies −
### For example, if we try to delete the student Subbu, we will lose the information that R. Prasad teaches C. These difficulties are caused by the fact the teacher is determinant but not a candidate key.
### Decomposition for BCNF
### Teacher-> subject violates BCNF [since teacher is not a candidate key].
### If X->Y violates BCNF then divide R into R1(X, Y) and R2(R-Y).
### So R is divided into two relations R1(Teacher, subject) and R2(student, Teacher).
## R1
![Selection_005](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/088e84a6-8e4f-4bab-b8f4-b823c08dc206)
## R2
![Selection_006](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/470440eb-08b2-4e8a-8e07-59a949fddd3f)
# Fourth Nomrmal Form
### Fourth Normal Form contains no non-trivial multivaued dependency except candidate key. The basic condition with Fourth Normal Form is that the relation must be in BCNF.
## Example
### STUDENT
![Selection_007](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/3ee6913a-4a74-410a-a15a-b2b5e5bc7cd1)
### The given STUDENT table is in 3NF, but the COURSE and HOBBY are two independent entity. Hence, there is no relationship between COURSE and HOBBY. In the STUDENT relation, a student with STU_ID, 21 contains two courses, Computer and Math and two hobbies, Dancing and Singing. So there is a Multi-valued dependency on STU_ID, which leads to unnecessary repetition of data.

### So to make the above table into 4NF, we can decompose it into two tables:

## STUDENT_COURSE
![Selection_008](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/41cda1a5-7fd4-4108-b601-be8998af45d2)
## STUDENT_HOBBY
![Selection_009](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/d7e4ebb8-07c9-4938-9ae9-7c35bb7b0824)
# Fifth Nomral Form
### A relation is in 5NF if it is in 4NF and not contains any join dependency and joining should be lossless. 5NF is satisfied when all the tables are broken into as many tables as possible in order to avoid redundancy. 5NF is also known as Project-join normal form (PJ/NF).
## Example
![Selection_010](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/669902b6-94b7-48d3-bb41-5e8018e75ed8)
### In the above table, John takes both Computer and Math class for Semester 1 but he doesn't take Math class for Semester 2. In this case, combination of all these fields required to identify a valid data.

### Suppose we add a new Semester as Semester 3 but do not know about the subject and who will be taking that subject so we leave Lecturer and Subject as NULL. But all three columns together acts as a primary key, so we can't leave other two columns blank.

### So to make the above table into 5NF, we can decompose it into three relations P1, P2 & P3:

## P1
![Selection_011](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/e59b7b27-33d7-430e-8058-201240537269)
## P2
![Selection_012](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/1828b177-89f1-4720-a20a-427908e24049)
## R3
![Selection_013](https://github.com/Ramneet1266/rdbms_2023batch/assets/144204781/a92a62a7-e62e-41f1-999c-059a2058543b)
