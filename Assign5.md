# Homework 5

This assignment will modify the schema design from  assignment 3 (University, Department, Student, Instructor).
The assignment must be performed in pure Python. No Jupyter magic! All SQL queries must be performed using python libraries such as `pymysql` or `datajoint`. 
You can submit pure python code or a PDF printout of the jupyter notebook implementing the solution.

The code will have three sections: 


## 1. Modified schema 

A correct design is likely to require five tables.

Rules: 
1. The University has several departments. One of them is MATH and another is BIOL, you can add a few others.
3. A person has a birthdate and a home address
2. A person in the university database can be a student, an instructor, or neither.
3. Some student student have a major and some don't. A major is a reference to a department. If a student has a major, they also a have a `declare_date`, i.e. the date when they were accepted into the program.
4. An instructor may instruct in multiple departments. 


## 2. Populate the tables 

Populate the tables with at least 3000 persons.  You may use the `faker` library. Make some of them students with and without majors. 
Make some of them instructors in one or more departments.


## 3. Write the following database queries

1. Easy: Show the names all students who are MATH majors
2. Medium: Show all persons who are neither students nor instructors. 
3. Medium: Show all persons who are both students and instructors. 
3. Medium: Show all departments that don't have any students majoring in them. 
3. Hard: Show instructors who teach in both MATH and BIOL departments. 
3. Hard: Show all students who declared their major  before age 18. 
3. Hard: Show all departments who have students declared their major before age 18.


Hints: These queries may require subqueries in their `WHERE` clauses. For date differences, please check the `DATEDIFF` function in the MySQL or MariaDB tutoral. 

If your schema design or contents do not allow answering these queries, please modify your schema design.


