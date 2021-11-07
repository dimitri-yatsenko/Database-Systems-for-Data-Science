# Aggregation Queries

This is a group project. Query the `shared_projects.group_assignement` table for `project=8`  to find your teammates.

In this assignment, you will make queries from shared databases:
1. Sakila database: `shared_sakila`
2. Sales database: `shared_sales`
3. Hotel database: `shared_hotel` or any of the `hw4_*` databases submitted by teams in homework 4, even your own.

Write all queries in SQL. Use `SHOW TABLES` and `SHOW CREATE TABLE` statements to understand the schema.

The queries may be simple single-table `SELECT` statements, `SELECT` statements with subqueries, or queries with inner joins, or queries with left joins and GROUP BY. 



## Sakila


1. List the names of top 10 actors who have acted in most films, include the number films. 

2. List the titles of all films on the inventory of Store 2 only, i.e. not found in Store 1.

3. List the names of all actors who have co-starred in the same movies with NATALIE HOPKINS.


## Sales 

4. List employees along with the their ages in years today. (Hint: Use the `DATEDIFF` or `TIMESTAMPDIFF` function along with `NOW()`).)

5. List all employees with November birthdays. (HINT: Use the `MONTH` function)

6. List all orders placed by employees on their own birthdays. (HINT: You may use the `MONTH` and `DAYOFMONTH` functions)

7. Show the date with highest number of orders placed.

8. List all days of the year (month and date)  of customer birthdays.

9. List the names of Products that are offered by only a single vendor, including the name of that vendor. 

10. List all products, including the name of the vendor that offers it at the lowest price.

11. List all unique  pairs of orders that have the same date, customer, and employee. (Hint: 10 pairs)

12. Challenge: show all the triplets of products that appear together on at least 100 unique orders. (Hint: 5 triplets)

13. Challenge: Find the most common list of products on an order  (Hint: The same list of 8 products is found on 23 orders. You may find the `GROUP_CONCAT` function helpful).




## Hotel

14. Show all guests who have made reservations for any nights when Samantha Smith made reservations.

15. Challenge: Find the pair of guests who have made reservations for the same night the most. (Hint: two of the guests have made reservations for the same nights 20 times if you are using `shared_hotels`) 


