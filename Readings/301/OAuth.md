# What is OAuth?

>Ooen standard authorization rpotocol or framwork the described how unrelated servers and services can safley alllow authenticated access to their assets without actually sharing the initial related single logon credential.

- Give an example of what using OAuth would look like.

>

- How does OAuth work? What are the steps that it takes to authenticate the user?

>signing in with 3rd party sources

- What is OpenID?

>Oauth is authorization, ID is authentication

- What is the difference between authorization and authentication?

>authorization says what youre allowed to do and authentication says whos allowed to do it based on who you are (id)

- What is Authorization Code Flow?

>server apps do not publicly expose data so they can use the authorization code flow which exchanges an authorization code for an access token

- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

>addds another layer of security on top of authorization code flow due to single page app challenges

- What is Implicit Flow with Form Post?

>intended for apps that cannot store secrets

- What is Client Credentials Flow?

>authorizes the application rather than the user. (not user and pass logins)

- What is Device Authorization Flow?

>when you click a link on your phone to authenticate somewhere.

- What is Resource Owner Password Flow?

>directly asking user for login information, usually not reccomended anymore.