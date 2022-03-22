# Express

## What’s the difference between PUT and PATCH?
PATCH is used to update an already existing item in the database with new information whereas PUT will set that items information completely. It will overwrite the item if it exists otherwise it will create it. (thinking about sql create table if not exists command)

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

  [SOAP UI](https://www.soapui.org/)
  [POSTMAN](https://postman.com)
  [THUNDER CLIENT](https://www.thunderclient.com/)

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

Swaggar uses Open API

Error 403 will be thrown, however letting a possible hacker know they made a properly strctured request may be useful to them, so logging the true error for the developer and sending the status of 404 not found or something.

## Compare and contrast SOAP and ReST

- SOAP (SIMPLE OBJECT ACCESS PROTOCOL)
  - Maintained by the World Wide Web Consortium (W3C), A big difference being SOAP is a protocol while REST is not. SOAP only supports XML, SOAP is more secure.
- REST (REPRESENTATIONAL STATE TRANSFER)
  - REST is a set of guidlines that offers flexible implementations, whareas SOPA is a protocol with specific requirements like XML. REST is stateless, able to cache data, has a uniform interface, and a layered system of constraint for security.

### Helpful vocabulary

- Web Server
  - A Web serber is a computer software that accespts requests via HTTP/HTTPS. When a request is made to a web server through HTTP/S Protocol(s) there is a response from the server to the requestor with the appropriate data. a web server allows this to happen. The software of the web server must be hosted on hardware in order for it to be running all the time.

- Express
  - [DOCS](https://www.tutorialspoint.com/nodejs/nodejs_express_framework.htm) Express is a minimal and flexible Node.js web application framework that procides us a set of features to develop web applications. it facilitates rapid development of node based web applications.

- Routing
  -[DOCS](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/routes) A route is a section of Epress code that associates an HTTP verb (GET POST ECT...), which is a URL path/pattern in a function that is called to handle that pattern. see docs for how to create routes. (Router looks cool)

- WRRC
  - Web Reqeuest Response Cycle.
  