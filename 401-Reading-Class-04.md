# Data Modeling  

### Name 3 advantages to Test Driven Development: (Links to an external site.)
1. faster development time.
1. lowering project cost.
1. code flexibility and ease of maintenance.
### In what case would you need to use beforeEach() or afterEach() in a test suite?
When some work is needed to be done repeatedly for many tests, it can use `beforeEach` and `afterEach`.  
### What is one downside of Test Driven Development ?
- Tests help to seek out bugs, but they can not find bugs that you simply introduce within the test code and in implementation code.  
- The tests need to be maintained because the code has got to. If the requirements changed, then the test need to be changed   

### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?  
The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.  
### Why REST?  
One of the key advantages of REST APIs is that they provide a great deal of flexibility. Data is not tied to resources or methods, so REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia. This flexibility allows developers to build an API that meets your needs while also meeting the needs of very diverse customers.

## Vocabulary Terms  
Term | Definition
--- | ---
functional programming | programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values.
Object-oriented programming | a programming paradigm that relies on the concept of classes and objects. It is used to structure a software program into simple, reusable pieces of code blueprints (usually called classes), which are used to create individual instances of objects
class | a blueprint for creating objects. They encapsulate data with code to work on that data.
super | keyword is used to access and call functions on an object’s parent.
this | keyword refers to the object it belongs to its scope.
TDD | a style of programming in three activities: coding, testing (in the form of writing unit tests) and design (in the form of refactoring)
Jest | a delightful JavaScript Testing Framework with a focus on simplicity.
CI | it stand for **Continuous Integration** ,which is the practice of merging all developers’ working copies to a shared mainline several times a day.  
REST | software architectural style that was created to guide the design and development of the architecture for the World Wide Web.
Data Model | defined as an abstract model that organizes data description, data semantics, and consistency constraints of data. The data model emphasizes on what data is needed and how it should be organized instead of what operations will be performed on data.  

## Preview  
1. Which 3 things had you heard about previously and now have better clarity on?  
    -  `beforeEach()` and `afterEach()`
    -  `REST`
    -  Object Oriented Programming
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?  
    - more about testing
    - CI
    - SQL
1. What are you most excited about trying to implement or see how it works?  


## Preparation Materials

**sql vs nosql:**  

- Flexible data models:  
NoSQL databases typically have very flexible schemas. A flexible schema allows you to easily make changes to your database as requirements change. You can iterate quickly and continuously integrate new application features to provide value to your users faster.

- Fast queries:   
Queries in NoSQL databases can be faster than SQL databases. Why? Data in SQL databases is typically normalized, so queries for a single object or entity require you to join data from multiple tables. As your tables grow in size, the joins can become expensive. However, data in NoSQL databases is typically stored in a way that is optimized for queries. The rule of thumb when you use MongoDB is Data is that is accessed together should be stored together. Queries typically do not require joins, so the queries are very fast.


- Easy for developers:   
Some NoSQL databases like MongoDB map their data structures to those of popular programming languages. This mapping allows developers to store their data in the same way that they use it in their application code. While it may seem like a trivial advantage, this mapping can allow developers to write less code, leading to faster development time and fewer bugs.

**sql modeling techniques:**

1. Hierarchical Technique:  
The hierarchical model is a tree-like structure. There is one root node, or we can say one parent node and the other child nodes are sorted in a particular order. But, the hierarchical model is very rarely used now. This model can be used for real-world model relationships.

2. Object-oriented Model:  
The object-oriented approach is the creation of objects that contains stored values. The object-oriented model communicates while supporting data abstraction, inheritance, and encapsulation.

3. Network Technique:  
The network model provides us with a flexible way of representing objects and relationships between these entities. It has a feature known as a schema representing the data in the form of a graph. An object is represented inside a node and the relation between them as an edge, enabling them to maintain multiple parent and child records in a generalized manner.

4. Relational Technique:  
Relational is used to describe the different relationships between the entities. And there are different sets of relations between the entities such as one to one, one to many, many to one, and many to many.
