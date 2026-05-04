# AWS Solutions Architect Associate Revision Sheet

## Official Principles and Core Ideas

### Domain 1: Design Secure Architectures (30%)

#### Task Statement 1.1: Design secure access to AWS resources

- Use AWS IAM for identity and access management
- Implement least privilege principle
- Use multi-factor authentication (MFA)
- Roles for EC2, Lambda, etc.
- AWS IAM Identity Center for workforce access

#### Task Statement 1.2: Design secure workloads and applications

- Use security groups and NACLs
- Encrypt data at rest and in transit
- Use AWS WAF, Shield for protection
- Implement logging and monitoring with CloudTrail, CloudWatch
- GuardDuty for threat detection

#### Task Statement 1.3: Determine appropriate data security controls

- Use KMS for key management
- S3 bucket policies, versioning
- RDS encryption
- Data classification and compliance
- Macie for data discovery

### Domain 2: Design Resilient Architectures (26%)

#### Task Statement 2.1: Design scalable and loosely coupled architectures

- Use Auto Scaling groups
- Decouple with SQS, SNS
- Use Lambda for serverless
- Microservices with ECS/EKS
- EventBridge for event-driven architectures

#### Task Statement 2.2: Design highly available and/or fault-tolerant architectures

- Multi-AZ deployments
- Use ELB for load balancing
- Backup and recovery with AWS Backup
- Route 53 for DNS failover
- CloudFormation for infrastructure resilience

#### Task Statement 2.3: Design decoupling mechanisms using AWS services

- SQS for message queuing
- SNS for pub/sub
- EventBridge for event routing
- Step Functions for workflows

#### Task Statement 2.4: Choose appropriate resilient storage

- S3 for durability (99.999999999%)
- EBS snapshots
- RDS multi-AZ
- Glacier for archive
- DynamoDB global tables

### Domain 3: Design High-Performing Architectures (24%)

#### Task Statement 3.1: Identify elastic and scalable compute solutions for a workload

- EC2 Auto Scaling
- Lambda for event-driven
- ECS/EKS for containers
- Batch for large jobs
- Fargate for serverless containers

#### Task Statement 3.2: Select high-performing and scalable storage solutions for a workload

- S3 for object storage
- EBS for block storage (gp3, io2)
- EFS for file storage
- FSx for specialized (Windows, Lustre)
- Storage Gateway for hybrid

#### Task Statement 3.3: Select high-performing networking solutions for a workload

- VPC with subnets
- Direct Connect for low latency
- CloudFront for CDN
- Global Accelerator
- Transit Gateway

#### Task Statement 3.4: Choose high-performing database solutions for a workload

- RDS for relational (Aurora for performance)
- DynamoDB for NoSQL
- Aurora for high performance
- ElastiCache for caching (Redis, Memcached)
- Redshift for analytics

### Domain 4: Design Cost-Optimized Architectures (10%)

#### Task Statement 4.1: Identify cost-effective storage solutions

- S3 storage classes (Standard, IA, Glacier)
- Lifecycle policies
- EBS types (gp2 vs gp3)
- S3 Intelligent-Tiering

#### Task Statement 4.2: Identify cost-effective compute and database services

- Reserved Instances, Savings Plans
- Spot Instances
- Right-sizing with Compute Optimizer
- Serverless options (Lambda, Fargate)

#### Task Statement 4.3: Design cost-optimized network architectures

- Use CloudFront
- Optimize data transfer costs
- VPC endpoints for private access
- Use Savings Plans for data transfer

### Domain 5: Design Solutions for Organizational Complexity (10%)

#### Task Statement 5.1: Determine cross-account authentication and access strategy

- AWS Organizations
- IAM roles for cross-account
- Resource Access Manager (RAM)
- Control Tower for governance

#### Task Statement 5.2: Evaluate automation and deployment strategies

- CloudFormation for IaC
- CodePipeline for CI/CD
- Systems Manager for automation
- Elastic Beanstalk for PaaS

#### Task Statement 5.3: Evaluate migration strategies

- AWS Migration Hub
- Application Migration Service (MGN)
- Database Migration Service (DMS)
- Snowball for large transfers

#### Task Statement 5.4: Evaluate hybrid IT architectures

- Direct Connect
- VPN (Site-to-Site, Client VPN)
- Storage Gateway
- Outposts for on-premises AWS

## Official Technologies and Concepts

### Architecture and Build

- APIs: programmatic interfaces for AWS operations.
- Infrastructure as code (IaC): define infrastructure with CloudFormation, CDK.
- AWS SDKs: developer libraries for AWS services.
- AWS Well-Architected Framework: best-practice design guidance.
- Compute: EC2, Lambda, containers.
- Databases: RDS, DynamoDB, Aurora.
- Storage: S3, EBS, EFS.
- Network services: VPC, Route 53, CloudFront.

### Security and Cost

- Security: protect identities, data, and workloads.
- AWS shared responsibility model: AWS secures the cloud; customers secure in the cloud.
- AWS Compliance: compliance programs and audit resources.
- Cost management: monitor and optimize cloud spending.
- AWS Pricing Calculator: estimate cost before deployment.

### Support and Guidance

- AWS Knowledge Center: official troubleshooting articles.
- AWS Prescriptive Guidance: strategies, patterns, and implementation guidance.
- AWS re:Post: community and AWS knowledge Q&A.
- AWS Support Center: place to manage support cases.
- AWS Support plans: Developer, Business, Enterprise On-Ramp, Enterprise.
- AWS Partner Network (APN): AWS partner ecosystem.
- AWS Professional Services: AWS expert delivery support.
- AWS solutions architects: AWS design and architecture guidance.

## Exam Topics and Common Question Patterns

### High-Frequency Topics

- Shared responsibility model
- IAM, MFA, root user
- Regions, Availability Zones, Edge Locations
- High availability with Multi-AZ, Auto Scaling, ELB
- Storage: S3, EBS, EFS
- Databases: RDS, DynamoDB
- Networking: VPC, subnets, security groups, NACLs
- Cost optimization: Reserved, Spot, Savings Plans
- Security: encryption, KMS, CloudTrail

### Common Question Patterns

- Best service for a use case
- Service comparisons
- Architecture design scenarios
- Cost optimization
- Security best practices

## Official In-Scope AWS Services

(List of services similar to Cloud Practitioner, but focused on SAA core services)

- Compute: EC2, Lambda, Auto Scaling, Batch, Lightsail, Outposts
- Containers: ECS, EKS, ECR, Fargate
- Storage: S3, EBS, EFS, FSx, Glacier, Storage Gateway, Backup
- Database: RDS, Aurora, DynamoDB, ElastiCache, Neptune, DocumentDB
- Networking: VPC, CloudFront, Route 53, API Gateway, Direct Connect, Global Accelerator, Transit Gateway
- Security: IAM, KMS, CloudHSM, GuardDuty, Inspector, Macie, Shield, WAF, Artifact, Cognito
- Management: CloudWatch, CloudTrail, Config, Systems Manager, Trusted Advisor, Organizations, Control Tower
- Analytics: Athena, Kinesis, Glue, Redshift, QuickSight
- Application Integration: SQS, SNS, EventBridge, Step Functions
- Migration: DMS, Migration Hub, Snow Family
- Developer Tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline, CloudFormation
- IoT: IoT Core
- ML: SageMaker, Comprehend, Rekognition
- End User Computing: WorkSpaces, AppStream 2.0
- Business Applications: Connect
- Cost Management: Budgets, Cost Explorer

## Official AWS Sources

- SAA-C03 exam guide
- Content domains
- Technologies and concepts
- In-scope services