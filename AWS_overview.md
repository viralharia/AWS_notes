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
     