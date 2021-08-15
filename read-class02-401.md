# Express
## Review, Research, and Discussion
+ What’s the difference between PUT and PATCH?
#### in put method when i want to update any part of data i need to send all parameters of the data again but patch method say that we will send just the part which is updated .
+ Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
[MockServer](https://www.mock-server.com/)
[Postman Mock Server](https://www.postman.com/)
[ Beeceptor](https://beeceptor.com/)
+ Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
#### Popularity: By comparing stats,  swagger-ui is more popular then apidocjs.
Consistency: If we already using swagger for our Dotnetcore service, then implementing swagger tool will consist more from Info and UI prospective.
Implementation complexity: apidocjs and swagger both required documentation content on implemented method as customize comment data. In addition they allow to write documentation data in separate resource file as .js and .json. If we already have swagger.json created by DotnetCore we can reuse more than 80% specification.
 Maintenance: For apidocjs will have to modify documentation for each affected method/endpoints if service changed. In swagger we can limit changes. But by implementing apidocjs we can isolate the layer.
Other benefits: Because swagger use plain .json that could be parsed through programing language, thus we can get advantage of various other 3rd parties in order to create http client and more. 
Future: Due to popularity of swagger, apidocjs provide information about apidoc-swagger converter so we can switch apidoc to swagger anytime.

+ Compare and contrast SOAP and ReST
1. SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State Transfer.
2. SOAP is a protocol whereas REST is an architectural pattern.
3. SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.
4. SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.
5. Comparing SOAP vs REST API, SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.
6. SOAP cannot make use of REST whereas REST can make use of SOAP.

[Github view](https://github.com/sbkhaloof/growthmindsit)
