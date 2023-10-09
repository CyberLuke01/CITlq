## CIT 114
# Auto Scaling and Monitoring
*Elastic Load Balancing*
- Distributes incoming app or network traffic across multiple targets in a single availability zone or across multiple availability zones
- Scales load balancer as traffic to the application changes
- Offers application, network, and classic load balancer
- A listener must be configured to expect incoming traffic
- Amazon CloudWatch metrics verifies that the system is working as expected and can send alarms using Amazon SNS

*Amazon CloudWatch*
- Monitors AWS resources and applications
- Collects and tracks standard and custom metrics
- Define rules to match changes in AWS environment
- Creates alarms based on static threshold, anomaly detection, and metric math expression

*Amazon EC2 Auto Scaling*
- Auto scaling helps you maintain application availability
- An auto scaling group is a group of EC2 instances treated as such for automatic scaling and management
- AMI, instance type, IAM role, security groups, and EBS volumes are used to configure auto scaling
- Responds to changing conditions by adding or terminating instances
- Launches instances from an AMI
- Enforces a minimum number of running EC2 instances
