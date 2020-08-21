# Chapter - 5 RDBMS

RDBMS stands for Relational Database Management Systems. All modern database management systems like SQL, MS SQL Server, IBM DB2, ORACLE, My-SQL and Microsoft Access are based on RDBMS. Data is represented in terms of tuples (rows) and attribute(column) in RDBMS. Relational database is most commonly used database. It contains number of tables and each table has its own primary key. Due to a collection of organized set of tables, data can be accessed easily in RDBMS.

The RDBMS database uses tables also known as relations to store data. A table is a collection of related data entries and contains rows and columns to store data. A table is the simplest example of data storage in RDBMS.

## Normalization
Normalization is the process of organizing the data in the database. Normalization is used to minimize the redundancy(duplicacy) from a relation or set of relations. It is also used to eliminate the undesirable characteristics like Insertion, Update and Deletion Anomalies. Normalization divides the larger table into the smaller table and links them using relationship. There are four types of normal forms:

<img src="https://www.gatevidyalay.com/wp-content/uploads/2018/04/Normal-Forms-in-DBMS.png" height="" width="">

### 1. First Normal Form (1NF)
A relation will be 1NF if it contains an atomic value.
It states that an attribute of a table cannot hold multiple values. It must hold only single-valued attribute. First normal form disallows the multi-valued attribute, composite attribute, and their combinations. In 1NF every column should contain the value of the same domain and order of rows and column are irrelevant.

**Example**: Relation EMPLOYEE is not in 1NF because of multi-valued attribute EMP_PHONE.

<img src="https://user-images.githubusercontent.com/54719422/90362135-854a6300-e07d-11ea-9f6d-2d288ec45294.png" height="" width="">

### 2. Second Normal Form (2NF)
In the 2NF, relational must be in 1NF. In the second normal form, all non-key attributes are fully functional dependent on the primary key.

**Example**: Let's assume, a school can store the data of teachers and the subjects they teach. In a school, a teacher can teach more than one subject.

<img src="https://user-images.githubusercontent.com/54719422/90361730-93e44a80-e07c-11ea-977d-68118442d769.png" height="" width=""><img src="https://user-images.githubusercontent.com/54719422/90361776-aeb6bf00-e07c-11ea-9235-951ae1443393.png" height="" width="">

### 3. Third Normal Form (3NF)
A relation will be in 3NF if it is in 2NF and not contain any transitive partial dependency.
3NF is used to reduce the data duplication. It is also used to achieve the data integrity. If there is no transitive dependency for non-prime attributes, then the relation must be in third normal form.

**Example**: Let's have a Employee details table of a company which contains complete imformation of the employee.

<img src="https://user-images.githubusercontent.com/54719422/90362383-1d484c80-e07e-11ea-90c4-d907ef9956eb.png" height="" width="">

Super key in the table above:

>{EMP_ID}, {EMP_ID, EMP_NAME}, {EMP_ID, EMP_NAME, EMP_ZIP}....so on  

Candidate key: 
>{EMP_ID}

Non-prime attributes: 
> all attributes except EMP_ID are non-prime.

Here, EMP_STATE & EMP_CITY dependent on EMP_ZIP and EMP_ZIP dependent on EMP_ID. The non-prime attributes (EMP_STATE, EMP_CITY) transitively dependent on super key(EMP_ID). It violates the rule of third normal form.

That's why we need to move the EMP_CITY and EMP_STATE to the new <EMPLOYEE_ZIP> table, with EMP_ZIP as a Primary key.

<img src="https://user-images.githubusercontent.com/54719422/90362499-67313280-e07e-11ea-8986-71f361b23303.png" height="" width="">

### 4. Boyce Codd normal form (BCNF)
BCNF is the advance version of 3NF. It is stricter than 3NF. A table is in BCNF if every functional dependency X → Y, X is the super key of the table.
For BCNF, the table should be in 3NF, and for every FD, LHS is super key.

Example: Let's assume there is a company where employees work in more than one department.

<img src="https://user-images.githubusercontent.com/54719422/90363160-c6dc0d80-e07f-11ea-9999-7e8d101944b2.png" height="" width="">

