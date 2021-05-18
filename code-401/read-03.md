# Express REST API
## **Classes**
Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.
Classes are in fact "special functions", and just as you can define function expressions and function declarations.
## Hoisting
An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not.

## Sub classing with extends
The extends keyword is used in class declarations or class expressions to create a class as a child of another class.
If there is a constructor present in the subclass, it needs to first call super() before using "this".Note that classes cannot extend regular (non-constructible) objects. If you want to inherit from a regular object, you can instead use Object.setPrototypeOf().
## Super class calls with super
The super keyword is used to call corresponding methods of super class. This is one advantage over prototype-based inheritance.
# Routing
Routing refers to how an application’s endpoints (URIs) respond to client requests.Defining routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests.
## Route methods
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.
## Route paths
Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions
## Route parameters
Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.
## Route handlers
You can provide multiple callback functions that behave like middleware to handle a request. The only exception is that these callbacks might invoke next('route') to bypass the remaining route callbacks.
## Route Middleware router.use()
Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.
## Conclusion
* Use express.Router() multiple times to define groups of routes.
* Apply the express.Router() to a section of our site using app.use().
* Use route middleware to process requests.
* Use route middleware to validate .parameters using .param().
* Use app.route() as a shortcut to the Router to define multiple requests on a route.

# Questions:
## Name 3 real world use cases where you’d want to change the request with custom middleware
*  Logging Middleware
*  Authentcation
*  Data Management 
## True or false: The route handler is middleware? false.
## In what ways can a middleware function end the process and send data to the browser?
 By calling res.end, res.send, res.render or any method that implicitely calls res.end
 ## At what point in the request lifecycle can you “inject” middleware?
 it is executed in between in the middle of receiving a request and sending back a response.
