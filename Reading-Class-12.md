# CRUD

## HTTP response status codes

**- Each group of status code represents:**

- 100’s = The response status codes here have Informational responses.

- 200’s = The response status codes here have Successful responses.

- 300’s = The response status codes here have Redirects .

- 400’s = The response status codes here have Client errors.
- 500’s = The response status codes here have Server errors.


**- What is a status code 202?**  
**202 Accepted:** The request has been received but not yet acted upon. It is noncommittal, since there is no way in HTTP to later send an asynchronous response indicating the outcome of the request.

**- What is a status code 308?**

**308 Permanent Redirect:** 
This means that the resource is now permanently located at another URI, specified by the Location: HTTP Response header.

**- What code would you use if an update didn’t return data to a client?**

204 No Content

**- What code would you use if a resource used to exist but no longer does?**

404 Not Found

**- What is the ‘Forbidden’ status code?**

403 Forbidden


## Build A REST API With Node.js, Express, & MongoDB - Quick

**- Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

Becuase its using a local host string path and when we deploy our application it won't be in our local host so we put it in `.env`.

**- What is middleware?**

Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

**- What does app.use(express.json()) do?**

express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app.

**- What does the /:id mean in a route?**

Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

**- What is the difference between PUT and PATCH?**

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

**- How do you make a default value in a schema?**

Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.


**- What does a 500 error status code mean?**

The HTTP status code 500 is a generic error response. It means that the server encountered an unexpected condition that prevented it from fulfilling the request.

**- What is the difference between a status 200 and a status 201?**

The 200 status code means that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).
