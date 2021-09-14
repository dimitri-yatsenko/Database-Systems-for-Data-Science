# Database-Systems-for-Data-Science (Fall 2021)
**MS Applied Data Science**

**Instructor:** Dimitri Yatsenko, Ph.D.

**TA:** Cinni Patel

## Syllabus

Organization concepts and terminology of data models and the underlying data architectures needed to support them. 
Presentation of the relational database management systems including an introduction to SQL programming: relational database design and data queries with integration into application programming languages, with Python used for examples. 

I will assume basic Python proficiency: we want to use databases directly from Python. 

The course will include practical exercises and will be graded based on several indvidual and group projects using real-world datasets.

## Class and attendance

Class participation is required and much of the material will be presented. The class will be held in room SHP 251 and also broadcast in Zoom.
We will also use a Slack channel. If you have not received access to any of these resources, please notify your instructor.

## Textbook 

The University provided you with a [Safari Books](https://www.oreilly.com) subscription account. Readings, examples, and projects will be selected primarily from the following references:

1. Jan L. Harrington, *Relational Database Design and Implementation*: 4th edition (2016)

  * https://learning.oreilly.com/library/view/relational-database-design/9780128499023/

2. Alan Beaulieu, Learning SQL, 3rd Edition (2020)

  * https://learning.oreilly.com/library/view/learning-sql-3rd/9781492057604/

3. Michael Hernandez, *Database Design for Mere Mortals: A Hands-On Guide to Relational Database Design*; 4th edition (2020).  ISBN-13: 978-0136788041 ISBN-10: 0136788041

  * https://learning.oreilly.com/library/view/database-design-for/9780136788133/

4. Josephine Bush, *Learn SQL Database Programming* (2020)

  * https://learning.oreilly.com/library/view/learn-sql-database/9781838984762/

Additional slides and notes will be provided in class.


## Grading 
8 Assignments/Projects

|grade| percent |
|---|---|
|**A** |>=94%|
|**A-**|>=90%|
|**B+**|>=86%|
|**B**|>=82%|
|**B-**|>=78%|
|**C+**|>=74%|
|**C**|>=70%|
|**C-**|>=66%|
|**D+**|>=62%|
|**D**|>=58%|
|**F**|>=0%|


## Weeks 1-2: (Aug 24, Aug 31)
Databases in data science. Data models: diverse ways to think about data: hiearchical, network, relational, object, graph, and document data models.
History of datatabases and database technologies. Next-generation databases.

Database access. Creating SQL tables and inserting data. Simple queries. sqlite and mysql.

Issue SQL queries from Jupyter using SQL Magic.

Issuing SQL queries from Python code using a database client library, (`pymysql`). 

`CREATE SCHEMA`, `CREATE TABLE`, `INSERT`, `DELETE`, `DROP TABLE`, `DROP SCHEMA`. 

Create schemas and tables, insert rows, delete, and drop.

Using the `faker` module to populate tables.

Using `datajoint` as a high-level interface. 

Datatypes: numerical, character strings, and enum. 

Primary key. 


### Homework 1 (due Sep 7): 

0. Readings: 
  * Harrington, Chapter 1, "The Database Environment"
  * Hernandez, Chapter 1, "The Relational Database" 
1. Answer questions in [Block1.md](Block 1). Submit as a PDF file as a direct message to the TA and the instructor on Slack.  
1. [Installation of SQL Magic for Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Install-SQL-Magic.ipynb)
2. [Connecting to the database from Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Connect-SQL.ipynb)
2. On the MySQL server, create a database named `<username>_university` and define a table named `person`. Make sure it has a well chosen primary key. 

### Homework 2 (due Sep 14)

0. Readings:
  * Beauliue, Chapter 2: "Creating and Populating a Database"
  * Generating fake data: https://towardsdatascience.com/generating-fake-data-with-python-c7a32c631b2a
1. Create a `university` database 
2. Create a table named `person` with basic attributes: name, date of birth, address, phone, 
3. Using the `faker` module, populate the `person` table with 3000 records.


### Key terms
Database, database system, database server, data model, data integrity, data consistency, ACID, relational data model, SQL, imperative queries, schema.

### Key skills
* Connect to the MySQL database provided for the class, create a simple table, and insert data into it.
* Issue queries in SQL (using the SQL magic in jupyter for quick SQL scripting) 
* Execute queries with a client library (`pymysql`). Generate fake data. See notebook `Fake-It.ipynb`
* Execute queries using DataJoint. See notebooks `DataJoint-config` and `DataJoint-Intro`.

## Weeks 3-4: (Sep 7, Sep 14)

### Key concepts 

* Data models: structured (schema) and self-desccribing (schema-less). 
* How a database table works. 
* Schema design. Simple queries. Primary key. Foreign keys. Entity integrity. Referential integrity. 
* Normalization. First normal form.  Entity normalization.
* Diagramming. Entity-Relationship Diagrams. DataJoint diagrams. 
* See the `Language` notebook used in Lecture 3.
* Relational algebra: restriction and projection. The structure of the `SELECT` Statement.
* Fetch. Order by. Offset and Limit.
* Declarative queries vs. imperative queries
* Default values. Nullable attributes. Nullable foreign keys.
* UUID, surrogate keys, secondary unique constraints


### Readings:
  * Harrington, Chapters 3-7
  * Hernandez, Chapters 2-3
  * Beaulieu, Chapters 3-4
  * Beaulieu [Appendix A. ER Diagram](https://learning.oreilly.com/library/view/learning-sql-3rd/9781492057604/app01.html)
  * Example databases: https://dev.mysql.com/doc/index-other.html

### Homework 3  (due Sep 21)

1. Create and populate a university database that has departments, persons. Use `faker` to create at least 3000 persons. Persons must have a home address.
2. Some persons are students. Students can optionally have one major (a reference to a department).  
3. Some persons are professors. They are affiliated with one department. 
4. Write a query that shows all students with a Texas home address.
4. Submit the Python code that creates and populates the database.
5. Leave the database in place so that the instructor and TA can verify its structure and contents

### Online exercises
* http://www.w3resource.com/mysql-exercises/ 
* http://www.w3resource.com/sql-exercises/

### Homework 4 (due Sep 28)
For this assignment, you will separate into groups of three. You will get full access to schemas with the prefix `hw4_team#_` where `#` is your team number. 
The team organization will be listed in the schema `shared_teams`. 

Design, populate, and query a database for a hotel reservation system with the following business rules:

1. The hotel has a number of rooms of two types: Deluxe and Suite 
2. For every night, some rooms are made available for reservation for a specific price. 
3. A guest can make a reservation for an avavilable room for one night. The reservation must include credit card payment info. At most one reservation can be made per night per room. 
4. A guest can check into a room that has been reserved. An attempt to check in without a reservation will generate an error.
5. A guest can check out only after checking in. An attempt to check out multiple times or check out without checking in will generate an error.

Your Python code should provide the following:
* A section to create the tables. The design must be in 3rd normal form following the conventions discussed in class and enforcing the business rules above.
* Provide code to populate rooms and room availability with prices. 
* The function `reserve_room(room, date, guest_name, credit_card)` to make a reservation. A script that populates at least 300 reservations (e.g. use `faker`)
* The functions `checkin(room, date)` and `checkout(room, date)` to check guests in and out. Write a script that invokes `checkin` and `checkout` for a buncha guests.  Demonstrate that that the functions enforces the rules of the business.


## Weeks 5-6

Modeling relationships. 

## Weeks 7-8
Advanced queries.

## Weeks 9-10:
Transactional processing. Data serialization. Computations.

## Weeks 11-:
Practice projects. Final Project

