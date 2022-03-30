# JWT

## JWT's explained

Json web token
Open standard (anyone can use it)
used to securely transfer information between 2 parties. digitally signed, verified and trusted data. JWT is very compact, so we can send via URL.
avoids querying database more than once. contains information about user. payload contains the user object and whatever information needed. the signature is added via base 54 or 126 encoding.

## JWT DOCS

[DOCS](https://jwt.io/introduction/)

JWT tokens can be encrypted, however signed tokens is more normal.

use JWT when needing to authorize an user, or exchange information between 2 parties. There are 3 parts of a JWT the header the payload and the signature.

## Are JWT tokens safe?

[article in question](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

JWT's can be signed or encrypted or both. The secret is the key used to unlock the JWT tokens functionality. without the secret being accurate theres no way to guess the JWT token or reqeust information.