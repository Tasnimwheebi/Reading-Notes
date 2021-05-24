# Bearer Authorization

## What is JSON Web Token?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 

### Here are some scenarios where JSON Web Tokens are useful:

* Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

* Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties.

### What is the JSON Web Token structure?
 JSON Web Tokens consist of three parts separated by dots (.):
 * **Header** : consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
* **Payload** : which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
* **Signature** : To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

    Example :

        HMACSHA256(
        base64UrlEncode(header) + "." +
        base64UrlEncode(payload),
         secret)


The signature is used to verify the message wasn't changed along the way, and, in the case of tokens signed with a private key, it can also verify that the sender of the JWT is who it says it is.

## **Term** 
* **A Client ID** is an identifier associated with an application that assists with client / server OAuth 2.0 authentication for ArcGIS client APIs . Developers create a client ID by defining an application on their developer dashboard.

* **A client secret** is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps.

* **Endpoint authentication** is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.

* **The token endpoint** is where apps make a request to get an access token for a user. This section describes how to verify token requests and how to return the appropriate response and errors. Authorization Code. Password Grant. Client Credentials.

* **API endpoint** is the point of entry in a communication channel when two systems are interacting. It refers to touchpoints of the communication between an API and a server. ... An API endpoint is basically a fancy word for a URL of a server or service.

* **The authorization code** is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request

* **An access token** is an object encapsulating the security identity of a process or thread. A token is used to make security decisions and to store tamper-proof information about some system entity.

## **Questions**

### **Write the following steps in the correct order:**
1. Register your application to get a client_id and client_secret.
2. Ask the client if they want to sign in via a third party.
3. Redirect to a third party authentication endpoint.
4. Make a request to the third-party API endpoint.
5. Receive authorization code.
6. Make a request to the access token endpoint.
7. Receive access tokent.

### **What can you do with an authorization code?**

The user sees the authorization prompt and approves the app's request. The user is redirected back to the application with an authorization code in the query string. The application exchanges the authorization code for an access token.

### **What can you do with an access token?**

A security token is a peripheral device used to gain access to an electronically restricted resource. The token is used in addition to or in place of a password. It acts like an electronic key to access something.

### **What’s a benefit of using OAuth instead of your own basic authentication?**

While the OAuth 2 “password” grant type is a more complex interaction than Basic authentication, the implementation of access tokens is worth it. Managing an API program without access tokens can provide you with less control, and there is zero chance of implementing an access token strategy with Basic authentication.