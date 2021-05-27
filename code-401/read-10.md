# OAuth 2 Simplified
## Roles 
### **The Third-Party Application: "Client"**

The client is the application that is attempting to get access to the user's account. It needs to get permission from the user before it can do so.

### **The API: "Resource Server"**
The resource server is the API server used to access the user's information.

### **The Authorization Server**
This is the server that presents the interface where the user approves or denies the request. In smaller implementations, this may be the same server as the API server, but larger scale deployments will often build this as a separate component.

### **The User: "Resource Owner"**
The resource owner is the person who is giving access to some portion of their account.

## Creating an App
Before you can begin the OAuth process, you must first register a new app with the service. When registering a new app, you usually register basic information such as application name, website, a logo, etc. In addition, you must register a redirect URI to be used for redirecting users to for web server, browser-based, or mobile apps.

### **Redirect URIs**
The service will only redirect users to a registered URI, which helps prevent some attacks. Any HTTP redirect URIs must be served via HTTPS.

### **Client ID and Secret**
The client secret must be kept confidential. If a deployed app cannot keep the secret confidential, such as single-page Javascript apps or native apps, then the secret is not used, and ideally the service shouldn't issue a secret to these types of apps in the first place.

# Authorization
The first step of OAuth 2 is to get authorization from the user. For browser-based or mobile apps, this is usually accomplished by displaying an interface provided by the service to the us.

## Web Server Apps
Web server apps are the most common type of application you encounter when dealing with OAuth servers.

## Single-Page Apps
Single-page apps (or browser-based apps) run entirely in the browser after loading the source code from a web page. Since the entire source code is available to the browser, they cannot maintain the confidentiality of a client secret, so the secret is not used in this case.

## Mobile Apps
Like browser-based apps, mobile apps also cannot maintain the confidentiality of a client secret. Because of this, mobile apps also use the PKCE flow which does not require a client secret.


