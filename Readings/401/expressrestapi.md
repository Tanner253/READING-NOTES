# Reading for express REST API

## what are ES6 classes?

classes allow us to template creating objects. They encapsulate data with code to work on that data. (think about the Array class and all of the methods and properties that come with Array's once we instantiate them.) Classes must be defined before they can be constructed. We use a constructor to define how objects will be created when the class is instantiated into an object. we can use OOP pricipal inheritance to use the keywrod extends to pass along like functionality to a child class. NOT COMPATABLE with internet explorer (weird).

## How do we use express routing?

Routing refers to how an applications enpoints or URI;s respond to a clients requests. When someone types in a route in their url (anything that comes after the .com) we  have access to different information and abilities depending on what that route does. Theres 2 parts to the route, the clientside, how is the route being requested, and server side, how are the routes setup and what do they do once they are requested. we use route methods to define what http action will be used when the endpoint is hit. We use route paths to define what the client must enter or request in order to hit those http actions for example a get request to /dog can only be triggered when the request from the front end makes a request with the url.com/dog 

## using express routing

In order to use express routing, we need to use express as a dependancy in our application with npm i
[Digital ocean docs](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4) this page is extremely useful for getting a quick down and dirty implementation of express with appropriate middlewares setup for user request and server response.
