#  Authentication
## Review, Research, and Discussion
+ Explain what a “Singleton” is (in Computer Science terms)
#### A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.
+ Explain how the Singleton pattern can be used with Node modules, specifically with classes
1. The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times.
2. The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times.
3. A singleton is intended to provide only one instance of itself while facilitating a global point of access. Implementing a singleton pattern involves creating a class with a method that creates a new instance of the class. In order to implement a singleton pattern, principles of single instance and global access must be satisfied.
4. The singleton class is like a global repository for an instance of itself, making the constructor private. Therefore, an instance outside the class cannot be created at all, and a singleton can contain only one instance. A singleton class instantiates itself and maintains that instance across systems
+ If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
#### npm init 
#### npm install express –save 
#### Create server.js and paste the following code:

#### const express = require(‘express’); const app = express();

#### app.get(‘/’, (req, res, next) => { res.send(‘Welcome Home’); });

#### app.listen(3000);


[Github view](https://github.com/sbkhaloof/growthmindsit)
