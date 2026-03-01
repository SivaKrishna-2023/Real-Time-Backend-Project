


src ->Inside the src folder all the actual source code regarding the project will reside,this wll not include any kind test.(You might want to make seprate test folder)

Lets take a Look inside the src folder.
config ->In this folder anything and everything regarding any configration or setup of library or module will be done.For example:setting up dotenv so that we can use the enviroment variables anywhere in cleaner fashion,this is done in the server-config.js file.One more example can be setup your logging libarary that can help you to prepare meaningful logs,so configuration for this library should also be done here.

routes ->Inside the routes folder,we register a route and corresponding middleware and controllers to it.

middlewares ->They are just going to intercept the incomming request where we can write our validators,authenticators etc.

controllers->They are kind of the last middleware as post them you call your bussiness layer to execute bussiness logic.In controllers we just recive the incomming request and data and pass it to bussiness laye and once bussiness layer returns the an output, we structure the API response in controllers and send the output.

repositories-This folder all the logic using which we intract the DB by writing the queries, all the all raw queries orm queries will go here.

services ->Contain all the business logic and interact with the repo for the data from the database.

utils ->Utils contain helper methos,error classes.