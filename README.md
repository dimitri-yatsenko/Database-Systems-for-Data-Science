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

### Weeks 4-6 (Sep 8, 15, 22)
Querying databases from a host programming language for data analysis (Python).
Client interfaces.  Work with individual tables: `CREATE`/`DROP` `INSERT`, `DELETE`, `UPDATE`, and `SELECT` statements.

**Assignments:**
You are welcome to use any SQL client to connect to the database as discussed in class. I recommend using Jupyter for ease of interaction.

1. [Installation of SQL Magic for Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Install-SQL-Magic.ipynb)
2. [Connecting to the database from Jupyter](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Connect-SQL.ipynb)
3. [Assignment 1](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Assign-01.ipynb)
4. [Question Block1](Block1.md)
5. [Assignment 2](Assign2.md)
6. [Assignment 3](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Assign-03.ipynb)
7. [Assignment 4](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Assign-04.ipynb)


### Weeks 7-8 (Sep 29, Oct 6)
Database design from conceptual modeling to implementation.
Data integrity. Database normalization.

### Week 9 (Oct 13) - No class - Fall Break

### Week 10-12 (Oct 20, Oct 27, Nov 3) 
Advanced database design and queries. Modeling complex relationships. Multi-table queries.

[Assignment 5](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Assign-05.ipynb)
Due Nov 12.

Indexes. 

Multi-table queries. Summarizing data. Using `LEFT JOIN` in conjunction  with `GROUP BY` and  the `HAVING` clause.

Assignment 6. "Problems for you to solve" from Chapters 12, 13, and 14. Due Nov 12.
[Assignment 5](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Assign-06.ipynb)
Due Nov 12.




### Weeks 13-15 (Nov 12, 19, 26)

Final Project -- group or individual.

1. The project must include a database of sufficient complexity: at least 5 related tables. Produce a diagram of your schema.
2. Design an original database schema using principles and techniques from the course.
3. Write a Python script to populate the database and to model common scenarios for data entry
4. Write at least ten interesting, complex queries, including joins, subqueries, and aggregation functions.
5. Present in class

Execute all code in each person's database account. Students do not have access to one another's databases. 


For the group project, the group has tentatively selected the Jeoparty dataset as the basis for the database, available here: https://github.com/jwolle1/jeopardy_clue_dataset

In a subsequent group meeting, the team chose to implement a Customer Relationship Management system. 



