# Authentication
## Hashing
Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.


The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.

## Basic access authentication
Basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

 **The Authorization header field is constructed as follows :**
 
* The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
* The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.
* The resulting string is encoded using a variant of Base64 (+/ and with padding).
* The authorization method and a space (e.g. "Basic") is then prepended to the encoded string.

**Authentication** : is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

### Implement Proper Password Strength Controls
* Password Length 
    * Minimum length of the passwords should be enforced by the application.Passwords shorter than 8 characters are considered to be weak
    * Maximum password length should not be set too low, as it will prevent users from creating passphrases.

* Do not silently truncate passwords.
* Allow usage of all characters including unicode and whitespace.
* Ensure credential rotation when a password leak, or at the time of compromise identification.
* Include password strength meter to help users create a more complex password and block common and previously breached passwords.

## node.bcrypt.js
A library to help you hash passwords.

# Term

* Router Middleware  : 
Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

* Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.
* The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton. Singletons are useful in situations where system-wide actions need to be coordinated from a single central place. An example is a database connection pool.
* Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones.
##  Questions :
1. **Explain what a “Singleton” is (in Computer Science terms)?**

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. 


2. **Explain how the Singleton pattern can be used with Node modules, specifically with classes?**


To create the singleton class, we need to have static member of class, private constructor and static factory method.
Static member: It gets memory only once because of static, itcontains the instance of the Singleton class.
Private constructor: It will prevent to instantiate the Singleton class from outside the class.

3. **If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**
*  First, you will need Node and NPM. To ensure you have them installed.
* To get started, you’ll use the most basic of Express’ built-in middleware.
* Create server.js
* Run the server via node server.js
* In Express, you can set up middleware to be “global” middleware; meaning it will be called for every incoming request.

`const express = require('express');
const app = express();`
* The middleware logs out the request object and then calls next(). The next middleware in the pipeline handles the get request to the root URL and sends back the text response. Using app.use() means that this middleware will be called for every call to the application.

* Example :

`const express = require('express');
const app = express();`

`app.use((req, res, next) => {
  console.log(req);
  next();
});`

`app.get('/', (req, res, next) => {
  res.send('Welcome Home');
});`

`app.listen(3000);`

