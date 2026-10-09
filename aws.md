## TABLE OF CONTENTS

1. [INTRODUCTION](#introduction)

2. [TERMINOLOGIES](#terminologies)

3. [SCHEME/GUIDELINE](#schemeguideline)

4. [REFERENCES](#references)

<br>
<br>
<br>
<br>

## INTRODUCTION

<br>

- Amazon Web Services (AWS) is a Comprehensive Cloud Platform used for various Software development needs.
- Cloud Computing is the on-demand delivery of IT resources via the internet.
- AWS services follows a Pay-as-you-use subscription/usage logic.

- EC2 is the AWS service that allows you to create virtual servers, which Amazon calls instances.
- Instance Type: How much CPU and memory our virtual server will have.
- Tags let you add a Label to the resources you are creating (key-value pair).
- Websites can be coded to automatically upload all its images to the S3 Storage Bucket when it first starts running.
- dnf (Dandified YUM): the default software package management tool on Amazon Linux virtual machines.
- Different regions can have different pricing.
- Generally, the regions in the US and Europe are the most affordable, other than US-West 1.
- Bes sure to set a spending limit on your account (AWS Budget).

<br>

### Services/Billing

- Multiple Data centers form an Availability Zone
- Not all AWS services are available in every region
- Every service has a different pricing
- Deployment/Hosting region considerations
  - Proximity to users
  - Availability of service(s)
  - Cost (U.S East is usally the cheapest)
  - Compliance and Legal requirements
- You can enable locked regions in your acount
- You can create/customise your dashboard
- If you are commiting to AWS (say I will use an EC2 instance for 3 years...), you get a discount.
- Recommend setting a Zero-spend budget or Monthly cost budget on every AWS account

<br>

### Cloud Computing

- Three main Categories/Services
  - SaaS: Software as a Service e.g. Gmail
  - PaaS: Platform as a Service e.g Heroku
  - IaaS: Infrastructure as a Service e.g Amazon EC2, Microsoft Azure
- Whenever you are creating any sort of resource within AWS, make sure you remember to delete that resource once you are done practising.

<br>

### IAM - Identity and Access Management

- IAM Users: Represents an individual person.
- IAM Groups: A Collection of users with shared permissions.
- IAM Roles:
  - Temporary identities assumed by users, apps or AWS services.
  - No permamnent credentials (keys are short-lived).
  - Best practice for EC2, Lambda, EKS, CI/CD.
- IAM Policies: JSON documents defining permissions.
- AWS managed: Policies created and managed by AWS.
- Bucket names must be unique Globally just like web signup usernames; though options are now available for regional uniqueness.
- Best Practices
  - Never use the root account
  - Setup IAM Users/Groups
  - MFA Everywhere
  - Follow Principle of Least Privilege

<br>

### Certifications

AWS IT Certifications are grouped across 4 levels

- Foundational:
  - Cloud Practitioner
  - AI Practitioner

- Associate
  - Solutions Architect
  - Machine Learning Engineer
  - Developer
  - Data Engineer
  - CloudOps Engineer

- Professional
  - Generative AI Developer
  - Solutions Architect (SAP-CO2)
  - Devops Engineer (DOP-CO2)

- Specialty
  - Advanced Networking
  - Security

#### Cost

- Foundational - $100
- Associate - $150
- Professional and Specialty - $300

NB: Every Exam after the first one becomes 50%

<br>

### EC2 = Elastic Compute Cloud

- **EC2** is an AWS service for renting virtual servers in the cloud.
- Instance is a running virtual server.
- AMI: Amazon machine image: Prebuilt OS along with software template that you can pick when lauching an instance.
- EBS (Elastic Block Store): full system block storage that you can attach to an instance.
- A key pair consisting of a public and a private key, is a set of security credentials that you use to prove your identity when connecting to an Amazon EC2 instance.
- When you install Ubuntu, you get one default user - `ubuntu`.

<br>

### Storage on AWS

Three Categories:

- **Object Storage** - S3 (Simple Storage Service)
  - Bucket is like a container at the root level of S3. Every file you store in S3 must go into a bucket.
  - You can use S3 buckets to host static websites.
  - Bucket versioning is a way S3 bucket keeps multiple versions of an object in the same bucket.
- **Block Storage** - EBS, RDS
- **File Storage** - EFS

### IP Addresses in AWS

- **Private IP:** Allocated to every instance created. Used for communication within AWS only.
- **Public IP:** Accessible in the internet.
- **Elastic IP:** Static, won't change even if you restart the instance.

### VPC - Virtual Private Cloud
- A Form of a Seperation of networks with each having it's own instances, services etc within the same user account. 
- Subnets: Grouping/segmentation inside a VPC
  - Private Subnet: Can't communicate in the internet (within)
  - Public Subnet: Instances can communicate with the internet
- Range of Public IP (Optional) and Private IPs are assigned to VPCs
- Route Tables


<br>
<br>
<br>
<br>

## SCHEME/GUIDELINE

<br>

This scheme uses SAP-CO2 as the scope for the learning pathway

<br>

### Content Domains

1. Design Solutions for Organizational Complexity
   - Architect Network Connectivity Strategies
   - Prescribe Security Controls
   - Design reliable and resilient architectures
   - Design a multi-account AWS environment
   - Determine Cost Optimization and visibility strategies

2. Design for new Solutions
   - Design a deployment strategy to meet business requirements
   - Design a solution to ensure business continuity
   - Determine security controls based on requirements
   - Design a strategy to meet reliability requirements
   - Design a solution to meet performance objectives
   - Determine a cost optimization strategy to meet solution goals and objectives

3. Continous Improvement for Existing Solutions
   - Determine a Strategy to improve overall operational excellence
   - Determine a strategy to improve security
   - Determine a strategy to improve performance
   - Determine a strategy to improve reliability
   - Identify opportunities for cost optimizations.

4. Accelerate Workload Migration and Modernization
   - Select existing workloads and processes for potential migration
   - Determine the optimal migration approach for existing workloads
   - Determine a new architecture for existing workloads
   - Determine opportunities for modernization and enhancements

<br>

### AWS Services, Technologies and Concepts

1. Technologies and Concepts
   - Compute
   - Cost Management
   - Database
   - Disaster recovery
   - High availability
   - Management and governance
   - Microservices and component decoupling
   - Migration and data transfer
   - Network, connectivity and content delivery
   - Security
   - Serverless design principles
   - Storage

2. In-scope AWS Services
   - Analytics
   - Application Integration
   - Blockchain
   - Business Applications
   - Cloud Financial Management
   - Compute
   - Containers
   - Database
   - Developer tools
   - End User Computing
   - Frontend Web and Mobile
   - Internet of Things (IoT)
   - Machine Learning
   - Media Services
   - Management and Governance
   - Migration and Transfer
   - Network and Content Delivery
   - Security, Identity and Compliance
   - Storage

<br>
<br>
<br>
<br>

## TERMINOLOGIES

<br>

- Amazon EC2 (Elastic Compute Cloud): Virtual Server that AWS has
- Availability Zones (AZs) - Backup
- Bucket Policy
- Hardening means making an account, system or an application more secure by reducing it's weakness.
- Load balancer
- Region: Group of availability zones in a given geographic area
- RDS Databases
- S3 Storage: Good Place to store files

<br>
<br>
<br>
<br>

## REFERENCES

<br>

- [AWS Tutorial for Beginners – Step-by-Step Guide to Cloud Computing](https://youtu.be/Nzv-tzU-UAw?si=S3CuwCBDSIU_xvy9)
- [Getting Started with AWS (Playlist)](https://www.youtube.com/watch?v=a9__D53WsUs&list=PLhr1KZpdzukf4p57gUnTyToXYJxGAPx03)
- [The BEST AWS Certification Roadmap 2026 (Updated + AI)](https://youtu.be/fQn24oajC0U?si=wjantJq0UxoJan_Z)
- [AWS Certification](https://aws.amazon.com/certification/)
- [AWS Certification Paths](https://d1.awsstatic.com/onedam/marketing-channels/website/aws/en_US/certification/approved/pdfs/AWS_certification_paths.pdf)
- [Solutions Architect Pro vs DevOps Pro: Which AWS Certification Should You Take?](https://www.jeeviacademy.com/solutions-architect-pro-vs-devops-pro-which-aws-certification-should-you-take/)
- [SA Pro vs DevOps Pro - Which is of more value?](https://www.reddit.com/r/AWSCertifications/comments/nejicb/sa_pro_vs_devops_pro_which_is_of_more_value/)
- [Exam Guide (DOP-C02)](https://docs.aws.amazon.com/pdfs/aws-certification/latest/devops-engineer-professional-02/devops-engineer-professional-02.pdf)
- [Exam Guide (SAP-C02)](https://docs.aws.amazon.com/pdfs/aws-certification/latest/solutions-architect-professional-02/solutions-architect-professional-02.pdf)
- [AWS Tutorial Course for Beginners, Developers, DevOps Engineers | Hands-On | AWS Cloud Computing](https://youtu.be/2OHr0QnEkg4?si=tTqoQ-R3YRPEkM1e)
- [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)
