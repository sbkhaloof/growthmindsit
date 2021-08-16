# Express REST API
1. Name 3 real world use cases where you’d want to change the request with custom middleware
+ handling error.
+ change in request object or response object
+ to do something into request object.
2. True or false: The route handler is middleware? false 
3. In what ways can a middleware function end the process and send data to the browser?
+ if it at the final middleware function
+ if it face an issue and pass the error in next .
4. At what point in the request lifecycle can you “inject” middleware?
### Middleware is a function which is called when send request before the route handler.
5. What can cause express to error with “Request headers sent twice, cannot start a second response”
### when you send more than one request to the server and make interupt between this requests, so kindlly he dell with this requests by send a response have an error.


[Github view](https://github.com/sbkhaloof/growthmindsit)