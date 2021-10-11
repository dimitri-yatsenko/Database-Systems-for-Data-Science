## Homework 4

For this assignment, you will separate into groups of three. You will get full access to schemas with the prefix `hw4_team#_` where `#` is your team number.
The team organization will be listed in the schema `shared_teams`.

Design, populate, and query a database for a hotel reservation system with the following business rules:

1. The hotel has a number of rooms of two types: Deluxe and Suite
2. For every night, some rooms are made available for reservation for a specific price.
3. A guest can make a reservation for an avavilable room for one night. The reservation must include credit card payment info. At most one reservation can be made per night per room.
4. A guest can check into a room that has been reserved. An attempt to check in without a reservation will generate an error.
5. A guest can check out only after checking in. An attempt to check out multiple times or check out without checking in will generate an error.

Your Python code should provide the following:

  a. A section to create the tables. The design must be in 3rd normal form following the conventions discussed in class and enforcing the business rules above.

  b. Provide code to populate rooms and room availability with prices.

c. The function `reserve_room(room, date, guest_name, credit_card)` to make a reservation. A script that populates at least 300 reservations (e.g. use `faker`)

d. The functions `checkin(room, date)` and `checkout(room, date)` to check guests in and out. Write a script that invokes `checkin` and `checkout` for a buncha guests.  Demonstrate that that the functions enforces the rules of the business.

e. Write a query to list all guests who have stayed in a given room in 2021.

f. Write a query to list all dates on which a specific guest stayed at the hotel.



