# More Complex Queries

In this assignment, you will make queries from shared databases:
1. Sakila database: `shared_sakila`
2. Sales database: `shared_sales`
3. Airport database: `shared_airport`

Write all queries in SQL. Use `SHOW TABLES` and `SHOW CREATE TABLE` statements to understand the schema.

The queries may be simple single-table `SELECT` statements, `SELECT` statements with subqueries, or queries with inner joins, or queries with left joins and GROUP BY. 

Some of the problems are very difficult. Please work on these problems early and bring your questions to class. You are welcome to work in groups but produce and submit your solutions individually.


## Sakila


1. List the names of all actors who have co-starred in the same movies with NATALIE HOPKINS.

2. List the pairs of actors and the number of films they have been in together.  Show only the top ten 10 pairs.

3. List the titles of all films on the inventory of Store 2 only, i.e. not found in Store 1.



## Sales 

4. List employees along with the their ages in years today. (Hint: Use the `DATEDIFF` or `TIMESTAMPDIFF` function along with `NOW()`).)

5. List all employees with November birthdays. (HINT: Use the `MONTH` function)

6. List all orders placed by employees on their own birthdays. (HINT: You may use the `MONTH` and `DAYOFMONTH` functions)

7. Show the date with highest number of orders placed.

8. List all days of the year (month and day only) of employee birthdays.

9. List the names of Products that are offered by only a single vendor, including the name of that vendor. 

10. List all products, including the name of the vendor that offers it at the lowest price.

11. List all unique  pairs of orders that have the same date, customer, and employee. (Hint: 10 pairs)

12. Challenge: show all the triplets of products that appear together on at least 100 unique orders. (Hint: 5 triplets)

13. Challenge: Find the most common list of products on an order  (Hint: The same list of 8 products is found on 23 orders. You may find the `GROUP_CONCAT` function helpful. Note that it has an `ORDER_BY` option).



## Airport
14. Find the passengers who have never flown.  (This may a couple of minutes since the data size is big).

15. For each airline, show the number of airports they fly to or from.

16. List pairs of airlines and the number of airports that they share, limit to the top 10 most connected airlines. 
