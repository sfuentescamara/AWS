# Summary of AWS Cloud Technical Essentials

## Week 1: Getting Started with AWS Cloud 
- Cloud computing
- Differencies between workloads premises/cloud
- Create AWS account
- Differentiate AWS Regions and Availability Zones
- AWS Identity and Acces Management

## Week 2: AWS Compute & Networking
- Difference between AWS servicies
- Elastic Compute Cloud (Amazon EC2) architecture
- Basic networking concepts and the features of Amazon Virtual Private Cloud (Amazon VPC)

## Week 3: Storage & Databases on AWS
- AWS storage services
- How Amazon Elastic Block Store (Amazon EBS) is used
- Databases on AWS, and the use cases for each AWS storage service

## Week 4: Monitoring, Optimizing, and Going Serverless on AWS 
- Monitoring on AWS
- Optimize solutions on AWS
- Function of Elastic Load Balancing (ELB), and how to differentiate between vertical scaling and horizontal scaling

AWS Q&A:
repost.aws

Keywords:
SDKs - Software Development Kits
VPC  - Amazon Virtual Private Cloud
EC2  - Amazon Elastic Compute Cloud
RDS  - Amazon Relational Database Service
CLI  - Amazon Command Line Inteface
S3   - Amazon Simple Storage Service
QA   - Quality assuranse
IAM  - Identity and Access Management
AMI  - Amazon Machine Image

## Week 1: Getting Started with AWS Cloud
### Cloud Computing
Cloud Computing is a service delivery model over the internet, providing on-demand access to IT resources such as servers, storage, databases, networking, software, and more, without the need to manage physical infrastructure.

### Differences Between Workloads on Premises and Cloud
This section discusses key differences between running workloads on-premises and in the cloud. Differences may include scalability, flexibility, and infrastructure management.

### Create AWS Account
Creating an AWS Account involves the process of signing up for Amazon Web Services to gain access to AWS cloud services. An AWS account is essential to start using AWS services. To use an AWS account other than the root account is a fundamental security practice.

### Differentiate AWS Regions and Availability Zones
AWS Regions are geographical locations where AWS has data centers. Availability Zones are isolated data centers within a region, providing redundancy and high availability. 

In summary, your Region and Availability Zone choices should be based on factors such as user proximity, compliance, high availability, cost, and the specific needs of your applications. Selecting the right combination can significantly impact the performance, reliability, and cost-effectiveness of your AWS infrastructure.

### AWS Identity and Access Management (IAM)
IAM (Identity and Access Management) is an AWS service that securely manages access to AWS resources. It allows the creation of users, groups, and policies to control who can access resources and what actions they can perform.

IAM users, groups, and roles are essential components of AWS's access control system. Users are individual entities with their own credentials, groups are collections of users to simplify permissions management, and roles are used to delegate and assume permissions as needed. Effective use of these entities is key to maintaining security and access control in your AWS environment.


## Week 2: AWS Compute & Networking
### Difference between AWS Services
AWS offers a variety of compute services, each designed for specific use cases. Key services include Amazon EC2 (virtual machines), AWS Lambda (serverless), Amazon Elastic Beanstalk (PaaS), and more. Choosing the right service depends on your application's requirements, scalability needs, and management preferences.

### Elastic Compute Cloud (Amazon EC2) Architecture
Amazon EC2 provides scalable, resizable virtual machines (instances) in the cloud. Key points include:
- Instances can run a wide range of operating systems and applications.
- Users can choose instance types based on CPU, memory, storage, and networking requirements.
- EC2 instances can be launched in different Regions and Availability Zones for high availability and redundancy.
- Users can create Amazon Machine Images (AMIs) to capture and replicate instance configurations.

### Basic Networking Concepts and Amazon Virtual Private Cloud (Amazon VPC)
Amazon VPC allows you to create a virtual network within the AWS cloud. Important concepts include:
- Subnets: VPCs can be divided into subnets to control network traffic and isolate resources.
- Security Groups: Act as firewalls for instances, controlling inbound and outbound traffic.
- Network Access Control Lists (NACLs): Work at the subnet level to control traffic.
- Route Tables: Define how traffic is routed between subnets and the internet.
- Internet Gateway: Enables communication between your VPC and the internet.
- VPC Peering: Allows connections between VPCs, providing isolation and resource sharing.
- Virtual Private Network (VPN) Connections: Securely connect your on-premises network to your VPC.
- Elastic IP Addresses: Static, public IP addresses for EC2 instances.


## Week 3: Storage & Databases on AWS
### AWS Storage Services
AWS offers a range of storage services, each designed for specific use cases.
- Amazon S3 (Simple Storage Service) is an object storage service that allows you to store and retrieve data, making it suitable for backup, data archiving, and web applications.
- Amazon EBS (Elastic Block Store) provides block storage volumes for use with Amazon EC2 instances, making it ideal for databases, file systems, and application storage.
- Amazon Glacier is a low-cost archival storage service for data that is rarely accessed but must be retained for compliance or long-term backup.
- AWS Storage Gateway acts as a bridge between on-premises environments and cloud storage.

### How Amazon Elastic Block Store (Amazon EBS) is Used
Amazon EBS offers block-level storage that can be attached to EC2 instances.
- EBS volumes come in different types, such as General Purpose (SSD), Provisioned IOPS (SSD), and Magnetic, each tailored to different performance requirements.
- EBS snapshots allow you to create point-in-time backups of your volumes, facilitating data protection and disaster recovery.

