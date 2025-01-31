**Booking system**

**Overview**

This repository contains an Entity-Relationship (ER) model for a movie and event booking system. The system allows users to book events, make transactions, and manage event details such as movies and venues.
The ER diagram represents the relationships between the following entities:
1. Users: Users who make bookings.
2. Bookings: Records of event reservations made by users.
3. Transactions: Payments associated with bookings.
4. Events: Scheduled events that users can book.
5. Movies: Films associated with events.
6. Venues: Locations where events take place.

**Relationships:** \n
User -> Booking: One user can make multiple bookings. 
transactions -> Bookings : 1 transaction can have multiple bookings. 
Ex: A user books tickets for multiple movies or showtimes in a single payment, all those bookings should be linked to the same transaction.
Movie -> events : A movie can have multiple showtimes but each event is linked to one movie.
Venue -> events: A venue can host multiple events but an event happens at only one venue.
Events -> booking : An event can have many bookings, but one booking is for one event only.

