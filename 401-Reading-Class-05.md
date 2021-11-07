# Authentication  

####  Singleton
A singleton or (singleton pattern) is a function or class which can have only one instance. It is a way of creating a single object that is shared with different part of the application or 3rd party users, without recreating it instance each time we want to use it

Only one instance of this object can instantiate at a time.  

### Singleton in Node  
1. We create a Singleton class in a js folder. We make a condition, that if there is no instance created, then we create it . After that we return the Singleton object.instance.  

```
class Singleton {
  constructor(){
    if(!Singleton.instance){
      Singleton.instance = this;
    }
    return Singleton.instance;
  }
}
```    
2. We instantiate our instance    

```
const ourInstance = new Singleton()  
```

3. We export only the instance.  
```
module.exports = ourInstance;
```  
4. We import out instance to where we want to use it.  

#### Approaches to construct/operate a middleware system  
I'll look for what services that my app will present and it's interface with other apps, to so it's middleware system can be vital to accept or refuse the interface of requests.The app middleware should have access to all app services and it is the one that put the rules of weather they are good to be processed or not. 


## Terms  
term | definition
--- | ---
Router Middleware | Router level middleware can be defined in the same way as application-level middleware
Dynamic Module Loading | The dynamic module loader library allows code to retrieve Node modules from a web server, install them locally and serve them up as though they’d been manually deployed to the running server.
Singleton Pattern | The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.
CRUD -> REST Method Matches | When the class is reduced to one instance, and the constructor is remembered, the same instance returns
Mock Testing | Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behavior of the real ones. … Such a service can be replaced with a mock object.   


## Preview  
1. Which 3 things had you heard about previously and now have better clarity on?  
  - Linked List.  
  - middleware systems.  
  - CRUD apps.  

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Singletons
  - middleware systems.
  - Authentication

3. What are you most excited about trying to implement or see how it works?
  - Singleton Pattern
  - Authentication
  - More tests 


  ## Preparation Materials

 ### Securing Passwords

 - Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

 - We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.


- Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

- The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. But why do we always hear about passwords being cracked? There are some weaknesses in cryptographic hash algorithm that allows an attacker to calculate the original value of a hashed password.

- PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM:
1. Brute Force attack: Hashes can't be reversed, so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack.

2. Hash Collision attack: Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash. MD5, SHA1, SHA2 are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.

3. BCrypt, IT's SLOW AND STRONG AS HELL
To overcome such issues, we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.

### Basic Auth

- In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon `:`

- When the server wants the user agent to authenticate itself towards the server after receiving an unauthenticated request, it must send a response with a HTTP 401 Unauthorized status line.

### OWASP auth cheatsheet

- Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

- Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict


### bcrypt docs

- A library to help you hash passwords.

- Verify that the node version you are using is a stable version; it has an even major release number. Unstable versions are currently not supported and issues created while using an unstable version will be closed.

- installation:   
Install via NPM 


```
npm install bcrypt
```

- Usage:   
async (recommended):  


```
const bcrypt = require('bcrypt');
const saltRounds = 10;
const myPlaintextPassword = 's0/\/\P4$$w0rD';
const someOtherPlaintextPassword = 'not_bacon';
```


- Why is async mode recommended over sync mode?   
If you are using bcrypt on a simple script, using the sync mode is perfectly fine. However, if you are using bcrypt on a server, the async mode is recommended. This is because the hashing done by bcrypt is CPU intensive, so the sync version will block the event loop and prevent your application from servicing any other inbound requests or events. The async version uses a thread pool which does not block the main event loop.