Functional dependencies are as follows:

>EMP_ID  →  EMP_COUNTRY  
EMP_DEPT  →   {DEPT_TYPE, EMP_DEPT_NO}  

Candidate key:
> {EMP-ID, EMP-DEPT}

The table is not in BCNF because neither EMP_DEPT nor EMP_ID alone are keys.

To convert the given table into BCNF, we decompose it into three tables:

<img src="https://user-images.githubusercontent.com/54719422/90363161-c80d3a80-e07f-11ea-85e5-9879ca2ea563.png" height="" width="">

Functional dependencies:

>EMP_ID   →    EMP_COUNTRY  
EMP_DEPT   →   {DEPT_TYPE, EMP_DEPT_NO}  

Candidate keys:

>For the first table: EMP_ID                           
For the second table: EMP_DEPT          
For the third table: {EMP_ID, EMP_DEPT}

Now, this is in BCNF because left side part of both the functional dependencies is a key.

## Joins

A SQL Join statement is used to combine data or rows from two or more tables based on a common field between them. Types of joins are shown below in picture:

<p align="center"><img src="https://cdn.mindmajix.com/blog/images/db-01_2119.png" height="300" width="400"></p>

##  Advance Database Applications
 Below are some of the applications of advance database:

### 1. Geographic Information Systems (GIS)
 
 A geographic information system (GIS) is a framework for gathering, managing, and analyzing data. Rooted in the science of geography, GIS integrates many types of data. It analyzes spatial location and organizes layers of information into visualizations using maps and 3D scenes.

<p align="center"><img src="https://media.nationalgeographic.org/assets/photos/000/322/32282.jpg" height="300" width="400"></p>


### 2. Computer Aided Design(CAD)

 CAD software is used to increase the productivity of the designer, improve the quality of design, improve communications through documentation, and to create a database for manufacturing. CAD output is often in the form of electronic files for print, machining, or other manufacturing operations.

 <p align="center"><img src="https://image.slidesharecdn.com/cadandcam-130913120130-phpapp02/95/cad-and-cam-7-638.jpg?cb=1379073734" height="300" width="350"></p>


### 3. Network Management System(NMS)
 An NMS is a system designed for monitoring, maintaining, and optimizing a network. It includes both hardware and software, but most often an NMS refers to the software used to manage a network.

 <p align="center"><img src="https://www.lantechcom.co.za/global/eng/Support/img/TT_SNMP1.png" height="300" width="350"></p>


### 4. Customer Relationship Management system (CRM)

 A  is another example of a database application that has been customized to manage the marketing, sales, and support relationships between a business and it's customers. The ultimate goal is to maximize sales, minimize costs and foster strategic customer relationships.

 <p align="center"><img src="https://www.engagebay.com/blog/wp-content/uploads/2019/01/CRM-Database-Cover-960x675.jpg" height="300" width="350"></p>


## Limitations of RDBMS
Relational Database Management System is very useful in DBMS. However, it does have some disadvantages. Some of those are as follows:
### 1. The abundance of information
 The advances in the complexity of the information can cause drawbacks for the relational database management system. Relational databases are designed in order to organize the data with the use of common characteristics. 

 ### 2. Structure limits
  This is another limitation as some of the relational databases have limits on the length of the field. Some of the search queries and names are shorter as compared to their actual position. This can lead to the loss of the data. 
 ### 3. Cost
  One of the main disadvantages of the relational database management system is high cost. The relational databases are expensive to set up and also the maintenance of the databases is also expensive. 
  
### 4. Isolated information
   Because the relational databases use a large number of tables, there are higher chances that some information can be forgotten when it is transformed from one location to another location. This is the main problem in the large-scale organization in which there is a large amount of data of the employees, accounts and financial data. Isolation of information problem arises when the organization has different database systems.

   ## Summary

   Above we discussed about the relational data management system(RDBMS), types of normalization, types of joins, advanced database application, limitations of RDBMS.

   In the next chapter, we will discuss about Extensions of DBMS.
