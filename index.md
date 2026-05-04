# AWS SAA-C03 Revision Sheet

Fast revision notes for AWS Certified Solutions Architect - Associate. This sheet follows the official AWS exam guide and focuses on the scenario patterns that appear in architecture questions.

## Exam Facts

- Exam code: SAA-C03
- Scored questions: 50
- Unscored questions: 15
- Passing score: 720/1000
- Target candidate: at least 1 year of hands-on experience designing AWS cloud solutions

## Content Domains

### Domain 1: Design Secure Architectures - 30%

#### 1.1 Design secure access to AWS resources

- Know IAM users, groups, roles, policies, resource policies, STS, federation, and IAM Identity Center.
- Apply least privilege, MFA, root user protection, cross-account roles, SCPs, and Control Tower patterns.
- Choose account and authorization boundaries for multi-account environments.

#### 1.2 Design secure workloads and applications

- Design secure VPCs with public and private subnets, route tables, security groups, network ACLs, NAT gateways, and endpoints.
- Protect applications with Shield, WAF, Secrets Manager, Cognito, GuardDuty, Macie, and secure hybrid connectivity.
- Recognize DDoS, SQL injection, exposed credentials, and overly open network paths.

#### 1.3 Determine appropriate data security controls

- Use KMS, CloudHSM, ACM, TLS, key policies, rotation, and certificate renewal appropriately.
- Apply data classification, retention, lifecycle, backup, replication, and access policies.
- Match encryption and compliance controls to the workload requirements.

### Domain 2: Design Resilient Architectures - 26%

#### 2.1 Design scalable and loosely coupled architectures

- Use SQS, SNS, EventBridge, Step Functions, API Gateway, Lambda, Fargate, ECS, and EKS to decouple components.
- Know horizontal vs vertical scaling, caching, read replicas, stateless services, and multi-tier design.
- Pick purpose-built services instead of forcing every workload onto EC2.

#### 2.2 Design highly available and fault-tolerant architectures

- Design across Availability Zones and Regions with ELB, Route 53, Auto Scaling, backups, and replication.
- Choose DR strategies: backup and restore, pilot light, warm standby, or active-active based on RPO and RTO.
- Mitigate single points of failure and track the right health and business metrics.

### Domain 3: Design High-Performing Architectures - 24%

#### 3.1 Determine high-performing and/or scalable storage solutions

- Compare object, block, and file storage: S3, EBS, EFS, FSx, Storage Gateway, and DataSync.
- Match IOPS, throughput, latency, access pattern, and future growth to the storage service and configuration.

#### 3.2 Design high-performing and elastic compute solutions

- Choose EC2 instance families, Auto Scaling, Lambda memory, Fargate, ECS, EKS, Batch, and EMR for the workload.
- Scale independent components using metrics, queues, and event-driven designs.

#### 3.3 Determine high-performing database solutions

- Compare RDS, Aurora, DynamoDB, ElastiCache, DocumentDB, Neptune, Keyspaces, and Redshift.
- Design for read/write access patterns, capacity planning, read replicas, proxies, serverless options, and caching.

#### 3.4 Determine high-performing and/or scalable network architectures

- Use VPC subnet tiers, routing, IP addressing, ELB types, PrivateLink, VPN, Direct Connect, CloudFront, and Global Accelerator.
- Place resources to meet latency, throughput, hybrid, global, and multi-tier requirements.

#### 3.5 Determine high-performing data ingestion and transformation solutions

- Use Kinesis, Data Firehose, MSK, Glue, EMR, Athena, Lake Formation, Redshift, and QuickSuite for analytics paths.
- Design secure ingestion, transformation, data lakes, streaming, and visualization flows.

### Domain 4: Design Cost-Optimized Architectures - 20%

#### 4.1 Design cost-optimized storage solutions

- Use lifecycle rules, S3 storage classes, Requester Pays, archive options, right-sized EBS, and backup strategies.
- Choose migration and hybrid transfer services by size, frequency, urgency, and network cost.

#### 4.2 Design cost-optimized compute solutions

- Compare On-Demand, Reserved Instances, Spot Instances, Savings Plans, serverless, containers, and EC2 hibernation.
- Right-size instance families, production vs non-production capacity, and scaling policies.

#### 4.3 Design cost-optimized database solutions

- Choose RDS, Aurora, DynamoDB, Redshift, and serverless database options based on access pattern and retention.
- Tune backups, snapshots, read replicas, caching, capacity mode, and migrations for cost.

#### 4.4 Design cost-optimized network architectures

- Watch NAT gateway placement, AZ-to-AZ traffic, Region-to-Region traffic, VPC endpoints, CDN caching, VPN, and Direct Connect.
- Pick load balancers and throttling strategies that match the actual traffic pattern.

