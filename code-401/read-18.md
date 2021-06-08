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



