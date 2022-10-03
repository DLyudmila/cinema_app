# Cinema project
Project's description
A simple web application, which ahs been written using Spring technologies, that supports authentication, authorization, and CRUD operations(see project's features).

Project's features
Authentication, authorization and creating of new users;
Assigning specific roles(USER, ADMIN);
Adding new movies and cinema halls;
Combining movies and cinema halls in movie sessions;
Adding movie sessions to a ticket;
Adding tickets to shopping carts of a specific user;
Completing an order by adding all needed information to it;
Role access to specific resources for ADMIN and for USER is configured using the following rules:

POST:   /register - all
GET:    /cinema-halls - user/admin
POST:   /cinema-halls - admin
GET:    /movies - user/admin
POST:   /movies - admin
GET:    /movie-sessions/available - user/admin
POST:   /movie-sessions - admin
PUT:    /movie-sessions/{id} - admin
DELETE: /movie-sessions/{id} - admin
GET:    /orders - user
POST:   /orders/complete - user
PUT:    /shopping-carts/movie-sessions - user
GET:    /shopping-carts/by-user - user
GET:    /users/by-email - admin

Database structure:
![schema_dependencies](https://user-images.githubusercontent.com/101473233/193642813-f8e6af1d-599d-457a-b03a-b0b82817dccf.png)

Following technologies that have been applied in this project:
Java (11);
Apache Tomcat;
MySQL;
Hibernate;
Spring Core;
Spring MVC;
Spring Security.
How to run this project on your PC:
You will need an installed environment to run Java code;
You will also need installed MySQL and Apache Tomcat;
Clone this project
Set up DB's parameters in db.properties
Run the Apache Tomcat.
You can use already initialized data(from DataInitializer)
