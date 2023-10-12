## CIT 114
# Final Reading Notes
*Cloud Concepts Overview*
- Cloud Computing is the on-demand delivery of computing resources, applications, storage, power, etc. via the internet with pay-as-you-go spending (hourly)
- Deployment models: Cloud, Hybird, and On-premises (private cloud)
- Infastructure as a Service (IaaS) is paid for on a "pay for what you consume" basis
- Cloud computing benefits include massive enconomics of scale, increased speed and agility, no more guessing capacity, go global in minutes, and no money spending on data centers
- Software as a Service (SaaS) services are typically rented via a subscription model despite many being free for personal use

*Cloud Economics and Billing*
- Three fundamental drivers of AWS pricing model: Compute, Storage, and Data transfer
- Services like Amazon S3, EBS, or EFS have tiered pricing
- EC2 free-tier service offers 750 hours
- Total Cost of Ownership (TCO) is A financial estimate to help find the cost of a system
- Four AWS Support plans: Basic, Developer, Business, and Enterprise support
- Business and Enterprise plans offer 24/7 support via chat or phone

*AWS Global Infrastructure Overview*
- An AWS Region is a geographical area that usually conists of two or more availability zones
- Each region has multiple availability zones, which consist of one or more data centers
- Availability zoned are designed for fault isolation and are connect with other zones by private high-speed links
- AWS recommends replicating data and other resources across availability zones
- Each availability zone is a separated partition of the AWS infastructure
- AWS Edge Locations are used to ensure low latency delivery
- Applications can be run to decrease latency to end users
- Elactic and scalable is a dynamic adaption of capacity
- Fault-tolerance is the built-in redundancy of components

*AWS Cloud Security*
- Customer is responsible for security 'in' the cloud, and AWS is responsible for security 'of' the cloud
- AWS responsibilites: Software and Hardware/AWS Global Infrastructure
- Customer responsibilites: Operating system, Applications, Network, and Firewall configuration
- IAM is used to manage access to AWS resources
- Two types of IAM policies: identity-based and resource-base
- Best practice is to not use the AWS account root except when necessary
- AWS Acceptable Use Policy shows info about prohibited actions in the AWS infrastructure
- AWS Organizations can be used to manage and secure multiple AWS accounts
- AWS Key Management Service (KMS) can create and manage encryption keys
- AWS Shield is a DDoS protection service
- AWS supports encryption of data at rest and in transit

*Networking and Content Delivery*
- Networks consist of a router and subnets
- CIDR consists of a network identifer (routing prefix) and host identifier
- Subnets are ranges of IP addresses that divide a VPC
- Private subnets do not have direct access to the internet, which can only be given by a NAT gateway
- MAXIMUM subnet range is /16, MINIMUM subnet range is /28
- Elastic network interface can be attached/detached to an instance
- Only one IGW can be used with a VPC at one time
- Two types of endpoints: Gateway and Interface
- A Network Access Control List (ACL) is another layer of security at the subnet level
- Route 53 is a scalable Domain Name System (DNS) web service, that is used to route users to web applications
- Route 53 supports different kinds of routing, including Simple, Weighted, Latency, etc.
- CloudFront is a fast, global, and secure CDN service, and self-service model that consists of edge locations and regional edge cache

*Compute*
- An Amazon Machine Image (AMI) consists of a template for EC2 instance, account launch permissions, and storage volumes
- AWS Identity and Access Management (IAM) role are kept in instance profile
- A security group is a set of firewall rules that controls traffic to the instance
- Tags can be used to attach metadata to a EC2 instance
- CloudWatch is used to monitor EC2 instances
- On-Demand Instance: Pay by the hour with no-term commitments; low cost and flexiblility, but spiky workloads
- Spot Instance: Instances runs as long as accessible; larger scale, dynamic workload, but time-insensitive
- Reserved Instance: Full, partical, or no upfront payment; easy predictability, with steady-state workloads
- Dedicated Instance: Run VPC on hardware only for a single AWS customer; save money on licensing, but overly sensitive workloads
- Four Pillars of Cost Optimization: Right size, increase elasticity, optimal pricing model, and optimize storage choices
- A Docker is a software platform that allows to quickly to build, test, and run applications
- Lambda is a serverless compute service that supports multiple programming languages with completely automated administration, and pay-per-use pricing
- AWS Elastic Beanstalk is a managed service that can easily boot up web applications

