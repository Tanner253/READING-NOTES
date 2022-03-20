# API reading

- What does REST stand for?

>REpresentational State Transfer

- REST APIs are designed around a ____.

>data set / request response cycle

- What is an identifer of a resource? Give an example.

>REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

- What are the most common HTTP verbs?

>The most common operations are GET, POST, PUT, PATCH, and DELETE.

- What should the URIs be based on?

>the data being requested/responded

- Give an example of a good URI.

><https://adventure-works.com/orders/1>

- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

>we want to send whole data packages instead of having the user make a bunch of requests. the less amount of requests the better.

- What status code does a successful GET request return?
A successful GET method typically returns HTTP status code 200 (OK). If the resource cannot be found, the method should return 404 (Not Found).

- What status code does a successful POST request return?
201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
- What status code does a successful DELETE request return?
If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled