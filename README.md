# query-search
Refer to readme file.


Documentation
Creating a web-app for implementing queries in a database (with autahentication)
## Introduction
To add data in a database and perform query searches on it. Only authorised users can access the database.
(For example: Village head cannot access the data of people of a district, but only the data of his/her village.)
Creating  front-end and back-end parts of the web-app; This implements accessing data from database using queries.

## Contents
1.	Add data in the database (using MongoDB).
2.	Add code for different parameters that access data with specific conditions (i.e. implementing queries).
3.	Write back-end code for accessing data through server.
4.	Add authentication to limit access of data to authorised users only (using login system).
5.	Create front-end part to provide user with ease of access for viewing data in a well formatted form.

## Adding Data to Database
•	Adding raw data in database of a MongoDB server
•	To add data :
1.	Connecting to a MongoDB server.
2.	Creating an object prototype with key-value pairs that will have all attributes of data as well as required constraints for each attribute. 
(For example: Phone number attribute will check number of characters entered and will only allow numbers. Name field cannot be left null.)
3.	Each entry will have a unique object in Mongo-DB server with a unique object ID.
Additional feature: Add/Update/Delete data directly from website.

## Implementing queries
1.	Adding techniques provided by MongoDB/Mongoose to access database in multiple ways.
2.	Adding techniques to search multiple queries at once.
(For example: To find names of all males in a village whose age is greater than 25).
3.	Add test cases to check if all queries are running properly under all conditions.
4.	In case of any error, the user will get a well formatted message.

## Writing Back-end code
1.	Creating a new express server.
2.	Adding required methods to easily connect back-end and front-end part of the web-app (by using node modules like Handlebars).
3.	Writing test cases to verify that server never fails.
4.	Write code that can be de-bugged easily and adding new features in future will become easy.
5.	Deploying the server online for live access

## Adding authentication
1.	Adding authentication by using a login system.
2.	Login system using specific Username and Password
3.	On a successful login, a token will be returned to the user.
4.	 This token will be sent with each request in database made by the user. This ensures all requests are authorised.
5.	On a failed login attempt, user will be notified that the username/password entered is incorrect.
6.	On logging out, the token is deleted.
7.	This will be implemented by using JWT (JSON Web Tokens) and hashing algorithms.
8.	Adding test-cases to check that no un-authorised user is able to access data and make any changes to it.
9.	Integrating authentication with express server and with mongoDB code.
## Adding front-end part of web-app
1.	Creating a new login page that has username and password fields and a login button.
2.	On successful login, user is taken to a new page where he/she can:
•	View the whole database that they have been authenticated the access to.
•	Implement queries by using various drop down menus and text-fields.
•	Send the request to server.
•	Server returns the data and it is viewed in a well formatted way. 

3.	On a failed login attempt, user is notified about it and asked to retry with the correct username/password.
4.	Once logged in, user can logout using logout button that is visible on right top of the screen.
5.	Integrating the front-end code with express using handle-bars.
6.	Making sure an invalid request of any type returns a well formatted output that informs user about it.

## Overview
A web-app to implement query searching in a database has to be created with working test-cases.
Authentication is needed to access the data.
Both front-end and back-end are wired for implementing the same.
## Tech-stack
Javascript, NodeJS, HTML, CSS, BOOTSRAP, MongoDB (Mongoose) and various NPM modules. (For eg: Mocha for testing, JWT for authentication, Handlebars for integrating front-end with express).


