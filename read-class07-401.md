# Bearer Authorization

## Review, Research, and Discussion
+ Write the following steps in the correct order:
1. .Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Make a request to a third-party API endpoint
4. Redirect to a third party authentication endpoint
5. Make a request to the access token endpoint
6. Receive access token
7. Receive authorization code
+ What can you do with an authorization code?
### The only thing you can do with the authorization code is to make a request to get an access token.the authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.
+ What can you do with an access token?
### Access tokens are used to make API requests on behalf of a user
+ What’s a benefit of using OAuth instead of your own basic authentication?
### It enables apps to obtain limited access (scopes) to a user’s data without giving away a user’s password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities.

[Github view](https://github.com/sbkhaloof/growthmindsit)
