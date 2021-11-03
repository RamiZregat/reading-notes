# Express

**- What’s the difference between PUT and PATCH?**

- The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

![](https://www.devopsschool.com/blog/wp-content/uploads/2020/04/put-vs-post-patch.jpg)

**- Provide links to 3 services or tools that allow you to “mock” an API for development like json-server:**   

1. [Postman](https://www.postman.com/)

2. [Wiremock](http://wiremock.org/)

3. [MockServer](https://www.mock-server.com/)


**- Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?**  

- Swagger 

```
  '200':
    description: OK
  '400':
    description: Bad request. User ID must be an integer and larger than 0.
  '401':
    description: Authorization information is missing or invalid.
  '404':
    description: A user with the specified ID was not found.
  '5XX':
    description: Unexpected error
```

- APIDoc.js 1

```
  '200':
  	Successful request and response.
  '400':
  	Malformed parameters or other bad request.
```

**- Compare and contrast SOAP and ReST:**  

- SOAP is a XML-based message protocol, while REST is an architectural style.

- SOAP uses WSDL for communication between consumer and provider, whereas REST just uses XML or JSON to send and receive data. 

- SOAP invokes services by calling RPC method, REST just simply calls services via URL path.

- SOAP doesn't return human readable result, whilst REST result is readable with is just plain XML or JSON.

- SOAP is not just over HTTP, it also uses other protocols such as SMTP, FTP, etc, REST is over only HTTP.

![](https://3.bp.blogspot.com/-zg3xuzcWTXg/Vaj0gLvGabI/AAAAAAAADZU/fhE-v_AXJFA/s640/SOAP%2Bvs%2BREST%2Bin%2BJava.png)

Term|Meaning
------------|-----
Web Server |A web server is computer software and underlying hardware that accepts requests and send responses via HTTP or its secure variant HTTPS, the network protocols created to distribute web contents  to client user agents.
Express|It is a web framework written in JS and hosted by node.js
Routing|Routing is the process of selecting a path for traffic in a network or between or across multiple networks. Broadly, routing is performed in many types of networks, including circuit-switched networks, such as the public switched telephone network, and computer networks, such as the Internet.
WRRC|web request/response cycle traces how a user’s request flows through the app.



**- Which 3 things had you heard about previously and now have better clarity on?**  

- middleware
- the backend development
- testing

**- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**  

- CI/CD
- How can i test the whole project
- routing

**- What are you most excited about trying to implement or see how it works?**  

that its actually works with me :) 



## Preview
**- NodeJS and Express:** 

- What is difference between node JS and express JS?

Express. js is a framework based on Node. js for which is used for building web-application using approaches and principles of Node. js.

Feature|Node.js|Express.js
-----|----|-----
Level of features	|Fewer features|More features than Node.js
Building Block	| It is built on Google's V8 engine| It is built on Node.js.	


**- What is NPM?**  
npm is the package manager for the Node JavaScript platform. It puts modules in place so that node can find them, and manages dependency conflicts intelligently.

**- What is TDD?**  
Test Driven Development (TDD) is a programming practice that instructs developers to write new code only if an automated test has failed.

**- CI/CD**  
CI/CD is a method to frequently deliver apps to customers by introducing automation into the stages of app development. The main concepts attributed to CI/CD are continuous integration, continuous delivery, and continuous deployment. CI/CD is a solution to the problems integrating new code can cause for development and operations teams.

