# Using the API

### Authorizing requests and identifying your application
Every request your application sends to the Books API needs to identify your application to Google. There are two ways to identify your application: using an OAuth 2.0 token (which also authorizes the request) and/or using the application's API key. Here's how to determine which of those options to use:

* If the request requires authorization (such as a request for an individual's private data), then the application must provide an OAuth 2.0 token with the request. The application may also provide the API key, but it doesn't have to.
* If the request doesn't require authorization (such as a request for public data), then the application must provide either the API key or an OAuth 2.0 token, or both—whatever option is most convenient for you.

## Acquiring and using an API key
API keys: A request that does not provide an OAuth 2.0 token must send an API key. The key identifies your project and provides API access, quota, and reports.

The API supports several types of restrictions on API keys. If the API key that you need doesn't already exist, then create an API key in the Console by clicking Create credentials > API key. You can restrict the key before using it in production by clicking Restrict key and selecting one of the Restrictions.

### Google Books IDs
You need to specify ID fields with certain API method calls. There are three types of IDs used within Google Books:

* Volume IDs
* Bookshelf IDs
* Bookshelf IDs

### Optional query parameters
you can use the following query parameters when performing a volumes search:
* Download Format : 
You use the download parameter to restrict the returned results to volumes that have an available download format of epub
* Filtering : You can use the filter parameter to restrict the returned results further by setting it the to one of the following values: partial, full , free-ebooks , paid-ebooks , ebooks.
* Pagination : You can paginate the volumes list by specifying two values in the parameters for the request: startIndex, maxResults.
* Print Type : You can use the printType parameter to restrict the returned results to a specific print or publication type. 
* Projection : You can use the projection parameter with one of the following values to specify a predefined set of Volume fields to return: full , lite.
* Sorting : You can change the ordering by setting the orderBy parameter to be one of these values: relevance , newest.


# What is EJS?
  EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

### Features
* Fast compilation and rendering
* Simple template tags: <% %>
* Custom delimiters (e.g., use [? ?] instead of <% %>)
* Sub-template includes
* Ships with CLI
* Both server JS and browser support
* Static caching of intermediate JavaScript
* Static caching of templates
* Complies with the Express view system


