# CIT 114
# AWS Cloud Security
*AWS Shared Responsibility Model*
- The Customer is responsible for security 'in' the cloud
- AWS is responsible for security 'of' the cloud
- AWS responsibilites: Software and Hardware/AWS Global Infrastructure
- Customer responsibilites: Operating system, Applications, Network, and Firewall configuration
- Infrastucture as a Service (IaaS)
- Platform as a Service (PaaS)
- Software as a Service (SaaS)

*AWS IAM*
- IAM is used to manage access to AWS resources
- IAM Essential Components: user, group, policy, and role
- Programmatic access permits AWS CLI, AWS Tools and SDKS
- AWS Management Console access prompts MFA, which requires an authentication code
- Two types of IAM policies: identity-based and resource-based

*Securing a New AWS Account*
- Best practice is to not use the AWS account root except when necessary
- Enable multi-factor authentication (MFA)
- Use AWS CLoudTrail
- Enable a billing report, such as AWS Cost and Usage Report

*Securing Accounts and Data*
- AWS Organizations can be used to manage and secure multiple AWS accounts
- AWS Key Management Service (KMS) can create and manage encryption keys
- AWS Shield is a DDoS protection service
- AWS supports encryption of data at rest (stored physically)
- Encryption of data in transit
