# BookMyShow



# Requirements

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
