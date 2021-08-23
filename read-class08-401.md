#  Access Control (ACL)
## Review, Research, and Discussion
+ When is Basic Authorization used vs. Bearer Authorization?
#### basic authorization used when in sign-in process, after signing-up,but bearer authorization used after basic auth done(for authrizaton issue).

+ What does the JSON Web Token package do?
#### generates a token that we can use with authorization and information exchange
+ What considerations should we make when creating and storing a SECRET?
* Never store unencrypted secrets in .git repositories.
* Don’t share your secrets unencrypted in messaging systems like slack.
* Use encryption to store secrets within .git repositories like environment variables.
* Restrict API access and permissions.
## Document the following Vocabulary Terms
- encryption :  is the process of taking plain text, like a text message or email, and scrambling it into an unreadable format — called “cipher text.
- token: it an encoded json, that we use in beare authorization to ensure if the user is authorized or not.
- bearer: is an HTTP authentication scheme that involves security , Bearer authentication is a security scheme with type: http and scheme: bearer 
- secret: it is a signiture for the developper that make his token secure and no one can access his data when his secret is exists.
- JSON Web Token: is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key .


[Github view](https://github.com/sbkhaloof/growthmindsit)