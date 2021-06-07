# AWS: S3 and Lambda

AWS Lambda allows writing code that is triggered in the cloud, without thinking about maintaining servers.

## Review, Research, and Discussion

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources.

1. Describe “The Cloud”
   is the on-demand availability of computer system resources, especially data storage (cloud storage) and computing power, without direct active management by the user.
2. What is a container (as it relates to computers and servers)?
   virtualize CPU, memory, storage, and network resources at the OS-level, providing developers with a sandboxed view of the OS logically isolated
3. What is auto-scaling?
   AWS Auto Scaling lets you build scaling plans that automate how groups of different resources respond to changes in demand.
4. What is bandwidth?
   a measure of how much information a network can transfer. The volume of data that can be transported varies, impacting how effectively a transmission medium, such as an Internet connection, operates.
5. How do cloud providers compute service costs?
   loud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.

## Vocabulary Terms

| word               | Defintion                                                                                                                                                                         |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Server Instances   | is a collection of SQL Server databases which are run by a solitary SQL Server service or instance                                                                                |
| Containers         | services are deeply integrated with AWS by design. This allows your container applications to leverage the breadth and depth of the AWS cloud                                     |
| Cloud Services     | are services available via a remote cloud computing server rather than an on-site server.                                                                                         |
| Cloud Architecture | refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. |
| AWS                | Amazon Web Services, a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals.                                                                |
|                    |                                                                                                                                                                                   |

## Preview

- Heroku Application

  - Heroku automatically manages, e.g, performs upgrades for, the Dynos and Heroku Postgres resources

  - Heroku automatically manages the DATABASE_URL and PORT environment variables.

  - Professional level Dynos are required to enable horizontal scaling and thus high availability (or something approximating it).

  - the PostgreSQL instances are publicly available; secured using SSL and an username / password pair.

- AWS Elastic Beanstalk Application

  - AWS automatically manages, e.g, performs upgrades for, the PostgreSQL and EC2 Instances.
  - AWS Elastic Beanstalk automatically manages the PORT environment variable.
  - EC2 and PostgreSQL Instances are in private Subnets and further secured using Security Groups. The PostgreSQL Instances are also secured using SSL and a username / password pair.

### AWS Lambda Basics

- AWS Lambda is a service which computes the code without any server. It is said to be serverless compute. The code is executed based on the response of events in AWS services such as adding/removing files in S3 bucket, updating Amazon DynamoDB tables, HTTP request from Amazon API Gateway etc.

- CDN:
  A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.
