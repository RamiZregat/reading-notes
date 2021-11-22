# AWS: S3 and Lambda

## Review, Research, and Discussion

### The Cloud

**The cloud** refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines.

### Computers and servers containers

Containers are a solution to the problem of how to get software to run reliably when moved from one computing environment to another. A container consists of an entire runtime environment: an application, plus all its dependencies, libraries and other binaries, and configuration files needed to run it, bundled into one package. By containerizing the application platform and its dependencies, differences in OS distributions and underlying infrastructure are abstracted away.

### Auto-scaling

**Auto scaling** is a cloud computing technique for dynamically allocating computational resources. Depending on the load to a server farm or pool, the number of servers that are active will typically vary automatically as user needs fluctuate.

### Bandwidth

The volume of information that can be sent over a connection in a measured amount of time – calculated in megabits per second (Mbps).

### Computing service costs

They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.

---

## Terms

> Server Instances : A collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

> Containers: A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another

> Cloud Services: services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

> Cloud Architecture: Cloud architecture is the way technology components combine to build a cloud, in which resources are pooled through virtualization technology and shared across a network

> AWS: Amazon Web Services is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis.

> EC2/Beanstalk vs Heroku:
>- One big difference is that Heroku’s pricing takes exponential price jumps as one adds common additional features, e.g., auto-scaling, where-as AWS pricing is fairly linear. On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.
>- Costs are nearly comparable when deploying an application.
>- AWS Elastic Beanstalk solution’s PostgreSQL Instances, being in private Subnets with restricted Security Groups, are more secure than the publicly available PostgreSQL Instances in the Heroku solution.
>- Heroku’s Dyno high availability, by randomly distributing across Availability Zones, is less robust than the AWS Elastic Beanstalk’s (actually powered by an EC2 Auto Scaling Group) active distribution across Availability Zones.
>- While we did not explore AWS Elastic Beanstalk’s Auto Scaling Group feature, it is available at no cost. For Heroku, Autoscaling is currently available only for Performance-tier dynos and dynos running in Private Spaces.

---

## Preparation Materials

### AWS S3

Amazon Simple Storage Service (Amazon S3) is an object storage service. Amazon claims that it offers industry-leading scalability, data availability, security, and performance.

- Benefits
  - Industry-leading performance, scalability, availability, and durability.
  - Wide range of cost-effective storage classes.
  - Unmatched security, compliance, and audit capabilities.
  - Easily manage data and access controls.
  - Query-in-place and process on-request.
  - Most supported cloud storage service.



### AWS Lambda Basics

**AWS Lambda** is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

- The Lambda functions can perform many computing task like:

  - serving web pages.
  - processing streams of data.
  - calling APIs and integrating with other AWS services.

- Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete.

- AWS Lambda is one of the main candidates for running the application code, because Lambda fills the primary role of the compute service on AWS. It also integrates with many other AWS services and, together with API Gateway, DynamoDB and RDS, forms the basis for Serverless solutions for those using AWS.

AWS Lambda is most useful where:

- individual tasks run for a short time.
- each task is generally self-contained.
- there is a large difference between the lowest and highest levels in the workload of the application.

Some of the most common use cases for AWS Lambda that fit these criteria are:

- Scalable APIs.
- Data processing.
- Task automation.

Supported languages and runtimes:

- Node.js 8.10
- Node.js 10.x (normally the latest LTS version from the 10.x series)
- Node.js 12.x (normally the latest LTS version from the 12.x series)
- Python 2.7
- Python 3.6
- Python 3.7
- Python 3.8
- Ruby 2.5
- Java 8
- Java 11
- Go 1.x (latest release)
- C# — .NET Core 1.0

### AWS Lambda Functions

Benefits:

- No servers to manage.
- Continuous scaling.
- Cost optimized with millisecond metering.
- Consistent performance at any scale.


Use cases:

- Data processing.

- Real-time file processing.  

- Real-time stream processing.  

- Machine learning.

- Backends.

- Web applications.  

- IoT backends  

- Mobile backends.  


## CDN


A **Content Delivery Network** (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content.

- CDNs work through servers nearest to the website visitor respond to the request.
- When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content.
- CDNs will also communicate with the originating server to deliver any content that has not been previously cached.
- Employing a CDN doesn’t only speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks, such as Denial of Service attacks. It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers.
- Reasons why company want to use CDNs:

  - improve Internet website load speeds.
  - improve content delivery speeds.
  - reduce the likelihood of falling victim to and improve defenses against Distributed Denial of Service attacks (DDoS).

- A smaller company probably doesn’t need to improve website load speeds with a CDN, because they don’t have an overwhelming amount of traffic, and it's not within their budget to pay for such service.

- The best advice to an SMB (small to medium Bushiness) is to know what a CDN is, and at most, establish a relationship with a CDN protection vendor without paying for protection. DDoS protection vendors include: Arbor Networks, AT&T, Verizon, and Akamai.
