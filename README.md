# BookMyShow

# Problem Statement:
Build a movie show booking system that allows a user to browse the movies in his/her city and book a show

# Requirements:
  Once customer sign in to BMS system and click book tickets for a movie in his city. The customer will be able to select the show and make booking,
  Then Booking manager handles movie ticket booking and also communicates with other services like Account, Payment, MovieShow for required information.


# New Version (Only Ticket Booking system in BMS)
  
  # Account Manager
  
    1. Responsible for providing user account details like user city, name etc.
    2. Also manages registration and login of user
    3. Manages different types of users like BMS customer, BMS Admin, Theatre Owner etc.
  
  # Show/Ticket Booking Manager
    
    1. Handles all movie show bookings
    2. Manages booking information of customers
  
  # Payment Manager
    Handles customer ticket booking payments for this system.
    
    However it can also do below actions
      1. Handles all types of payments
      2. Also manages payments for Book My Show employees
      3. And deals payments between BookMyShow and Theatre owners
  
  # Strategy Manager
     Manages all strategies and helps other managers with deciding pricing or payment or any other strategy.
  
  # Movie Show Manager
     1. Manages all movie shows running in a city for each day.
     2. Also provides seat details (like seat type and pricing)


# Design patterns can be used:
  1. Theatres or Seats creation (Factory pattern)
  2. Ticket Pricing (Strategy or Decorator Pattern)
  3. Movie filters (Strategy Pattern)
  4. Search Movies or Events (Strategy Pattern)
  5. Payment handling (Strategy Pattern)


# Version 1: Whole system (High level)
  Book my show system features:
  
    1. Register a user (can be a customer or theatre owner or bookmyshow admin)
    2. System should preselect city for movies/events to list out
    3. BookMyShow admin can list or delist movies/events into the system
    4. BookMyShow admin can add more cities into the system
    5. Theatre owner should signin and add movie shows or screens into the system
    6. Theatre owner can also delist the shows or cancel the shows
    7. BookMyShow admin can support both customers or theatre owners with onbaording or resolving the issues
    8. Customer can search for movies/events running in a particular city and book the tickets for a particular show
    9. Customer can filter the movies/events by language or genre or format
    10.System can show recommendations to the customers based on their past browsing experience with the site/BMS system
 
# Responsibilities of each entity in BookMyShow System:

1. Customer
  - Register and signin 
  - Search movie and theatre
  - Filter movies by rating, language, genre, format etc (strategy pattern)
  - Book a movie show with desired number of seats
  - See all his/her bookings for a particular date
  - Add the review for a movie
 
2. Theatre Owner
  - Add or remove movie shows
  - Cancel a movie show
  - Add pr remove screens
  - Add or remove seats for a particular show

3. BookMyShow Admin
  - Add or remove city
  - Add or remove theatre in a city or list of cities
  
4. System
  - Onboard users
  - Fetch the list of cities
  - Fetch the list of movies
  - Fetch the list of movie shows
  - Fetch the bookings of a particular user
  - Availability of seats for a particular show
  - Generate refund for cancelled shows
  - Generate ticket
  

# Actors:
1. Customer
2. TheatreOwner
3. BookMyShowAdmin
4. System

# Models:
1. User
2. Movie
3. Theatre
4. Screen
5. Seat
6. Review
7. City
8. Payment
9. Account
10. Booking
11. MovieTicket
12. Location

# Constants:
1. Gender
2. Genre
3. SeatType
4. AccountStatus
