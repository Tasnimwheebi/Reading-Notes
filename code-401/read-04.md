# Data Modeling
## SQL vs NoSQL Database 
* SQL databases are primarily called as Relational Databases,NoSQL database are primarily called as non-relational .
* SQL databases are table based databases,NoSQL databases are document based, key-value pairs, graph databases or wide-column stores.
* SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
* SQL databases are vertically scalable,NoSQL databases are horizontally scalable.
* SQL databases uses SQL ( structured query language ) for defining and manipulating the data. In NoSQL database, queries are focused on collection of documents. 
* SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL.NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb.
* SQL databases are good fit for the complex query intensive environment, NoSQL databases are not good fit for complex queries.
* SQL databases are not best fit for hierarchical data storage.NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.
* SQL databases are vertically scalable. NoSQL databases are horizontally scalable.
*  SQL databases are best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data,you can use NoSQL for transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications.
*  Excellent support are available for all SQL database from their vendors. For some NoSQL database you still have to rely on community support, and only limited outside experts are available for you to setup and deploy your large scale NoSQL deployments.
* SQL databases emphasizes on ACID properties, NoSQL database follows the Brewers CAP theorem.
*  SQL databases as either open-source or close-sourced from commercial vendors.  NoSQL databases can be classified on the basis of way of storing data as graph databases, key-value store databases, document store databases, column store database and XML databases.

## SQL Database Examples
* MySQL Community Edition
* MS-SQL Server Express Edition
* Oracle Express Edition
## NoSQL Database Examples
* MongoDB
*  CouchDB
* Redis

# Question

## Name 3 advantages to Test Driven Development
* Better program design and higher code quality.
* Detailed project documentation .
* TDD reduces the time required for .project development.
* Code flexibility and easier maintenance.
* With TDD you will get a reliable solution.
* Save project costs in the long run.

## In what case would you need to use `beforeEach()` or  `afterEach()` in a test suite?

If you have some work you need to do repeatedly for many tests, you can use beforeEach and afterEach.

## What is one downside of Test Driven Development?

Probably, the strongest argument against TDD is that the tests need to be maintained because the code has got to. Whenever requirements change, you would like to vary the code and tests. ... So, actually, this disadvantage is that the same as before when writing code that apparently takes an extended time.

## What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?


The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance. A constructor in JavaScript is just a plain old function that returns an object.

## Why REST?

REST aims to make caching easier. Since the server is stateless and each request can be processed individually, GET requests should usually return the same response regardless of previous ones and the session. This makes the GET requests easily cacheable and browsers usually treat them as such.