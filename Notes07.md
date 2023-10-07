## CIT 114
# Storage
*AWS EBS*
- Amazon Elastic Block Store (EBS) provide storage volumes for EC2 instances
- Block storage is more faster and uses less bandwidth than object storage, but costs more
- Snapshots can recreate a new volume at any time
- Encryption enrypts volumes at no additional cost
- Elasticity can increase capacity

*AWS S3*
- Amazon Simple Storage Service (S3) stores data as objects in buckets
- Offers virtually unlimited storage
- Wide range of object-level storage classes designed for different scenarios
- Data can be accessed through managment console, command line interface, or SDK
- Pay only for what you use

*AWS EFS*
- Amazon Elastic File Service (EFS) is a file storage for EC2 instances
- Intended for big data and analytics, web serving, media workflows, etc.
- Has elastic capacity and shared storage

*AWS S3 Glacier*
- Glacier is a data archiving service designed for security, durability, and low cost
- Can configure lifecycle archiving of data
- Lifecycle policies can move or delete objects based on age
