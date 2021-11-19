# Database design project:  The Car Sharing App

Design the database to support a car sharing service with the following rules. 
This may be similar to the car sharing service  **Turo** or  RV sharing service **Outdoorsy**.

## Business Rules

0. The app allows users to register so that they can either rent out their own cars or rent other people's cars.
1. A user can register one or more of her own cars to share with others.
2. The car information must includes VIN, make, model, year, body type, fuel type, number seats, trunk size, and fuel economy (in MPG). 
3. Some users can register as drivers, in which case they need to provide their drivers license, sex, and date of birth.
4. A car owner can make her car available for rental  any day, specifying the price for each day, the free miles per day, and the price for extra miles. 
5. A driver may reserve a car for any trip period from a start date to an end date if the car is available for each of the included dates. 
6. All cars are equipped with locks that can be opened by the smartphone app. Upon completing the trip, the app records the completed trip, and the miles traveled.

You can add additional rules and assumption as  you find necessary, providing an explanation.


## Database design

Design the relational  database to support the app following the rules of data normalization learned in class.

## Populate initial data

1. User the `faker` module to populate at least 500 users. 
2. Add 300 cars owned by some of the user. A user may own multiple cars. You can use the `faker_vehicle` plugin of the `faker` module. https://pypi.org/project/faker-vehicle/
3. Designate some users as drivers and provide their drivers license information. 
4. Make some cars available for rental for some dates between Dec 1, 2021 and Jan 31, 2022.  Have at least 6000 car days available.

## Functions 

1. Write the function `get_available_cars` that returns the list of cars available for rental and not already reserved. 
2. Write the function `reserve_car` that creates a reservation with a start date and an end date. 
3. Write the function `start_trip` and `complete_trip` 

## Operations

1. Generate at least 300 reservations
2. Generate at least 200 completed trips 

## Queries

1. List all drivers who have reserved a car between Christmas and New Years. 
2. Pick one car and show all the drivers who have rented it. 
2. List all drivers who have rented a car before they turned 25 yo.
3. List all male drivers aged 65 and over.
4. List the total number of cars available and not yet reserved for each night at a price under $50 and seating at least four people.
5. List all completed trips and the amount  owed  based on the mileage logged and the prices provided.
6. Show the car makes sorted by the number of reservations.
7. For each driver, show the total miles driven in their completed trips.
