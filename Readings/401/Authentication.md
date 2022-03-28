# Authentication

## Securing passwords with Bycrypt

 - Brute force attack - hacker doesnt try to reverse hash, just tries to hash random inputs until cracked.
 
 - hash collision attack - 2 different inputs that create the same hash out put (big datasets vulnerability);

 - BCrypt - SLOW AND STRONG AS HELL, An adaptive hashing that is based on blowfish symetric block sypher cytography -> allows you to determine how expensive a hash function will be.

 ## Basic Auth

 - auth is handled in the HTTP methods through user agent. The url provides an user name and password to the request to verify the user making the request is allowed to recieve the data.

 ## OWASP

 [https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html](helpful documentation for authentication);

Cheat sheet for everything you need Authentication and Authorization.

## BCrypt docs

see site for async inplementations and with promises

```js
//setup auth variables
const bcrypt = require('bcrypt');
const saltRounds = 10;
const myPlaintextPassword = 's0/\/\P4$$w0rD';
const someOtherPlaintextPassword = 'not_bacon';

//hash a password
bcrypt.genSalt(saltRounds, function(err, salt) {
    bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {
        // Store hash in your password DB.
    });
});

// Load hash from your password DB.
bcrypt.compare(myPlaintextPassword, hash, function(err, result) {
    // result == true
});
bcrypt.compare(someOtherPlaintextPassword, hash, function(err, result) {
    // result == false
});
```

async is reccomended because hashing passwords is an extremely heavy operation

BCrypt is NOT susceptible to timing attacks.
