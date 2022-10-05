# Cinema project
<br/>**Project description:**
<br/> A simple web application, which has been written using Spring technologies, that supports authentication, authorization, and CRUD operations(see project's features). 
<br/>
<br/>**Features:**
<br/>:arrow_forward: Authentication, authorization and creating of new users;
<br/>:arrow_forward: Assigning specific roles(USER, ADMIN);
<br/>:arrow_forward: Adding new movies and cinema halls;
<br/>:arrow_forward: Combining movies and cinema halls in movie sessions;
<br/>:arrow_forward: Adding movie sessions to a ticket;
<br/>:arrow_forward: Adding tickets to shopping carts of a specific user;
<br/>:arrow_forward: Completing an order by adding all needed information to it;
<br/>:arrow_forward: Role access to specific resources for ADMIN and for USER is configured using the following rules:
<br/>
- POST:   /register - all
- GET:    /cinema-halls - user/admin
- POST:   /cinema-halls - admin
- GET:    /movies - user/admin
- POST:   /movies - admin
- GET:    /movie-sessions/available - user/admin
- POST:   /movie-sessions - admin
- PUT:    /movie-sessions/{id} - admin
- DELETE: /movie-sessions/{id} - admin
- GET:    /orders - user
- POST:   /orders/complete - user
- PUT:    /shopping-carts/movie-sessions - user
- GET:    /shopping-carts/by-user - user
- GET:    /users/by-email - admin

<br/>**Database structure:**
![schema_dependencies](https://user-images.githubusercontent.com/101473233/193642813-f8e6af1d-599d-457a-b03a-b0b82817dccf.png)

<br/>**Technologies that were used in the project:**
<br/>- Java (11);
<br/>- Apache Tomcat;
<br/>- MySQL;
<br/>- Hibernate;
<br/>- Spring Core;
<br/>- Spring MVC;
<br/>- Maven;
<br/>- Spring Security.
<br/>:eyes: **How to run the project:**
- You will need an installed environment to run Java code;
- You will also need installed MySQL and Apache Tomcat;
- Clone this project
- Set up DB's parameters in db.properties
- Run the Apache Tomcat.
- You can use already initialized data(from DataInitializer)
