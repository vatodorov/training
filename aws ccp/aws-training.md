
# Module 1 - Introduction


## Benefits of cloud computing

* Trade upfront expense (servers/infrastructre) for variable expense (pay for servers when you need them)
* Stop spending money to run and maintain data centers - Computing in data centers often requires you to spend more money and time managing infrastructure and servers
* Stop guessing capacity - With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application
* Benefit from massive economies of scale - lower variable cost with cloud than doing it on my own
* Increase speed and agility
* Go global in minutes


## AWS Developer Tools
* Web Console
* Command Line Tool
* Integrated Development Environment (IDE)
* Software Development Kit (SDK)
* Infrastructure as Code


## Cloud Computing Models
* Infrastructure as a Service (IaaS) - contains the basic building blocks for cloud IT and typically provide access to networking features, computers (virtual or on dedicated hardware), and data storage space.
* Platform as a Service (PaaS) - PaaS removes the need for organizations to manage the underlying infrastructure (usually hardware and operating systems) and allow you to focus on the deployment and management of your applications.
* Software as a Service (SaaS) - SaaS gives you a completed product that is run and managed by the service provider. In most cases, people referring to Software as a Service are referring to end-user applications


## Cloud Computing Deployment Models
* Cloud
* On-prem
* Hybrid



# Module 2 - Compute in the cloud

## EC2 Instance types
* General purpose
* Compute optimized
* Memory optimized
* Accelerated computing
* Storage optimized


## Pricing
* On-demand - get it on demand
* EC2 savings plan - Amazon EC2 Savings Plans enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term. This term commitment results in savings of up to 66% over On-Demand costs.
* Reserved instance - billing discount applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term, and Scheduled Reserved Instances for a 1-year term. You realize greater cost savings with the 3-year option.
* Spot instances - ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot Instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off of On-Demand prices.
* Dedicated Hosts - physical servers with Amazon EC2 instance capacity that is fully dedicated to your use. 


## Scaling
* Amazon EC2 auto scaling


## Elastic load balancing
* Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances. A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. 


## Messaging and queueing
When designing applications on AWS, you can take a microservices approach with services and components that fulfill different functions. Two services facilitate application integration: Amazon Simple Notification Service (Amazon SNS) and Amazon Simple Queue Service (Amazon SQS).

* Monolithic applications - These components might include databases, servers, the user interface, business logic, and so on. This type of architecture can be considered a monolithic application. In this approach to application architecture, if a single component fails, other components fail, and possibly the entire application fails.
* Microservices - In a microservices approach, application components are loosely coupled. In this case, if a single component fails, the other components continue to work because they are communicating with each other. The loose coupling prevents the entire application from failing. 

* Amazon Simple Notification Service (Amazon SNS) - a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers
* Amazon Simple Queue Service (Amazon SQS) - a message queuing service. Using Amazon SQS, you can send, store, and receive messages between software components, without losing messages or requiring other services to be available. In Amazon SQS, an application sends messages into a queue. A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.


## Additional compute services
* AWS Lambda - Serverless computing.AWS Lambda is a service that lets you run code without needing to provision or manage servers. While using AWS Lambda, you pay only for the compute time that you consume. Charges apply only when your code is running. You can also run code for virtually any type of application or backend service, all with zero administration. 


## Containers
* Amazon Elastic Container Service (Amazon ECS) - a highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS. Amazon ECS supports Docker containers.
* Amazon Elastic Kubernetes Service (Amazon EKS) - fully managed service that you can use to run Kubernetes on AWS. 
* AWS Fargate - serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS. When using AWS Fargate, you do not need to provision or manage servers. AWS Fargate manages your server infrastructure for you. You can focus more on innovating and developing your applications, and you pay only for the resources that are required to run your containers.

* 
* 
* 
