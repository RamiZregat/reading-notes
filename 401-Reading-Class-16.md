# AWS: Cloud Servers 

## Review, Research, and Discussion  
### Web-Request-Response-Cycle  
- The web is a cycle of requests and responses that flow between clients and servers.  
This cycle start when a client is asking for a resource from a certain server. The asking is the **request**,and it can be summarized in 4 methods. `GET`, `POST`, `PUT` AND `DELETE`. The **Request** is sent with address and parameters. After that the server receive the request and respond with which ever the client want. this this is called the **Response**, and normally it contains a status code, `200` if successful and the resource the client requested.  
### Server and WRRC  
A **server** is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.  
In the `web` we interact with a `web server`, which is a computer program that serves requested HTML pages or files. In this case, a web browser acts as the client. Usually the server interact with a database by the request of the client.  
### Application Deployment  
When a developer builds an application on his/her computer, it is locally stored and an only be accessed throw its machine/device. However, i the developer want to share the application with others, he/she needs to upload the application on the web and make it active with all of its components. This is called deployment.  

---  


## Term  
Server :

  > A server is a computer program or device that provides a service to another computer program and its user, also known as the client. In a data center, the physical computer that a server program runs on is also frequently referred to as a server. That machine might be a dedicated server or it might be used for other purposes.  

Pub/Sub:

  > Publish/Subscribe allows services to communicate asynchronously, with latencies on the order of 100 milliseconds. Pub/Sub is used for streaming analytics and data integration pipelines to ingest and distribute data. It is equally effective as messaging-oriented middleware for service integration or as a queue to parallelize tasks.  

WRRC:

  > The request/response cycle traces how a user’s request flows through the app , it includes the client sending a request to the backend server , the backend server would do some process then send a response back to the client 
  
---  

## Preparation Materials  
### Virtual Machine  
**Operating system**:  
  > It is a software that control the hardware of a computer.  
**Virtual Machine Manager**:  
  > It is a software that allows us to run an operating system within another operating system.  
  Examples:   
    1. VirtualBox  
    2. vmware  
- An operating system created by `Virtual Machine Manager` is called a `Virtual Machine`.  

#### Reasons to use Virtual Machines:
  1. Trying a new operating system.
  1. Testing an application.
  1. Running old applications.  

### Virtualization and Cloud Computing  
- **Virtualization**  allows us to better utilize the resources we have available in out machine.  

Virtualization is when many **Virtualization Machines** are controlled and operate inside one single machine. This gives us the following advantages:  
  - Fewer machines.
  - Lower capital investment.
  - Centralized management.
  - Lower operation cost.

- **Cloud Computing** is when someone is using a computer that is in another location.  

### AWS EC2
It's a service provided by `Amazon`. The term **AWS EC2** stands for "Amazon Elastic Compute Cloud". it is a web service that provides secure, resizable compute capacity in the cloud.  
`Amazon` claims It is designed to make web-scale cloud computing easier for developers and it's simple web service interface allows you to obtain and configure capacity with minimal friction. Also, It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.  

### EC2 For Humans  
**EC2** is a service, where clients can rent a like server (not physical machine) or in other words virtual machine, that is independent form other virtual machines that are on aws server.  

Throw `amazon` site you can create an instance , where you can choose the type of operating system, memory size, number of CPUs, storage capacity and more.  

This virtual machine can be used for storing data, web application, machine learning and more.

There are different settings that fit each usage, related to access and privacy.  

### Elastic Beanstalk  
**Elastic Beanstalk** is a service that deploys, manages and scales web apps and services on behave of the developer.  

**Elastic Beanstalk** uses managed containers like:  
  - `java.net`
  - `PHP`
  - `Node.js`
  - `Python`
  - `Ruby`
  - `docker`

It also works on familiar servers such as :  
  - apache HTTP
  - apache tomcat
  - engin x
  - passenger
  - IIS  

**Elastic Beanstalk** leverages familiar AWS services such as :  
  - Amazon EC2
  - Amazon S3
  - Amazon simple notification service
  - Amazon elastic load balancing
  - Amazon auto scaling  

To start with **Elastic Beanstalk** you can use, AWS management console, the command line interface or the API. choose your platform and amazon EC2 instance type, then select additional resources to use such as Amazon relational database service, then upload yor code.  

**Elastic Beanstalk** will handle Load Balancing, Provisioning, Auto Scaling and Application Health Monitoring.