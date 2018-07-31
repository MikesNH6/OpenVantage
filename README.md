# OpenVantage 

This is a project intended to show simple CRUD tasks using Spring boot(API) and Angular 6(Front end)

When first opening and running the spring API please create a local database called OpenVantage and create an account with an admin username and no password. Or you could update the application properties to what suits you. Note that it will create the table and drop information once the api is restarted, you can bypass this by changing the (spring.jpa.hibernate.ddl-auto = none) that will keep the data stored in the database.

To test the API you can call it by using: (A REST client is probably a better tool to use for this.)
(GET) http://localhost:8080/api/tasks/
(GET) http://localhost:8080/api/tasks/1
(POST) http://localhost:8080/api/tasks/
(Delete) http://localhost:8080/api/tasks/delete/1
(PUT) http://localhost:8080/api/tasks/update/1

The Spring boot Api works but trying to create update and delete tasks from the Angular UI doesn't for some reason although it can query the tasks. I will be actively looking into this issue.

Make sure spring is running and the database is setup before you run angular.

The Angular ui can be run by pointing to the location of the folder in command prompt and typing in "npm start". If ofcourse angular is installed on your system. 

The server runs on http://localhost:4200/
Routes that may help: 
http://localhost:4200/admin
http://localhost:4200/
http://localhost:4200/server/api/tasks/1 (This is to query the database from angular)
