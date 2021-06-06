# AWS: Cloud Servers

# Readings: AWS: Cloud Servers
## Review, Research, and Discussion
* Describe the Web-Request-Response-Cycle
    * WRRC is a cycle that show the flow of data when a user or server make request to specific site then this request will go to the ISP (internet service provider) to check the DNS (Domain name server, which is basically a lot of IP addresses) and find to you the IP address of the server you are requesting then send request to that server and that server will check this request and check the databases then back with a response to your ISP and back to you with the final results.
* Explain what a “server” is, as it relates to the WRRC
    * a computer that runs all the time and deal with requests (HTTP) and responses form clients or other servers, also sending requests to the database and back to the clients with responses.
* What does it mean to “deploy” an application?
    *  is the process of installing, configuring, and enabling a specific application or set of applications, usually through an application manager (app manager) or software management system, to a specific URL on a server. Once the process of deploying the application(s) has been completed it becomes publicly accessible on the URL.
## Document the following Vocabulary Terms
* A Web server:  is a program that uses HTTP (Hypertext Transfer Protocol) to serve the files that form Web pages to users, in response to their requests, which are forwarded by their computers' HTTP clients.
* Pub/Sub: is an asynchronous messaging service that decouples services that produce events from services that process events.
* WRRC:	The web is a cycle of requests and responses that flow between clients and servers.
## Virtual Machine
a machine that runs simultaneously on another device by sharing its resources with the original device
It can be considered a software that will allow you to run more than one OS (operating System, is a software that allow you to control the Hardware) on the same computer! We use VM to try another OS, Test application on another OS or to run applications that need different/older OS.

## AWS EC2
Amazon Elastic Compute Cloud it is a service that provides Cloud Computing in secure, resizable compute capacity. Amazon EC2 offer the fastest processors in the cloud and the only cloud with 400 Gbps ethernet networking. and you connect to it using CLI, SSH.
It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.
## EC2 For Humans
Amazon EC2 provides the following features:
* Bare Metal instances
* Optimize Compute Performance and Cost with Amazon EC2 Fleet
* Pause and Resume Your Instances
* Various configurations of CPU, memory, storage, and networking capacity for your instances, known as instance types
* GPU Compute Instances
* GPU Graphics Instances
* High I/O Instances
* Virtual computing environments, known as instances
* Dense HDD Storage Instances
* Optimized CPU Configurations
* Flexible Storage Options
* Paying for What You Use
* Multiple Locations
* Secure login information for your instances using key pairs (AWS stores the public key, and you store the private key in a secure place)
* Elastic IP Addresses
* Amazon EC2 Auto Scaling
* High Performance Computing (HPC) Clusters
* Enhanced Networking
* Elastic Fabric Adapter (Fast interconnect for HPC clusters)
* Available on AWS PrivateLink
* Amazon Time Sync Service
* Preconfigured templates for your instances, known as Amazon Machine Images (AMIs), that package the bits you need for your server (including the operating system and additional software)

## Elastic Beanstalk
AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS.
