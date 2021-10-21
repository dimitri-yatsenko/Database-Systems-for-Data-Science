# Queries with inner joins

This is a group project. Query the `shared_projects` to find your teammates.

In this assignment, you will make queries from shared databases:
1. Sakila database: `shared_sakila`
2. Sales database: `shared_sales`
3. Hotel database: `shared_hotel` or any of the `hw4_*` databases submitted by teams in homework 4, even your own.

Write all queries in SQL. Use `SHOW TABLES` and `SHOW CREATE TABLE` statements to understand the schema.

The queries may be simple single-table `SELECT` statements, `SELECT` statements with subqueries, or queries with inner joins.

Some queries will require `ORDER BY` and `LIMIT` clauses but will NOT  require aggregation operators such as `MAX`, `AVG`, `SUM`, etc.

The queries will NOT require outer joins or `GROUP BY` clauses.



## Sakila

1. List all stores including their full address and their manager names. 

2. List all payments over $11.00, including the payment date, the customer name, and the staff name. 

3. List all customers who have made single payments of $11.00 or more.

## Sales 

4. Display all products and their categories

5. Display the product names, number ordered, and total  mount owed for each item  on order 160

6. Display all customers who have ever ordered a bicycle 

7. Display the names of products that have never been ordered

8. Display the names of customers who have never ordered anything

9. Show the customer/employee pairs who share the same last names

10. Show the names of all  vendors who sell clothing

11. Show all products that have not sold since the end of 2017

12. Show all product names offered by Texas vendors

13. Show the name of the  customer who ordered a bicycle most recently

14. Show the name of the vendor who sells the most expensive product


## Hotel

15. Show the rooms that have never been reserved

16. Show the names of guests who have made reservations but have not checked in.

17. Show the names of guests who have checked into Deluxe rooms and have not yet checked out.

18. Show the names of the 10 guests who checked in most recently.