## High-Value Question Patterns

- Loose coupling: SQS, SNS, EventBridge, Step Functions.
- High availability: Multi-AZ, ELB, Route 53, Auto Scaling, backups, replication.
- Global speed: CloudFront for caching, Global Accelerator for optimized global routing, Route 53 for DNS routing policies.
- Private access: VPC endpoints, PrivateLink, gateway endpoints, resource policies.
- Database scale: Aurora replicas, DynamoDB, ElastiCache, RDS Proxy.
- Lower cost: Savings Plans, Spot Instances, lifecycle policies, right-sizing, Cost Explorer.

## In-Scope AWS Service Categories

- Analytics: Athena, Data Exchange, Data Firehose, EMR, Glue, Kinesis, Lake Formation, MSK, OpenSearch Service, QuickSuite, Redshift.
- Application Integration: AppFlow, AppSync, EventBridge, MQ, SNS, SQS, Step Functions.
- AWS Cost Management: Budgets, Cost and Usage Report, Cost Explorer, Savings Plans.
- Compute: Batch, EC2, EC2 Auto Scaling, Elastic Beanstalk, Outposts, Serverless Application Repository, VMware Cloud on AWS, Wavelength.
- Containers: ECR, ECS, ECS Anywhere, EKS, EKS Anywhere, EKS Distro.
- Database: Aurora, Aurora Serverless, DocumentDB, DynamoDB, ElastiCache, Keyspaces, Neptune, RDS, Redshift.
- Developer Tools: X-Ray.
- Front-End Web and Mobile: Amplify, API Gateway, Device Farm.
- Machine Learning: Comprehend, Kendra, Lex, Polly, Rekognition, SageMaker AI, Textract, Transcribe, Translate.
- Management and Governance: Auto Scaling, CLI, CloudFormation, CloudTrail, CloudWatch, Compute Optimizer, Config, Control Tower, Health Dashboard, License Manager, Managed Grafana, Managed Service for Prometheus, Management Console, Organizations, Service Catalog, Systems Manager, Trusted Advisor, Well-Architected Tool.
- Media Services: Elastic Transcoder, Kinesis Video Streams.
- Migration and Transfer: Application Migration Service, DataSync, DMS, Snow Family, Transfer Family.
- Networking and Content Delivery: Client VPN, CloudFront, Direct Connect, ELB, Global Accelerator, PrivateLink, Route 53, Site-to-Site VPN, Transit Gateway, VPC.
- Security, Identity, and Compliance: Artifact, Audit Manager, ACM, CloudHSM, Cognito, Detective, Directory Service, Firewall Manager, GuardDuty, IAM Identity Center, Inspector, KMS, Macie, Network Firewall, RAM, Secrets Manager, Security Hub, Shield, WAF, IAM.
- Serverless: AppSync, Fargate, Lambda.
- Storage: Backup, EBS, EFS, FSx for all types, S3, S3 Glacier, Storage Gateway.

## Final Review Checklist

- IAM roles vs users vs resource policies vs SCPs.
- Security groups vs network ACLs vs AWS Network Firewall.
- Public subnet, private subnet, NAT gateway, internet gateway, route table.
- S3 storage classes, lifecycle policies, replication, encryption, and access policies.
- EBS vs EFS vs FSx vs S3 vs Storage Gateway.
- RDS Multi-AZ vs read replicas vs Aurora replicas vs DynamoDB global tables.
- SQS vs SNS vs EventBridge vs Step Functions.
- ALB vs NLB vs Gateway Load Balancer.
- CloudFront vs Global Accelerator vs Route 53 routing policies.
- Direct Connect vs Site-to-Site VPN vs Client VPN vs PrivateLink.
- Backup and restore vs pilot light vs warm standby vs active-active.
- On-Demand vs Reserved Instances vs Savings Plans vs Spot Instances.
- Cost Explorer, Budgets, Cost and Usage Report, tags, and multi-account billing.
- CloudWatch vs CloudTrail vs Config vs X-Ray.
- Well-Architected pillars and tradeoffs.

## Official AWS Sources

- [AWS Certified Solutions Architect - Associate SAA-C03 exam guide](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03.html)
- [Content Domain 1: Design Secure Architectures](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain1.html)
- [Content Domain 2: Design Resilient Architectures](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain2.html)
- [Content Domain 3: Design High-Performing Architectures](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain3.html)
- [Content Domain 4: Design Cost-Optimized Architectures](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain4.html)
- [Technologies and Concepts](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/saa-technologies-concepts.html)
- [In-Scope AWS Services](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/saa-03-in-scope-services.html)
