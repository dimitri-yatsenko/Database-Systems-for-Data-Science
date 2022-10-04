# Aggregation Queries

In this assignment, you will make queries from shared databases:
1. Sakila database: `shared_sakila`
2. Sales database: `shared_sales`
3. Hotel database: `shared_hotel` 
4. Airport database: `shared_airport`

Write all queries in SQL. Use `SHOW TABLES` and `SHOW CREATE TABLE` statements to understand the schema.
The queries may be simple single-table `SELECT` statements, `SELECT` statements with subqueries, or queries with inner joins, or queries with left joins and GROUP BY. 



## Sakila

1. List actor names and the total number of films they have acted in. 

2. List the top ten most rented films.

3. For each store, show the total number of rentals and the total payments received.


## Sales 

4. Count customers who live in Seattle.

5. List the average price of bikes.

6. List all vendors and the number of products they sell.

7. List all customers including the total number of orders they placed, the last date they placed an order.

9. List the top five bestselling products (based on total sales revenue). 

10. Count the orders whose total amount exceeds $500.

11. List employee names and the total  number of orders they have placed

12. List employee names and the total amounts they have made in sales.

13. List employee names and the total numbers of customers they have served.

14. For each month when sales have been made, list the total sales amounts. Hint: you may need to use the `YEAR` and `MONTH` functions.


## Hotel

15. List all the rooms and the number of times they have been rented, including those rooms that have never been rented.

16. List the average number of nights each room has been rented. 

17. List all guests, including the number of nights they have stayed at the hotel (based on reservations). 

18. List the average numbers of rooms that have been reserved on each day of the week. (Seven rows will result). Hint: first compute the totals for each date and then group by the day of the week using the `WEEKDAY` function.


