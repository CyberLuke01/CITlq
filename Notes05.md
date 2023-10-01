# CIT 114
## Networking and Content Delivery
*Networking Basics*
- Networks consist of a router and subnets
- IP, IPv4 and IPv6 addresses
- CIDR consists of network identifer (routing prefix) and host identifier

*Amazon VPC*
- Amazon VPC can provision a logically isolated section of the AWS Cloud
- Gives you control over network resources
- Subnets are ranges of IP addresses that divide a VPC
- Largest IPv4 CIDR block size is /16
- Smallest IPv4 CIDR block size is /28
- Public IPv4 address and Elastic IP address
- Elastic network interface can be attached/detached to an instance
- Route table contains configurable rules

*VPC Networking and Security*
- Two types of endpoints: Gateway and Interface
- Security groups act at the instance level
- Security groups have rules and are stateful
- Network ACLs act at the subnet level
- A network ACL has separate inbound and outbound rules and are stateless

*Route 53*
- Route 53 is a scalable Domain Name System (DNS) web service
- Used to route users to internet applications
- Supports different kinds of routing, including Simple, Weighted, Latency, etc.

*CloudFront*
- CloudFront is a fast, global, and secure CDN service
- Self-service model
- Has edge locations and regional edge cache
