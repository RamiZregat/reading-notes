# Mongo and Mongoose

## nosql vs sql

The Difference|SQL|NoSQL
--------------|---|--------
Data base name|SQL databases are primarily called as Relational Databases (RDBMS).|NoSQL database are primarily called as non-relational or distributed database.
Data base based on|SQL databases are table based databases.|NoSQL databases are document based.
Data base schema|SQL databases have predefined schema.|NoSQL databases have dynamic schema for unstructured data.
Data base scaleable|SQL databases are vertically scalable.|NoSQL databases are horizontally scalable.


**- What kind of data is a good fit for an SQL database?**

For complex queries: SQL databases are good fit for the complex query intensive environment.

**-Give a real world example.**

NoSQL databases do a better job at representing real world objects.
It’s all fresh in my mind, I had my exam on Advanced DataBases just yesterday and thus was one of the questions!!


**-What kind of data is a good fit a NoSQL database?**

NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.


**- Give a real world example.**

Lets say you want to build the next Google Analytics. You figure out you want to track IP Address, Browser & Device type. Later you, however, finds out you might want to track Browser Size as well. Since analytics databases can contain millions/billions of data, it isn't so easy to add an extra column to your table. It would simply take too long.

With a NOSQL solution you might just add it to the future rows, without having to change every row in the tracking table

**- Which type of database is best for hierarchical data storage?**

NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.


**- Which type of database is best for scalability?**


it depends on which scale we are talking about SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
________________________________________________

## More info about sql vs nosql:

**-What does SQL stand for?**

stands for Structured Query Language.

**-What is a realational database?**

A relational database is a type of database that stores and provides access to data points that are related to one another.


**-What type of structure does a relational database work with?**

its SQL, SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.


**-What is a ‘schema’?**

A schema is a collection of logical structures of data, or schema objects. A schema is owned by a database user and has the same name as that user. Each user owns a single schema. Schema objects can be created and manipulated with SQL.


**-What is a NoSQL database?**

NoSQL databases (aka "not only SQL") are non tabular, and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads.


**-How does NoSQL  work?**

The major purpose of using a NoSQL database is for distributed data stores with humongous data storage needs. NoSQL is used for Big data and real-time web apps. For example, companies like Twitter, Facebook and Google collect terabytes of user data every single day.


**- What is inside of a Mongo database?**

MongoDB makes use of records which are made up of documents that contain a data structure composed of field and value pairs. Documents are the basic unit of data in MongoDB. The documents are similar to JavaScript Object Notation, but use a variant called Binary JSON (BSON).


**-Which is more flexible - SQL or MongoDB? and why.**

In MongoDB, all individual records are stored as documents which are collections of fields with a dynamic schema. Here, each collection need not have the same set of fields which makes it more flexible


**-What is the disadvantage of a NoSQL database?**

* NoSQL databases don’t have the reliability functions which Relational Databases have (basically don’t support ACID).  
This also means that NoSQL databases offer consistency in performance and scalability.


* In order to support ACID developers will have to implement their own code, making their systems more complex.
  
  This may reduce the number of safe applications that commit transactions, for example bank systems.

* NoSQL is not compatible (at all) with SQL.  

  Note: Some NoSQL management systems do use a Structured Query Language.  
This means that you will need a manual query language, making things slower and more complex.

* NoSQL are very new compared to Relational Databases, which means that are far less stable and may have a lot less functionalities.
  

