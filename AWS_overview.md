# Cloud Computing
* Cloud Computing is simply the delivery of IT resources over the Internet.
* IT resources here means:
    * Compute power
    * Storage service
    * Networking
    * Security services
    * Analytics, artificial intelligence etc

### Main benefits of cloud:
* Agility
* Elasticity
* Cost savings

### Types of Cloud Computing:
#### Infrastructure-as-a-Service (IaaS)
* The provider supplies virtual server instances, storage, and mechanisms for you to manage servers.
* Infrastructure as a Service provides you with the highest level of flexibility and management control over your IT resources.
* You manage the servers and applications both in IaaS.
* Ex - AWS, Digital Ocean, Rackspace.
Actually, Amazon Web Services (AWS) provides a mix of infrastructure as a service (IaaS), platform as a service (PaaS) and packaged software as a service (SaaS) offerings.
#### Platform-as-a-Service (PaaS)
* A platform of development tools hosted on a provider's infrastructure.
* The PaaS provider manages development tools such as OS, runtimes such as JDKs etc. and you just need to take care of the application development and deployment
* Ex - Heroku
#### Software-as-a-Service (SaaS)
* A software application that runs over the Internet and is managed by the service provider.
* Ex - Microsoft O365, Gmail
****
# Elastic Cloud Compute
* Elastic Cloud Compute or EC2 is a foundational piece of AWS' cloud computing platform and is a service that provides servers for rent in the cloud.

## Pricing Options
There are several pricing options for EC2.
1. On Demand - Pay as you go, no contract.
2. Dedicated Hosts - You have your own dedicated hardware and don't share it with others.
3. Spot - You place a bid on an instance price. If there is extra capacity that falls below your bid, an EC2 instance is provisioned. If the price goes above your bid while the instance is running, the instance is terminated.
4. Reserved Instances - You earn huge discounts if you pay up front and sign a 1-year or 3-year contract.
****
# Elastic Block Store
* Elastic Block Store (EBS) is a storage solution for EC2 instances and is a physical hard drive that is attached to the EC2 instance to increase storage.
* There are several EBS volume types that fall under the categories of Solid State Drives (SSD) and Hard Disk Drives (HDD).
* Benefit of EBS is that data is persisted after an EC2 instance is terminated.
****
# Virtual Private Cloud (VPC)
* Virtual Private Cloud or VPC allows you to create your own private network in the cloud. You can launch services, like EC2, inside of that private network. A VPC spans all the Availability Zones in the region.
* VPC allows you to control your virtual networking environment, which includes:
    * IP address ranges
    * subnets
    * route tables
    * network gateways
* You can easily customize the network configuration for your Amazon VPC. For example, you can create a public-facing subnet for your web servers that has access to the Internet, and place your backend systems such as databases or application servers in a private-facing subnet with no Internet access.
* Your AWS resources are automatically provisioned in a ready-to-use default VPC that was created for you. You can configure this VPC by adding or removing subnets, attaching network gateways, changing the default route table and modifying the network ACLs.
* Resources:
    * https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html
    * https://aws.amazon.com/vpc/
# Elastic Beanstalk
* Elastic Beanstalks is an orchestration service that allows you to deploy a web application at the touch of a button by spinning up (or provisioning) all of the services that you need to run your application.
* Elastic Beanstalk can spin up database instances for you, VPCs, security groups, EC2 instances.
****
# Storage 
* Amazon Simple Storage Service (Amazon S3)
* Amazon Simple Storage Service (Amazon S3) Glacier

## Amazon Simple Storage Service (Amazon S3)
* Amazon Simple Storage Service (or S3) is an object storage system in the cloud.
* Examples of things that can be stored in it includes - Text documents, Image files, HTML files.
* There are several use cases for S3, hosting static websites, content delivery, backup and recovery, archiving and big data, application data, and hybrid cloud storage.
* **_SignedURLs_** allow clients to send and receive data by directly communicating with the file store. This saves the server from using its bandwidth to serve as the intermediary that transmits data to and from the client. This is faster for clients as well.

### Storage Classes
* S3 offers several storage classes, which are different data access levels for your data at certain price points.
    * S3 Standard
    * S3 Glacier
    * S3 Glacier Deep Archive
    * S3 Intelligent-Tiering
    * S3 Standard Infrequent Access
    * S3 One Zone-Infrequent Access
****
# Database Services
* DynamoDB
    * DynamoDB is a NoSQL document database service that is fully managed. Unlike traditional databases, NoSQL databases, are schema-less. Schema-less simply means that the database doesn't contain a fixed (or rigid) data structure.
