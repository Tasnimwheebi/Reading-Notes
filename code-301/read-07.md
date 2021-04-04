# SuperAgent
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

     request
       .post('/api/pet')
       .send({ name: 'Manny', species:  'cat' })
       .set('X-API-Key', 'foobar')
      .set('Accept', 'application/json')
       .then(res => {
          alert('yay got ' + JSON.stringify(res.body));
       });

## Request basics
A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request. For example a simple GET request:

    request
       .get('/search')
       .then(res => {
          // res.body, res.headers, res.status
      })
       .catch(err => {
      // err.message, err.response
      });

HTTP method may also be passed as a string:
         request('GET', '/search').then (success, failure);   

### DELETE, HEAD, PATCH, POST, and PUT requests can also be used, simply change the method name.

 **DELETE can be also called as .del() for compatibility with old IE where delete is a reserved word.**

 ### **Setting header fields:**

 * Setting header fields is simple, invoke .set() with a field name and value.
 * You may also pass an object to set several fields in a single call.

 ### **GET requests:**
The .query() method accepts objects, which when used with the GET method will form a query-string. 
* Or as a single object.
* The .query() method accepts strings as well.
* Or joined.
### HEAD requests
You can also use the .query() method for HEAD requests


### POST / PUT requests
A typical JSON POST request might look a little like the following, where we set the Content-Type header field appropriately, and "write" some data, in this case just a JSON string.

Since JSON is undoubtedly the most common, it's the default!
Or using multiple .send() calls.

SuperAgent formats are extensible, however by default "json" and "form" are supported. To send the data as application/x-www-form-urlencoded simply invoke .type() with "form", where the default is "json". This request will POST the body "name=tj&pet=tobi".

### Setting the Content-Type
As a short-hand the .type() method is also available, accepting the canonicalized MIME type name complete with type/subtype, or simply the extension name such as "xml", "json", "png", etc.

### Serializing request body
SuperAgent will automatically serialize JSON and forms. You can setup automatic serialization for other types as well.

### Retrying requests
When given the .retry() method, SuperAgent will automatically retry requests, if they fail in a way that is transient or could be due to a flaky Internet connection.

This method has two optional arguments: number of retries (default 1) and a callback. It calls callback(err, res) before each retry. The callback may return true/false to control whether the request should be retried (but the maximum number of retries is always applied).

### Setting Accept
In a similar fashion to the .type() method it is also possible to set the Accept header via the short hand method .accept(). Which references request.types as well allowing you to specify either the full canonicalized MIME type name as type/subtype, or the extension suffix form as "xml", "json", "png", etc.

### Query strings
By default the query string is not assembled in any particular order. An asciibetically-sorted query string can be enabled with req.sortQuery(). You may also provide a custom sorting comparison function with req.sortQuery(myComparisonFn). The comparison function should take 2 arguments and return a negative/zero/positive integer.
### Parsing response bodies
SuperAgent will parse known response-body data for you, currently supporting application/x-www-form-urlencoded, application/json, and multipart/form-data. You can setup automatic parsing for other response-body data as well.

### JSON / Urlencoded
The property res.body is the parsed object, for example if a request responded with the JSON string '{"user":{"name":"tobi"}}', res.body.user.name would be "tobi". Likewise the x-www-form-urlencoded value of "user[name]=tobi" would yield the same result. Only one level of nesting is supported. If you need more complex data, send JSON instead.

### Multipart
The Node client supports multipart/form-data via the Formidable module. When parsing multipart responses, the object res.files is also available to you.
### Response properties
Many helpful flags and properties are set on the Response object, ranging from the response text, parsed response body, header fields, status flags and more.

* **Response body**
Much like SuperAgent can auto-serialize request data, it can also automatically parse it. When a parser is defined for the Content-Type, it is parsed, which by default includes "application/json" and "application/x-www-form-urlencoded". The parsed object is then available via res.body.

* **Response header fields**
The res.header contains an object of parsed header fields, lowercasing field names much like node does. For example res.header['content-length'].

* **Response Content-Type**
The Content-Type response header is special-cased, providing res.type, which is void of the charset (if any). For example the Content-Type of "text/html; charset=utf8" will provide "text/html" as res.type, and the res.charset property would then contain "utf8".

* **Response status**
The response status flags help determine if the request was a success, among other useful information, making SuperAgent ideal for interacting with RESTful web services.