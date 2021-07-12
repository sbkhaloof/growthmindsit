# CRUD
## Status Codes Based On REST Methods
1. In your own words, describe what each group of status code represents:
* 100’s =These are informational status codes .
* 200’s =These are the success codes.
* 300’s =These are redirection codes.
* 400’s =These are the client error codes.
* 500’s =These are the server error codes. 
2. What is a status code 202?
#### Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.
3. What is a status code 308?
#### Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.
4. What code would you use if an update didn’t return data to a client?
#### 204 No Content 
5. What code would you use if a resource used to exist but no longer does?
#### 410
6. What is the ‘Forbidden’ status code?
#### 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
#### You can use the mongo shell to query and update data as well as perform administrative … Once you have verified that the mongod server is running, open a terminal … Adding your to the PATH environment variable … You can specify the replica set name and members in the connection string.
2. What is middleware?
#### is software that provides common services and capabilities to applications outside of what’s offered by the operating system.
3. What does app.use(express.json()) do?
#### express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app. … urlencoded() is a method inbuilt in express to recognize the incoming Request Object as strings or arrays
4. What does the /:id mean in a route?
#### Gives access to whatever the client provides after the slash.
5. What is the difference beween PUT and PATCH?
#### The main difference between PUT and PATCH requests is witnessed in the way the server processes the enclosed entity to update the resource identified by the Request-URI. When making a PUT request, the enclosed entity is viewed as the modified version of the resource saved on the original server, and the client is requesting to replace it. However, with PATCH, the enclosed entity boasts a set of instructions that describe how a resource stored on the original server should be partially modified to create a new version.The second difference is when it comes to idempotency. HTTP PUT is said to be idempotent since it always yields the same results every after making several requests. On the other hand, HTTP PATCH is basically said to be non-idempotent. However, it can be made to be idempotent based on where it is implemented.
6. How do you make a defalut value in a schema?
#### You pass in default into the keys.
7. What does a 500 error status code mean?
#### Internal Server Error
8. What is the difference between a status 200 and a status 201?
#### The 200 (ok) status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed.but 201 - Created A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).


