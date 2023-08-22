# Modeling relationships

In this assignment, you will design a few simple database schemas. 
Each must implement and enforce a set of rules. 
Your design tables, their primary keys, and foreign keys to enforce each of the rules.
Some tables may require an additional unique index. 
You are not required to populate these tables but you should try breaking some of the rules to ensure that you have implemented all the constraints.
You must define these schemas in the database under the specified names.
The score for each problem is the number of rules that the schema correctly enforces.

## Bookstore `<username>_bookstore`

Create a database to keep track of each copy of a collection of book titles in your bookstore.  

1. Book titles are identified by their ISBN.
2. Your store may have several copies under the same title.


## States and capitals `<username>_states`
Model cities, states, and capitals:
1. Each city belongs to one state.
2. Each state has one capital.
3. A capital is a city.
4. A capital must be in the same state.


## Tennis club `<username>_tennis`
Model a tennis club that has courts, members, and 1-hour reservations.

1. The club has several courts identified by letters: A, B, C, D.
2. The club has members identified by the phone numbers.  Two members may have the same names.
3. A member can reserve a court for a 1-hour session starting at the top of the hour.
4. A member cannot reserve more than one court for the same hour.
5. No two members can reserve the same court for the same hour.


## Chess tournament `<username>_chess`
Model the chess games between members of your chess clubs.

1. Club members are identified by a 12-character nickname 
2. Each game has two players: one playing white and the other black.
2. Each game has a start date/time and an end date/time.
3. Each game also has one of four possible outcomes: white wins, black wins, draw, or aborted.

## Payments `<username>_payments`

Create a database of users with their payment methods.

1. Users are identified by their user names
2. Users have names and emails; no two users can share the same email. 
2. User may have one or more payment methods.
2. A payment method is identified by a 16-bit credit card number and has a requird  expiration date.
2. If a user has any payment methods, one them must be designated as the default payment methods. A user cannot have more than one default payment methods.

## Image labels `<username>_recognition`

In a distopian universe, create a database of images and the identity of people recognized in each image.

1. You have several security cameras labeled A, B, C, D.
2. The cameras take pictures identified by their camera and a timestamp. 
1. You have a collection of people identified by their implanted RFID chip numbers. People have no names.
2. Each  person can have any any combination of the following skills:  hunt, forage, and fight.
2. For each image, the database identifies all the people who were recognized in it by the face recognition algorithm.

