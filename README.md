# Database-Systems-for-Data-Science (Fall 2022)
**MS Applied Data Science**

**Instructor:** Dimitri Yatsenko, Ph.D.

**TA:** Juan Gallegos

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


## Weeks 1-2: (Aug 23, Aug 30)
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


### Homework 1 (due Sep 6): 

0. Readings: 
  * Harrington, Chapter 1, "The Database Environment"
  * Hernandez, Chapter 1, "The Relational Database" 
1. Answer questions in [Block1.md](Block 1). Submit as a PDF file as a direct message to the TA and the instructor on Slack.  
1. [Installation of SQL Magic for Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Install-SQL-Magic.ipynb)
2. [Connecting to the database from Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Connect-SQL.ipynb)
2. On the MySQL server, create a database named `<username>_university` and define a table named `person`. Make sure it has a well chosen primary key. 

### Homework 2 (due Sep 13)

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

## Weeks 3-5: (Sep 6, Sep 13, Sep 20)

September 14 was cancelled due to Tropical Storm Nicholas.

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
  * https://www.datajoint.com/blog/2021-09-28-data-needs-direction

[Assignment 3](Assign3.md) -- Due Sep 28

### Online exercises
* http://www.w3resource.com/mysql-exercises/ 
* http://www.w3resource.com/sql-exercises/

[Assignment 4](Assign4.md) -- Due Oct 7

## Weeks 6-8 (Oct 5 - off, Oct 12, Oct 19, Oct 26)

Surrogate keys / Natural keys. 
Indexes, secondary unique keys.
Data serialization - blobs.

Notebooks 
* [Joins](notebooks/Joins.ipynb)
* [GroupBy](notebooks/GroupBy.ipynb)

Advanced Queries: 

* Subqueries
* Inner Joins: cross join, theta join, equijoin, natural join
* Aggregations 

Reading: Harrington  Chapters 16-19

* [Assignment 5](Assign5.md) -- Due Oct 26
* [Assignment 6](Assign6.md) -- Due Nov 3
* [Assignment 7](Assign7.md) -- Due Nov 10

## Weeks 9, 10 (Nov 2, Nov 9)

Nov 2: Lecture will start at 7.30 pm. 

Modeling relationships: 

* Sequences and workflows.
* Specialization / generalization.
* Hierarchies (ownership, composite keys, partial keys)
* Groupings 
* Directed Graphs (including trees)
* Unidrected Graphs.
* Master-part relationships

Transactional processing. Computations.

Reading: 

* Harrington: Chapters 13, 14, 15 (case studies), 22 (concurrency and transactions)


## Weeks 10-11 (Nov 16, Nov 23):
Putting it all together. Practical examples

* [Assignment 8](Assign8.md) -- Due Nov 18
* [Assignment 9](Final.md) -- Due Dec 12 

Practice projects. Final Project
