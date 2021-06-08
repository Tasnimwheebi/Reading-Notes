# AWS: API, Dynamo and Lambda
## Amazon API Gateway 
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

###  How does API Gateway work

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

### How does API Gateway work with the Serverless Framework?

The Serverless Framework uses a Lambda Proxy integration to make API Gateway events easily available to your Serverless functions.

## Benefits of Amazon API Gateway

* Map HTTP requests to specific functions in a Serverless application viaanAPI Gateway event.
* Map WebSocket events to Serverless functions.
* Use multiple microservices to serve the same top-level API.
* Save time with integrations: authentication, developer portal, CloudTrail, CloudWatch.


### Amazon API Gateway limits
* Regional APIs: you can only have 600 regional APIs per AWS account. That’s a lot; most teams won’t reach this limit.
* Integration timeouts: the shortest possible timeout for an integration in API Gateway is 50 ms, and the longest is 29 seconds.
* Payload size: the maximum payload size that can be returned by an API endpoint is 10MB. If you’re planning to return more data per request than that, you may need to split up the payload into multiple pages.


## What are serverless functions?
A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

## If you were to create a system that emulated Lambda functions, how would you do it?

Lambda functions are used when you need a function for a short period of time. This is commonly used when you want to pass a function as an argument to higher-order functions, that is, functions that take other functions as their arguments.

## Describe how a CDN works?
A CDN (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. Without a CDN, content origin servers must respond to every single end user request.

##

* **A serverless function** is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

* **Cloud storage** allows you to save data and files in an off-site location that you access either through the public internet or a dedicated private network connection. Data that you transfer off-site for storage becomes the responsibility of a third-party cloud provider.

* **Cloud CDN** (Content Delivery Network) uses Google's globally distributed edge points of presence to cache external HTTP(S) load balanced content close to your users. Caching content at the edges of Google's network provides faster delivery of content to your users while reducing serving costs.

