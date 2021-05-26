# Access Control (ACL) 
## What is RBAC?
RBAC is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

## Benefits of RBAC?

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

RBAC may sound intimidating, but it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.

## RBAC vs. ABAC vs. ACL
* **Access control lists (ACL)** — An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.

* **Attribute-based access control (ABAC)** — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.

## RBAC implementation 

**Five-step approach to getting RBAC implemented :**
1. Inventory your systems
2. Analyze your workforce and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

## **Term**

* **Encryption** is the method by which information is converted into secret code that hides the information's true meaning. The science of encrypting and decrypting information is called cryptography. In computing, unencrypted data is also known as plaintext, and encrypted data is called ciphertext.
* **A JSON Web Token**  is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.
* **Bearer Tokens** are the predominant type of access token used with OAuth 2.0. A Bearer Token is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens.
## **Questions**


### **When is Basic Authorization used vs. Bearer Authorization?**
The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617). The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750.

### **What does the JSON Web Token package do?**

A JSON Web Token is used to send information that can be verified and trusted by means of a digital signature. It comprises a compact and URL-safe JSON object, which is cryptographically signed to verify its authenticity, and which can also be encrypted if the payload contains sensitive information.

## **What considerations should we make when creating and storing a SECRET?**
Store secrets safely:
1. Use encryption to store secrets within .git repositories.
2. Use environment variables.
3. Use "Secrets as a service" solutions.