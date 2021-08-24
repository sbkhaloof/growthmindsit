# Authorization/Authentication
## Review, Research, and Discussion
+ What header(s) are used in authentication and authorization
#### basic encode(username:password)
#### Bearer Token
+ What is safe to put into a JWT
#### It’s safe to put very strong SECRET-Key ,So nobody can change user info from JWT used => And put encoding password , So nobody can know it from JWT used By this way we can get more Safe and Secure
+ How are JWTs validated
#### if the signature is correct, then the user is correctly authenticated and the request goes through. => if not, the application server can simply reject the request.
## Document the following Vocabulary Terms
* RBAC: (role base access control) is a method of restricting network access based on the roles of individual users within an enterprise.
* User Roles :permissions for users to perform a group of tasks. In a default WordPress installation there are some predefined roles with a predefined set of permissions. These roles are Super Admin, Administrator, Editor, Author, Contributor, and Subscriber
* JWT Token:open standard define a way for securely transmitting information between parties as json object 





[Github view](https://github.com/sbkhaloof/growthmindsit)