* Relational Database Service (RDS)
    * RDS (or Relational Database Service) is a service that aids in the administration and management of databases. RDS assists with database administrative tasks that include upgrades, patching, installs, backups, monitoring, performance checks, security, etc.
    * Features
        * failover
        * backups
        * restore
        * encryption
        * security
        * monitoring
        * data replication
        * scalability
* Redshift
    * Redshift is a cloud data warehousing service to help companies manage big data. Redshift allows you to run fast queries against your data using SQL, ETL, and BI tools. Redshift stores data in a column format to aid in fast querying.
* ElastiCache
* Neptune
* Amazon DocumentDB
****
# Cloud Front
* CloudFront is used as a global content delivery network (CDN). Cloud Front speeds up the delivery of your content through Amazon's worldwide network of mini-data centers called Edge Locations.
* CloudFront ensures that end-user requests are served from the closest edge location.
* Cache control headers determine how frequently CloudFront needs to check the origin for an updated version your file.
* The maximum size of a single file that can be delivered through Amazon CloudFront is 20 GB.
* CloudFront works with other AWS services, as shown below, as an origin source for your application:
    * Amazon S3
    * Elastic Load Balancing
    * Amazon EC2
    * Lambda@Edge
    * AWS sheild
****
# Identity & Access Management
* Identity & Access Management (IAM) is an AWS service that allows us to configure who can access our AWS account, services, or even applications running in our account. IAM is a global service and is automatically available across ALL regions.
* Security Concepts
    * User
    * IAM Group
    * IAM Role
        * IAM user role: an IAM role can give a user a set of permissions to access one or more services.
        * IAM service role: an IAM role gives a service a set of permissions to access one or more services   
    * Policy

## Access keys
* You use access keys to sign programmatic requests that you make to AWS if you use AWS CLI commands (using the SDKs) or using AWS API operations.
* Access keys consist of two parts: an access key ID (for example, AKIAIOSFODNN7EXAMPLE) and a secret access key (for example, wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY).
*  Resources
    *   https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html
****
# Networking
## Route 53
* Route 53 is a cloud domain name system (DNS) service that has servers distributed around the globe used to translates human-readable names like www.google.com into the numeric IP addresses like 74.125.21.147.
    * Features
        * scales automatically to manage spikes in DNS queries
        * allows you to register a domain name (or manage an existing)
        * routes internet traffic to the resources for your domain
        * checks the health of your resources.
  * This service allows you to set up routing profiles for your domain names and direct traffic to services inside of and external to AWS.

## Elastic Load Balancing
* Elastic Load Balancing automatically distributes incoming application traffic across multiple servers.
* Elastic Load Balancer is a service that:
    * Balances load between two or more servers
    * Stands in front of a web server
    * Provides redundancy and performance.
    * Elastic Load Balancing works with EC2 Instances, containers, IP addresses, and Lambda functions.
    * You can configure Amazon EC2 instances to only accept traffic from a load balancer.
**** 
# Simple Notification Service
* Amazon Simple Notification Service (or SNS) is a cloud service that allows you to send notifications to the users of your applications. SNS allows you to decouple the notification logic from being embedded in your applications and allows notifications to be published to a large number of subscribers.
* SNS uses a publish/subscribe model.
SNS can publish messages to Person(Mobile Push, text message, email), other AWS services such as Amazon SQS queues, AWS Lambda functions, and HTTP/S webhooks.
****
# Cloud Trail
* Cloud Trail allows you to audit (or review) everything that occurs in your AWS account. Cloud Trail does this by recording all the AWS API calls occurring in your account and delivering a log file to you.
* CloudTrail provides event history of your AWS account activity, including:
    * who has logged in
    * services that were accessed
    * actions performed
    * parameters for the actions
    * responses returned
* This includes actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services.
****
# Cloud Watch
* Cloud Watch is a service that monitors resources and applications that run on AWS by collecting data in the form of logs, metrics, and events.
* Features
    * Collect and track metrics
    * Collect and monitor log files
    * Set alarms and create triggers to run your AWS resources
    * React to changes in your AWS resources
****
# Cloud Formation
AWS Cloud Formation allows you to model your entire infrastructure in a text file template allowing you to provision AWS resources based on the scripts you write.
* Cloud Formation templates are written using JSON or YAML.
* You can still individually manage AWS resources that are part of a CloudFormation stack.