*Storage*
- Amazon Elastic Block Store (EBS) provide storage volumes for EC2 instances
- Block storage is more faster and uses less bandwidth than object storage, but costs more
- Snapshots can recreate a new volume at any time
- Amazon Simple Storage Service (S3) stores data as objects in buckets, with virtually unlimited storage
- Stored data can be accessed through managment console, command line interface, or SDK
- Amazon Elastic File Service (EFS) is a file storage for EC2 instances with elastic capacity and shared storage
- EFS is intended for big data and analytics, web serving, media workflows, etc.
- AWS S3 Glacier is a data archiving service designed for security, durability, and low cost
- Glacier can configure lifecycle archiving of data

*Databases*
- Amazon RDS is a managed service that sets up and runs a relational cloud database, with read replication
- RDS is typically used for web, mobile, and ecommerce applications and games; and complex transactions or queries
- RDS can automatically patch software and back up a database
- DynamoDB is a fast and flexible NoSQL database service for any scale and read-write throughput
- DynamoDB can query tables and retrive items using the query operation
- DynamoDB offers two kinds of primary keys: Partition key and partition and sort key
- Amazon Redshift is a fast, fully managed data warehouse that easily anaylzes data
- Redshift is compatible with SQL and existing business intelligence tools
- Redshift is useful for enterprise data warehouse and big data
- Amazon Aurora is a enterprise-class relational database, compatible with MySQL and PostgreSQL
- Aurora is a fast, simple, pay-as-you-go, and managed service; and can automate time-consuming tasks
- Aurora has high availablility and is designed for instant crash recovery

*Cloud Architecture*
- Pillars of AWS Well-Architected Framework: Operational excellence, security, reliability, performance efficiency, cost optimization
- Perform operations as code and annotate documentation; frequently make small, reversible changes; anticipate failure and learn from them
- Implement strong identity foundation and enable traceability; fully apply security and automate best practices; protect data in transit and at rest
- Test procedures to automatically recover from failure; scale horizontally to increase availability of aggregate system; stop guessing capacity and manage change in automation
- Democratize advanced technologies; use serverless architectures; have mechanical sympathy and experiment often
- Adopt consumption model and stop spending money on data center operations; measure overall efficiency, use managed and application-level services to reduce costs
- High availability: when a system can withstand some degradation while still available with minimal downtime
- Reliability: a measure of your system's ability to provide functionality when desired by the user
- Fault tolerance: the ability of an application to remain operational even when a failure occurs
- Scalability: the ability of an application to accommodate increases in capacity without design changes
- AWS Trusted Advisor is an online tool that provides real-time guidence to help provision resources
- AWS Trusted Advisor gives recommendations in cost optimization, performance, security, fault tolerance, and service limits

*Auto Scaling and Monitoring*
- Elastic Load Balancing (ELB) distributes incoming app or network traffic across multiple targets in a single availability zone or across multiple availability zones
- ELB includes application, network, and classic load balancers
- A listener must be configured to expect incoming traffic
- CloudWatch metrics verifies that the system is working as expected and can send alarms using Amazon SNS
- Amazon CloudWatch monitors AWS resources and applications, collects and tracks standard and custom metrics
- Can create alarms based on static threshold, anomaly detection, and metric math expression
- CloudWatch supports basic monitoring (free) and detailed monitoring
- EC2 auto scaling helps you maintain application availability
- Auto scaling group: a group of EC2 instances treated as such for automatic scaling and management
- An Amazon Machine Image (AMI), instance type, and configuration name are required to create an Auto Scaling launch configuration
- Auto scaling responds to changing conditions by adding or terminating instances
