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
- Each region has multiple availability zones
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
- Private subnets do not have direct access to the internet
- MAXIMUM subnet range is /16, MINIMUM subnet range is /28
- Elastic network interface can be attached/detached to an instance
- Only one IGW can be used with a VPC at one time
- Two types of endpoints: Gateway and Interface
- Route 53 is a scalable Domain Name System (DNS) web service, that is used to route users to web applications
- Route 53 supports different kinds of routing, including Simple, Weighted, Latency, etc.
- CloudFront is a fast, global, and secure CDN service, and self-service model that consists of edge locations and regional edge cache
