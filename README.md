# Database-Systems-for-Data-Science (Fall 2020)
**MS Applied Data Science**

**Instructor:** Dimitri Yatsenko, Ph.D.

**TA:** Cesar Flores

## Syllabus

Organization concepts and terminology of data models and the underlying data architectures needed to support them. 
Presentation of the relational database management systems including an introduction to SQL programming: relational database design and data queries with integration into application programming languages, with Python used for examples. 

The course will include practical exercises and will be graded based on a few indvidual and group projects on real-world datasets.


**Textbook:** 
This courses focuses on learning through examples and relevant concepts will be introduced while applying them. 

We will use two practical books for learning SQL, which will provide us with examples and exercises.

Practical skills for querying (Viescas) and designing (Hernandez) relational databases: 

1. John Viescas *SQL Queries for Mere Mortals*, Addison-Wesley Professional; 4 edition (2018). ISBN-10: 0134858336, ISBN-13: 978-0134858333
2. Michael Hernandez, *Database Design for Mere Mortals: A Hands-On Guide to Relational Database Design*; 3rd edition (2013). ISBN-13: 978-0321884497, ISBN-10: 9780321884497

Not required: a more systematic and comprehensive introduction into database systems from the Computer Science undergraduate/grad perspective: 
*   Elmasri & Navathe, *Fundamentals of Database Systems* Person; 7th Edition (2015), ISBN-10: 1484213300, ISBN-13: 978-0133970777



### Weeks 1-2: (Aug 25, Sept 1)
Databases in data science. Data models: diverse ways to think about data: hiearchical, network, relational, object, graph, and document data models.
History of datatabases and database technologies. Next-generation databases.

A Taste of SQL: Database access. Creating SQL tables and inserting data. Simple queries. sqlite and mysql.

Homework 1 (due Sep 10): 

0. Chapters 1-3
1. Answer questions in [Block1.md](Block 1). Submit as a PDF file on Slack. Send a copy to the TA as well. 
1. [Installation of SQL Magic for Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Install-SQL-Magic.ipynb)
2. [Connecting to the database from Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Connect-SQL.ipynb)
2. On the MySQL server, create a database named `<username>_university` and define a table named `person`. Make sure it has a well chosen primary key. 


### Weeks 4-6 (Sep 8, 15, 22)
Querying databases from a host programming language for data analysis (Python).
Client interfaces.  Work with individual tables: `CREATE`/`DROP` `INSERT`, `DELETE`, `UPDATE`, and `SELECT` statements.

**Assignments:**
You are welcome to use any SQL client to connect to the database as discussed in class. I recommend using Jupyter for ease of interaction.

1. Chapters 4-6
5. [Assignment 2](notebooks/Assign-02.ipynb) -- Due Sep 24.  Print as PDF and send by Slack or email.

### Weeks 7-8 (Sep 29, Oct 6)
Advanced database design and queries. Modeling complex relationships. Multi-table queries.
Subqueries, joins. 
Summarizing data. Using `LEFT JOIN` in conjunction  with `GROUP BY` and  the `HAVING` clause.

6. [Assignment 3](notebooks/Assign-03.ipynb) -- Due Oct 1.  Print as PDF and send by Slack or email.
6. [Assignment 4](notebooks/Assign-04.ipynb) -- Due Oct 9.  Print as PDF and send by Slack or email.
6. [Assignment 5](notebooks/Assign-05.ipynb) -- Due Oct 21. DataJoint queries with aggregation.  Print as PDF and send by Slack or email.

### Week 9 (Oct 13) - No class - Fall Break
Database design from conceptual modeling to implementation.
Indexes. 
Data integrity. Database normalization.

### Week 10-12 (Oct 20, Oct 27, Nov 3) 
9. [Assignment 6](notebooks/Assign-06.ipynb) -- Due Oct 28. SQL queries with inner joins and subqueries.
9. [Assignment 7](notebooks/Assign-07.ipynb) -- Due Nov 12. SQL queries with LEFT JOIN, GROUP BY, and HAVING.

10. [Indexes](notebooks/Indexes.ipynb)
11. [DatabaseDesign1](notebooks/

### Weeks 13-15 (Nov 10, 17, 24)
Final Project -- group or individual.