### Databases on AWS and Use Cases for AWS Storage Services
AWS offers a range of managed database services, including Amazon RDS, Amazon DynamoDB, Amazon Aurora, and more.
- Amazon RDS is ideal for managing relational databases, such as MySQL, PostgreSQL, and Oracle.
- Amazon DynamoDB is a fully managed NoSQL database service suitable for high-traffic, web-scale applications.
- Amazon Aurora is a high-performance, MySQL and PostgreSQL-compatible relational database.
The choice of a database and storage service depends on your specific use case, scalability requirements, and data structure.

## Week 4: Monitoring, Optimizing, and Going Serverless on AWS
### Monitoring on AWS
Monitoring is essential for understanding the performance, health, and security of your AWS resources.
Amazon CloudWatch is a monitoring service that provides data and actionable insights for your applications and infrastructure. It collects and stores metrics, monitors logs, and triggers actions based on defined thresholds.

### Optimize Solutions on AWS
Optimization involves making efficient use of resources to reduce costs, improve performance, and enhance scalability.
Techniques for optimization include rightsizing instances, implementing auto-scaling, using Reserved Instances for cost savings, and applying caching strategies.
Regularly reviewing your infrastructure and applications for opportunities to optimize is a best practice.

### Function of Elastic Load Balancing (ELB), and Differentiating Vertical and Horizontal Scaling
Elastic Load Balancing (ELB) is a service that automatically distributes incoming application traffic across multiple Amazon EC2 instances to ensure high availability and fault tolerance.
- Vertical Scaling involves increasing the capacity of an individual instance (e.g., increasing CPU or memory). It is suitable for workloads with varying resource demands.
- Horizontal Scaling involves adding more instances to your application, distributing the load across multiple servers. It is ideal for high availability and managing traffic spikes.


NOTES:
It is possible set up services with CLI (Linea de comandos), Console (API AWS) o SDKs (python/javascript...)


This link shows free services in AWS:
https://aws.amazon.com/es/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=tier%23always-free&awsf.Free%20Tier%20Categories=*all
    - FAQS:
    https://aws.amazon.com/es/free/faqs/

1º Creating billing alert:
https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/DEV-AWS-MO-GCNv2/exercise-1-account.html

2º Creating users ans their permissions
https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/DEV-AWS-MO-GCNv2/exercise-2-iam.html

3º: Launch and Corporate Directory Application on Amazon EC2  
https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/DEV-AWS-MO-GCNv2/exercise-3-compute.html


5ª Creating an S3 Bucket and Modifying the EC2 Instance
https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/DEV-AWS-MO-GCNv2/exercise-5-storage.html


7ª Load Balancing and Auto Scaling
https://aws-tc-largeobjects.s3.us-west-2.amazonaws.com/DEV-AWS-MO-GCNv2/exercise-7-elb.html


## Summary of Instance
 a) EC2: Elastic Computing on Cloud is a service that allows to create a Virtual Machine in AWS.
 b) Fargate: It is a serverless compute engine for containers that allows you to run containers without managing the underlying infrastructure.
 c) Lambda: It is a serverless computing service that lets you run code in response to events without the need to manage servers or infrastructure.


## Choose the Right Storage Service
Here’s a recap of all the storage services mentioned so far. By the end of this reading, you should be able to better answer the question “Which storage service should I use?” for some of the more common scenarios.

### Amazon EC2 Instance Store
Instance store is ephemeral block storage. This is preconfigured storage that exists on the same physical server that hosts the EC2 instance and cannot be detached from Amazon EC2. You can think of it as a built-in drive for your EC2 instance. Instance store is generally well-suited for temporary storage of information that is constantly changing, such as buffers, caches, and scratch data. It is not meant for data that is persistent or long-lasting. If you need persistent long-term block storage that can be detached from Amazon EC2 and provide you more management flexibility, such as increasing volume size or creating snapshots, then you should use Amazon EBS. 

### Amazon EBS
Amazon EBS is meant for data that changes frequently and needs to persist through instance stops, terminations, or hardware failures. Amazon EBS has two different types of volumes: SSD-backed volumes and HDD-backed volumes.

Here are a few important features of Amazon EBS that you need to know when comparing it to other services. 
- It is block storage.
- You pay for what you provision (you have to provision storage in advance).
- EBS volumes are replicated across multiple servers in a single Availability Zone.
- Most EBS volumes can only be attached to a single EC2 instance at a time.

### Amazon S3
If your data doesn’t change that often, Amazon S3 might be a more cost-effective and scalable storage solution. S3 is ideal for storing static web content and media, backups and archiving, data for analytics, and can even be used to host entire static websites with custom domain names.Here are a few important features of Amazon S3 to know about when comparing it to other services. 

- It is object storage.
- You pay for what you use (you don’t have to provision storage in advance).
- Amazon S3 replicates your objects across multiple Availability Zones in a Region.
- Amazon S3 is not storage attached to compute.

### Amazon Elastic File System (Amazon EFS) and Amazon FSx
For file storage that can mount on to multiple EC2 instances, you can use Amazon Elastic File System (Amazon EFS) or Amazon FSx. Use the following table for more information about each of these services. 

Amazon Elastic File System (EFS)
- Fully managed NFS file system.

Amazon FSx for Windows File Server
- Fully managed file server built on Windows Server that supports the SMB protocol.

Amazon FSx for Lustre
- Fully managed Lustre file system that integrates with S3.

Here are a few important features of Amazon EFS and FSx to know about when comparing them to other services. 
- It is file storage.
- You pay for what you use (you don’t have to provision storage in advance).
- Amazon EFS and Amazon FSx can be mounted onto multiple EC2 instances.
