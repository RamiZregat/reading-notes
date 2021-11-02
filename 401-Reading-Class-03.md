# Express REST API

**- Name 3 real world use cases where you’d want to change the   request with custom middleware:**  

- Async Actions
- Routing
- Login authentication

**- True or false: The route handler is middleware?**  

- False, they are not middleware functions by definition. If such function is used on routing methods then they are only handler functions. We use such a handler function which is not a middleware when it is the only one callback function.

**- In what ways can a middleware function end the process and send data to the browser?**  

In 2 ways:

- Throwing an error throw new Error(‘error message’)
- next('error message')

**- At what point in the request lifecycle can you “inject” middleware?**  
 
The generated server allows for 3 extension points to inject middleware in its middleware chain. These are:

1. to add middleware all the way to the top of the middleware stack.

2. right before actually handling a matched request.

3. setting the middleware for existing handler by its route and HTTP method. It can be done in the configureAPI function by calling api.AddMiddlewareFor method.

 **- What can cause express to error with “Request headers sent twice, cannot start a second response”**  

 The request handler function already sent a response to the client using the res.json() method which automatically sets the response header(every response to the client should contain headers) for the response(in this case theContent-Type to application/json). Node picks up this atrocity and our server crashes because express under the hood is attempting to set the response header for this second response.


 Term|Meaning
-----|-----
Middleware|Middleware functions can perform the following tasks: Execute any code. Make changes to the request and the response objects.
Request Object|represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
Response Object|represents the HTTP response that an Express app sends when it gets an HTTP request.
Application Middleware|bound to an instance of express, using app. use() and app. VERB(). Router level middleware work just like application level middleware except they are bound to an instance of express.
Routing Middleware|Routing defines the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware.
Test Driven Development|is an iterate process that begins with writing a test code for an application or function before starting out to write the application.
Behavioral Testing|s a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests.





 **- Which 3 things had you heard about previously and now have better clarity on?**  

- Databases.

- APIs.

- Request cycle.  

**- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**  

- noSQL

- Authentication

- middleware usage

**- What are you most excited about trying to implement or see how it works?**  

- middleware functions

**Review: ES6 Classes**
- Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

- In ES6 we can create classes, the class function basically creates a template that we can use to create objects later, the constructor() method is a special method called when an instance of the User class is created.

**Using Express Routing**  
- Routing refers to how an application’s endpoints (URIs) respond to client requests.

- You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function.

**Express Routing**  
- Use the express.Router class to create modular, mountable route handlers. A Router instance is a complete middleware and routing system; for this reason, it is often referred to as a “mini-app”.
 




