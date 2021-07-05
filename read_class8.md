# APIs
## API Design Best Practices
1- What does REST stand for?
##### Representational state transfer
2- REST APIs are designed around a _resources___.
#####
3- What is an identifer of a resource? Give an example.
##### A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: https://adventure-works.com/orders/1
4- What are the most common HTTP verbs?
##### The most common operations are GET, POST, PUT, PATCH, and DELETE.
5- What should the URIs be based on?
##### When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
6- Give an example of a good URI.
##### https://adventure-works.com/orders // Good
7- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
##### web APIs that expose a large number of small resources. no it's bad thing .
8- What status code does a successful GET request return?
##### A successful GET method typically returns HTTP status code 200 (OK).
9- What status code does an unsuccessful GET request return?
##### If the resource cannot be found, the method should return 404 (Not Found).
10- What status code does a successful POST request return?
#####  it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
11- What status code does a successful DELETE request return?
##### f the delete operation is successful, the web server should respond with HTTP status code 204.
