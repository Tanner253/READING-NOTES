- In your own words, describe what each group of status code represents:

- 100’s = Informational Codes
- 200’s = Success Codes
- 300’s = redirect codes
- 400’s = client errors (I did something wrong)
- 500’s = server errors (you did something wrong)
- What is a status code 202? accepted response
- What is a status code 308? permanant redirect
- What code would you use if an update didn’t return data to a client? 204
- What code would you use if a resource used to exist but no longer does? 410
- What is the ‘Forbidden’ status code?

 >The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

- Why do we need to pull our MongoDB database string out of our server and put it into our .env?

 > To protect against data breaches

- What is middleware?

>code that runs before the final route back

- What does app.use(express.json()) 

>do? middleware that parses json for use

- What does the /:id mean in a route?

>app.get('/users/:userId/books/:bookId' Specifies the IF od user and the ID of book when responding

- What is the difference between PUT and PATCH?

>Patch is used to update existing entitiy with new info, PUT will set an entetis imformation completley. Putting is close to post

- How do you make a default value in a schema?

> if you dont specify values for object default values will kick in. noted that this only occurs if the value is strictly undefined.

- What does a 500 error status code mean?

> Internal server error

- What is the difference between a status 200 and a status 201?

>201 indidcates the request has been successful and the resouce has been created while a 200 is simply a success code that indicates processing.