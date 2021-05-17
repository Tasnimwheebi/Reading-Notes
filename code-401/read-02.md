# Express/Node introduction

Node :is an open-source, cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. As such, the environment omits browser-specific JavaScript APIs and adds support for more traditional OS APIs including HTTP and file system libraries.

Express is the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks.While Express itself is fairly minimalist, developers have created compatible middleware packages to address almost any web development problem. There are libraries to work with cookies, sessions, user logins, URL parameters, POST data, security headers, and many more.
### **How popular are Node and Express?**
Based on the number of high profile companies that use Express, the number of people contributing to the codebase, and the number of people providing both free and paid for support, then yes, Express is a popular framework!

### **What does Express code look like?**
a web application waits for HTTP requests from the web browser . When a request is received the application works out what action is needed based on the URL pattern and possibly associated information contained in POST data or GET data. Depending on what is required it may then read or write information from a database or perform other tasks required to satisfy the request. The application will then return a response to the web browser, often dynamically creating an HTML page for the browser to display by inserting the retrieved data into placeholders in an HTML template.Express provides methods to specify what function is called for a particular HTTP verb (GET, POST, SET, etc.) and URL pattern ("Route"), and methods to specify what template ("view") engine is used, where template files are located, and what template to use to render a response.

### Importing and creating modules
A module is a JavaScript library/file that you can import into other code using Node's require() function. Express itself is a module, as are the middleware and database libraries that we use in our Express applications.

## npm
npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

npm consists of three distinct components:
* Use the website to discover packages, set up profiles, and manage other aspects of your npm experience.
* The CLI runs from a terminal, and is how most developers interact with npm.
* The registry is a large public database of JavaScript software and the meta-information surrounding it.

## TDD
TDD : “Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing and design.
### Skill Levels
* Beginner 
    * able to write a unit test prior to writing the corresponding code
    * able to write code sufficient to make a failing test pass
* Intermediate
    * practices “test driven bug fixing”: when a defect is found, writes a test exposing the defect before correction
    * able to decompose a compound program feature into a sequence of several unit tests to be written
    * knows and can name a number of tactics to guide the writing of tests
    * able to factor out reusable elements from existing unit tests, yielding situation-specific testing tools
* Advanced
    * able to formulate a “roadmap” of planned unit tests for a macroscopic features
    * able to “test drive” a variety of design paradigms: object-oriented, functional, event-drive
    * able to “test drive” a variety of technical domains: computation, user interfaces, persistent data access

## What’s the difference between PUT and PATCH? 
The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.
## 
1 – Nock

2 – MockServer

3 – Mockoon

## Compare and contrast SOAP and ReST
As opposed to SOAP, REST is not a protocol but an architectural style. ... It allows different messaging formats, such as HTML, JSON, XML, and plain text, while SOAP only allows XML. REST is also a more lightweight architecture, so RESTful web services have a better performance.

