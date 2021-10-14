# Homework 5

## Simple SQL queries

This is a pure SQL assignment. Submit the assignment as PDF of the notebook using SQL Magic or as a simple text file containing the SQL code for each problem. 

We will work with two database on the server: `shared_sales` and `shared_sakila`. 

The sales database closely matches the sales database from John L. Viescas' "SQL Queries for Mere Mortals" https://learning.oreilly.com/library/view/sql-queries-for/9780134858432/ 

You can review chapters 4, 5, and 6 for additional explanations of SQL queries.

Use the SQL `SHOW SCHEMAS` and `SHOW TABLES` and `SHOW CREATE TABLE` commands to understand the structure of the data in the database.
You can use diagramming software to learn the schema. 

These queries will contain only one select statement with no joins or groupings. Some queries will require a subquery in the `WHERE` clause.

Finally, make sure that your submission is easy to understand. Include the problem statement in a comment preceding your solution.

## USE `shared_sales`

### Problem 1: 

Show the names and addresses of all employees

### Problem 2: 

Show the vendor names sorted by state and city.

### Problem 3:

Show all products with price reduced by 5%.

### Problem 4:

Show the list of orders made by each customer in descending order date. Hint: you might need to order by more than one column. You do not need to include the customers' names -- the customer ID will suffice.

### Problem 5:

List the five most expensive products.

### Problem 6: (subqueries)
List the total value of each product's stock (price x quantity)

### Problem 7: (subqueries)
List all products that have never been sold.

## Use `shared_sakila`

### Problem 8:

List all movies over 3 hours in length

### Problem 9:

List all movies containing the substring "GUMP" in them

### Problem 10:
List the last rental date for customer 148. 

### Problem 11: 

List the titles of all movies in the "Horror" category in alphabetical order

### Problem 12:

List all actors who have acted in horror movies.


