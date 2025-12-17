# AWS Cloud Practitioner Notes - Domain 3: Cloud Technology and Services

## Domain 3 Overview

### What Domain 3 Covers:
- AWS services and technology
- Types of AWS services
- Infrastructure
- Operational aspects of using AWS Cloud

### Building on Previous Knowledge:
- Domain 1: Cloud Concepts (already covered)
- Domain 2: Security and Compliance (already covered)
- Domain 3: Deeper dive into AWS services and technology

---

## Domain 3 Task Statements

### Eight Task Statements:

**Task Statement 3.1:** Define methods of deploying and operating in the AWS Cloud

**Task Statement 3.2:** Define the AWS global infrastructure

**Task Statement 3.3:** Identify AWS compute services

**Task Statement 3.4:** Identify AWS database services

**Task Statement 3.5:** Identify AWS network services

**Task Statement 3.6:** Identify AWS storage services

**Task Statement 3.7:** Identify AWS artificial intelligence and machine learning services and analytics services

**Task Statement 3.8:** Identify services from other in-scope AWS service categories

---

## What Each Task Statement Covers

### Task Statement 3.1: Methods of Deploying and Operating in AWS

**Focus:**
- Types of deployment models
- Connectivity options

### Task Statement 3.2: AWS Global Infrastructure

**Focus:**
- Dive deeper into AWS global infrastructure
- Components that make up global infrastructure:
  - Availability Zones
  - Regions
  - Edge locations

### Task Statements 3.3 - 3.8: AWS Core Services

**Coverage:**
- All about AWS core services
- Categories of core services
- Examples of each category

---

## Four Categories of Core AWS Services

### Primary Categories:

**1. Compute**

**2. Storage**

**3. Networking**

**4. Database**

### Additional Service Categories Covered:
- Artificial Intelligence (AI)
- Machine Learning (ML)
- Analytics
- Few other AWS services in scope for exam

---

## Three Key Areas of Understanding

### 1. Service Categorization

**What You Need to Know:**
- How various AWS services fit into different categories (compute, storage, networking, database, etc.)
- What makes a service compute versus database?
- What does categorization say about the services?
- Is there any overlap you should be aware of?

### 2. Service Selection

**When to Choose What:**
- Why would you choose one category and service over another?
- Example question: When would you choose database service over running database on Amazon EC2 instance?
- Understanding use cases and trade-offs

### 3. Subcategories Within Categories

**Understanding Depth:**
- Pay attention to subcategories that exist within each larger category
- Each main category has multiple subcategories
- Understand the nuances and specializations

**Note:** Will cover all of this in upcoming lessons

---

## Course Structure for Domain 3

### Approach:
- Each task statement addressed individually
- Breaking down knowledge and skills expected for success
- Progressive learning through categories and services

---

## Study Strategy for Domain 3

### Key Questions to Ask Yourself:

**For Each Service:**
1. What category does this service belong to?
2. What makes it part of that category?
3. When would I use this service?
4. What are the alternatives?
5. What subcategory does it fall into?

**Service Comparison:**
1. What's the difference between similar services?
2. When would I choose one over another?
3. Are there any overlaps between categories?
4. What are the trade-offs?

---

## Important Exam Considerations

### What You Must Know:

**1. Service Categories:**
- Understand the four primary categories
- Know additional categories (AI, ML, Analytics, etc.)
- Recognize how services fit into categories

**2. Service Selection:**
- Know when to use which service
- Understand use cases
- Recognize trade-offs

**3. Service Characteristics:**
- What defines a compute service?
- What defines a database service?
- What defines a storage service?
- What defines a networking service?

**4. Subcategories:**
- Within compute: different types of compute services
- Within storage: different types of storage services
- Within database: different types of database services
- Within networking: different types of networking services

---

## Learning Objectives

### By End of Domain 3, You Should Be Able To:

**1. Deployment and Operations:**
- Understand deployment models
- Know connectivity options

**2. Global Infrastructure:**
- Explain AWS global infrastructure
- Understand Regions, Availability Zones, Edge Locations

**3. Service Identification:**
- Identify compute services and their uses
- Identify database services and their uses
- Identify network services and their uses
- Identify storage services and their uses
- Identify AI/ML services and their uses
- Identify analytics services and their uses
- Identify other in-scope services

**4. Service Selection:**
- Choose appropriate service for given scenario
- Understand when to use managed vs. unmanaged services
- Know trade-offs between different service options

---

## Domain 3 Structure Overview

### Task Statement Breakdown:

**Foundation (Task Statements 3.1-3.2):**
- Deployment and operations (3.1)
- Global infrastructure (3.2)

**Core Services (Task Statements 3.3-3.6):**
- Compute services (3.3)
- Database services (3.4)
- Network services (3.5)
- Storage services (3.6)

**Advanced Services (Task Statements 3.7-3.8):**
- AI/ML and Analytics services (3.7)
- Other in-scope services (3.8)

---

## Preparation Tips

### Study Approach:

**1. Start with Categories:**
- Understand what defines each category
- Learn the primary characteristics

**2. Learn Services:**
- Study services within each category
- Understand their specific use cases

**3. Compare and Contrast:**
- Compare services within same category
- Compare services across categories
- Understand overlaps and differences

**4. Practice Scenarios:**
- Work through use case scenarios
- Practice selecting appropriate services
- Understand why one service over another

---

## Key Concepts to Master

### Service Understanding:
- What each service does
- When to use each service
- How services relate to each other

### Category Knowledge:
- Four main categories (Compute, Storage, Networking, Database)
- Additional categories (AI, ML, Analytics, Others)
- Subcategories within main categories

### Decision Making:
- How to choose between services
- When managed services are appropriate
- When unmanaged services are appropriate
- Trade-offs in service selection

---
## Notes for Success

**Remember:**
- Domain 3 is about AWS services and technology
- Builds on concepts from Domains 1 and 2
- Focus on understanding, not memorization
- Know use cases and when to apply services
- Understand relationships between services
- Pay attention to subcategories and specializations

**Exam Strategy:**
- Know service categories
- Understand when to use each service
- Recognize trade-offs
- Identify appropriate services for scenarios
- Understand AWS global infrastructure components


# AWS Cloud Practitioner Notes - Task Statement 3.1: Define Methods of Deploying and Operating in AWS

## Methods of Communicating with AWS

### Four Main Methods Available:

**1. Programmatic Access to APIs**
- Through Software Development Kits (SDKs)

**2. API Access Through AWS Command Line Interface (CLI)**

**3. Graphical Interface**
- Through AWS Management Console

**4. Infrastructure as Code**
- Various infrastructure as code offerings
- Example: AWS CloudFormation

---

## Understanding Methods - Beyond Just Knowing They Exist

### What You Must Know:

**Not Just What Methods Exist:**
- More important to know HOW and WHEN to use them

**Strengths and Limitations:**
- Should be aware of strengths and limitations of each method

**When to Use What:**
- Think about when to use Management Console over SDKs
- Think about when to use CLI versus CloudFormation

**Example Question:**
- What benefits do you see in accessing Amazon S3 in console vs. running commands in CLI?

---

## Cloud Deployment Models

### Four Types of Deployment Models:

**1. Public Cloud**
**2. Private Cloud**
**3. Hybrid Cloud**
**4. Multi-Cloud**

### Important Understanding:

**More Than Definitions:**
- Not only important to know how to define different deployment types
- Must be aware of how they look in action

**Questions to Ask Yourself:**
- Would applications working together between local data center and AWS be considered on-premises or hybrid deployment?
- Why would you choose to keep certain resources on-premises instead of moving everything to AWS?
- What are considerations needed when utilizing various types of deployment?

---

## Public Cloud

### Definition:
- Cloud environment available to the public
- Meets cloud criteria discussed in earlier cloud computing lesson

### Examples:
- AWS offers public cloud platform
- Azure offers public cloud platform
- Google offers public cloud platform

---

## Multi-Cloud

### Definition:
- Still public cloud
- Using MORE than one public cloud

### Examples:
- Using AWS and Azure
- Using AWS and Google
- Using all three (AWS, Azure, Google)

### Consideration:
- Sounds really cool
- Can be difficult to design and build

---

## Private Cloud

### Characteristics:

**1. Dedicated Services:**
- For your environment
- Services are on-premises

**2. Directly Dedicated:**
- Dedicated directly to your environment

**3. Cloud Vendors:**
- Each cloud vendor has private cloud service
- Example: AWS Outposts

### Main Difference from Other On-Premises Services:

**Private Cloud Requirements:**
- Must meet cloud computing criteria (discussed earlier)
- Must be directly dedicated to your business

**Other On-Premises Services:**
- May not meet all cloud computing criteria

---

## Hybrid Cloud vs. Hybrid Environment

### CRITICAL DISTINCTION - Easy to Confuse:

**Hybrid Cloud:**
- Using public cloud AND private cloud together
- Both must meet cloud computing criteria

**Hybrid Environment:**
- Using on-premises data center AND AWS together
- Does NOT require private cloud (which must meet cloud computing criteria)

### Common Misconception:
- **WRONG:** Using AWS and on-premises data center = Hybrid Cloud
- **CORRECT:** Using AWS and on-premises data center = Hybrid Environment
- **CORRECT:** Using public cloud and private cloud = Hybrid Cloud

---

## AWS Public vs. Private Services

### How AWS Determines Public or Private:

**Determined by Network (not what you might think)**

---

## AWS Public Services

### Definition:
- Service that can be connected to from anywhere there's an internet connection

### Architecture:

**AWS Public Zone:**
- Sits inside AWS
- Sits adjacent/beside public internet (NOT the same as public internet)
- Has network attached directly to public internet
- Can communicate openly with public internet

**Where Public Services Sit:**
- AWS public services sit and run from public zone
- Network attached to open internet

**Example: Amazon S3**
- AWS public service
- When users connect to S3 bucket, they connect through public internet

---

## AWS Private Services

### Definition:
- Private AWS service that lives inside AWS private zone

### Architecture:

**AWS Private Zone:**
- No direct connection to open internet
- No direct connection to AWS public zone
- Completely isolated by default

**What You Can Create:**
- Isolated environment like Amazon VPC
- Amazon EC2 instance (isolated by default)

**Adding Connectivity:**
- Can add permissions for EC2 instance or VPC to access:
  - Public zone
  - Public internet
- Must configure routing or make instance public
- Will be covered in depth later in course

**Default Access:**
- Only services inside private zone can access services inside private zone
- No permissions for private zone except local routes by default

---

## Importance for Exam

### Why This Matters:

**Throughout Course:**
- Will discuss if AWS services are private or public

**Exam Questions:**
- May ask how to give user or customer access to specific AWS service
- Understanding what makes service public vs. private is critical
- Understanding how to design connectivity is essential
- With this knowledge, can confidently answer these questions

---

## Connectivity Options

### Focus:
- How network connectivity can be handled to various AWS services

### Three Main Connectivity Types:

**1. Virtual Private Network (VPN)**

**2. AWS Direct Connect**

**3. Public Internet**

---

## What You Should Know About Connectivity

### Understanding Required:

**1. Advantages and Limitations:**
- Of each connectivity type

**2. Use Cases:**
- Where one might be preferred
- Where one might be avoided

**3. Generalities:**
- How they work

---

## AWS Direct Connect

### Key Characteristics:

**Definition:**
- Private dedicated connection

**Keyword for Exam:**
- "Dedicated connection" = Direct Connect

---

## Internet Gateway vs. NAT Gateway

### Example Question:

**Scenario:**
- Want to connect public Amazon EC2 instances in public subnet to public internet
- What do you use: Internet Gateway or NAT Gateway?

**Answer: Internet Gateway**

### Internet Gateway Characteristics:
- Horizontally scaled
- Redundant
- Highly available
- Allows communication and traffic between:
  - Instances in your VPC
  - Public internet

---

## Key Exam Expectations

### What You're Expected to Know:

**1. Utilization:**
- How connectivity, deployment, and operational methods can be utilized

**2. Decision Making:**
- When to choose one option over another

**3. Beyond Definitions:**
- More than just definitions
- Envision how you would use components, tools, features, and services
- How they interact with each other

**4. Interaction Understanding:**
- Not expected to be expert on everything
- Base understanding includes comprehending interactions

---

## Study Strategy for Task Statement 3.1

### Questions to Guide Your Study:

**For Each Method/Model:**
1. What is it?
2. When would I use it?
3. What are its strengths?
4. What are its limitations?
5. How does it interact with other components?

**For Deployment Models:**
1. What defines this model?
2. When would I choose this model?
3. What are the considerations?
4. What are real-world use cases?

**For Connectivity Options:**
1. What type of connection does it provide?
2. What are advantages?
3. What are limitations?
4. When would I use this over alternatives?

---

## Exam Tips Summary

### Critical Concepts:

**Deployment Models:**
- Public Cloud: Available to public, meets cloud criteria
- Private Cloud: Dedicated on-premises, meets cloud criteria
- Hybrid Cloud: Public + Private cloud (both meet cloud criteria)
- Hybrid Environment: AWS + on-premises data center (different from hybrid cloud)
- Multi-Cloud: Multiple public clouds

**AWS Service Architecture:**
- Public Services: In public zone, connected from anywhere with internet
- Private Services: In private zone, isolated by default
- Example: S3 is public service, EC2 is private service (by default)

**Connectivity:**
- VPN, Direct Connect, Public Internet
- Internet Gateway: Connects VPC to public internet
- Direct Connect keyword: "Dedicated connection"

**Methods of Access:**
- SDKs (programmatic)
- CLI (command line)
- Management Console (graphical)
- Infrastructure as Code (CloudFormation)

---
# AWS Cloud Practitioner Notes - Task Statement 3.2: Define the AWS Global Infrastructure

## Importance of Understanding Global Infrastructure

### Why It Matters:
- Helps you know how to connect, design, build, and deploy architectures in AWS
- Remember: Components covered earlier include Availability Zones, Regions, and Edge Locations

### What You Need to Understand:
1. How components function individually
2. How components function together
3. What choices you have
4. How to determine when services use specific Availability Zone, Region, or Edge Location

---

## AWS Service Resilience Levels

### Three Levels of Resilience:

**1. Globally Resilient Services**

**Definition:**
- Service operates globally
- Example: Single database with data replicated across AWS Regions
- Region can fail, but service continues to run

**Examples:**
- IAM (Identity and Access Management)
- CloudFront
- Amazon Route 53

**2. Region Resilient Services**

**Definition:**
- Operate in one Region
- One set of data in that Region
- Replicate data to multiple Availability Zones inside that Region
- If you lose one Availability Zone: Service continues to operate
- If whole Region fails: Service fails

**Examples:**
- Amazon EFS (Elastic File System)
- AWS Batch

**3. Availability Zone Resilient Services**

**Definition:**
- Run in single Availability Zone
- If that Availability Zone fails: Service fails

**Examples:**
- Amazon EBS (Elastic Block Store)

**Zonal Services:**
- Amazon EC2 (tied to particular Availability Zone)

### Exam Tip:
**Know what level of resilience an AWS service has**
- Helps answer exam questions
- Gives much deeper understanding

---

## AWS Global Infrastructure Overview

### What It Is:
- Collection of individual infrastructures located all over the world
- AWS offers Regions and Edge Locations globally
- Designed to have multiple Regions, multiple Availability Zones, and multiple Edge Locations around the world

### Infrastructure Layers:

**Foundation Layer:**
- AWS Regions around the world

**Service Layer on Top:**
Multiple levels of services including:

**Compute:**
- Amazon EC2
- AWS Lambda

**Storage:**
- Amazon S3
- Amazon EFS

**Database:**
- Amazon RDS
- Amazon Aurora
- Amazon DynamoDB

**Other Service Categories:**
- Migration and Transfer
- Network and Content Delivery
- Developer Tools
- Robotics
- Blockchain
- Satellite
- Management and Governance
- Machine Learning
- Security, Identity, and Compliance
- Application Integration
- Cost Management
- And more

---

## AWS Regions

### Definition:
- Geographical area consisting of two or more Availability Zones

### Key Characteristics:

**1. Regional Rules:**
- All Regions are under that Region's rules
- If data sits in particular Region: Data will NOT leave that Region
- Unless you specifically move that data

**2. Geographic Distribution:**
- AWS designs Regions to be geographically spread across world
- Allows use of different Regions to design infrastructure that can withstand global disasters
- Separation between Regions
- Each Region is fault tolerant

### Exam Tip (and Real World):

**When Selecting Regions for Applications:**
1. Check if there are compliance requirements
2. Choose closest Region to reduce latency for users

### Region Extensions:

**1. Local Zones**
- Extension of AWS Region
- In close geographic proximity to your users

**2. AWS Wavelength**
- Similar to Local Zones
- Helps build applications that deliver ultra-low latency to mobile devices and end users
- Has Wavelength Zones:
  - Isolated zone in carrier location where Wavelength infrastructure is deployed
  - Tied to AWS Region
  - Extensions like Local Zones

---

## Availability Zones (AZs)

### Definition:
- One or more data centers with:
  - Redundant power
  - Networking connectivity
  - And more

### Structure:

**Data Centers:**
- In separate facilities inside different AWS Regions
- AWS has multiple data centers across world
- Building filled with:
  - Servers
  - SANs (Storage Area Networks)
  - Switches
  - Load balancers
  - Firewalls
  - Storage
  - And more

**Availability Zone Composition:**
- Think of AZ as one or more data centers
- Can have more than one data center in each AZ
- Each AZ is isolated:
  - Compute
  - Storage
  - Network
  - And more

### High Availability Design:

**Distribution Strategy:**
- Distribute infrastructure across multiple AZs in your Region
- For high availability

**Isolation Benefits:**
- If one AZ fails: Other AZs should remain operational
- Because they are isolated from each other
- But connected with high-speed redundant networking

**Service Placement:**
- Services can be placed across multiple AZs
- Adds resilience and high availability

---

## AWS Edge Locations

### Definition:
- Global service
- Endpoint for AWS used for caching content

### AWS Content Delivery Network (CDN):

**CloudFront:**
- AWS CDN service

**How It Works:**
1. User requests certain information
2. Information is cached at edge location
3. Next time another user requests same information:
   - Information already available
   - Delivered much faster
   - No need to go back to database

**Example: Netflix**
- Uses edge locations to store content as close to customers as possible
- Customers get very low latency when requesting movies and shows

**Performance Principle:**
- Further data is from customers: Slower the transfer
- Closer data is to customers: Faster the transfer

---

## AWS Global Accelerator

### What It Is:
- Global service
- Supports endpoints in multiple AWS Regions
- Improves performance of applications for local and global users

### CloudFront vs. Global Accelerator

**Important for Exam: Know the Difference**

**Similarities:**
- Both use AWS Global Network
- Both use Edge Locations
- Both integrate with AWS Shield for DDoS protection

**CloudFront:**
- Improves content delivery for cached content
- Both static and dynamic content
- Content served from edge location most of the time
- Has caching available

**Global Accelerator:**
- Improves performance for applications over TCP and UDP
- Packets proxied from edge locations to applications running in one or more Regions
- All requests make it to the edge
- NO caching available
- Great for HTTP use cases that need:
  - Static IP
  - Fast regional failover

---

## Cloud Service Models

### Ensure You Know:

**Infrastructure as a Service (IaaS)**

**Platform as a Service (PaaS)**

**Software as a Service (SaaS)**

**Additional Models:**
- Database as a Service (DBaaS)
- And more

---

## Study Components Separately

### Availability Zones Study Focus:

**What to Study:**
1. Which services are bound by AZ borders
2. How AZs help when building highly available environment
3. How AZs come into play when determining points of failure in architectures
4. How communication is handled going from one AZ to another
5. Which services deal specifically with AZs
6. How services connect and communicate across AZs

**Note:** Communication differs based on services

---

### Regions Study Focus:

**Similar to AZs, But Also:**
1. Ways to use Regions for disaster recovery
2. Ways to use Regions for business continuity
3. What you can do to avoid catastrophic failures
4. What services help you utilize Regions
5. Why you would use different Regions
6. What benefits from using particular Region
7. What benefits from using multiple Regions
8. How Region usage affects compliance requirements

**Important Compliance Note:**
- Data management often determined by sovereign borders
- Know how laws and requirements affect AWS Cloud usage

---

### Edge Locations Study Focus:

**What to Study:**
1. What services take advantage of edge locations
2. How those services differ in their utilization
3. Can you choose which edge location to use?
4. How edge locations are utilized by CloudFront
5. How edge locations are utilized by AWS Global Accelerator
6. Do edge locations come into play only with certain services?
7. Are there other times when you're using them?
8. What benefits are provided by edge locations?
9. What level of management can you dictate?

---

## Foundational Understanding

### Critical Exam Knowledge:

**Availability Zones, Regions, and Edge Locations are foundational components**

**What You Must Understand:**
1. How they help your architectures
2. How they affect your architectures
3. What you can do to take advantage of their benefits
4. Services that are bound by these components
5. Services that directly interact with these components

---

## Exam Preparation Summary

### Most Likely to See on Exam:

**Questions on:**
- Differences between Region, Availability Zone, and Edge Locations
- When to use which component
- How components work together

### Key Concepts to Master:

**Resilience Levels:**
- Globally resilient (IAM, CloudFront, Route 53)
- Region resilient (EFS, Batch)
- AZ resilient (EBS, EC2)

**Region Selection:**
- Compliance requirements
- Latency considerations
- Data sovereignty

**High Availability:**
- Distribute across multiple AZs
- Use multiple Regions for disaster recovery
- Understand isolation and connectivity

**Content Delivery:**
- CloudFront: Caching at edge locations
- Global Accelerator: TCP/UDP performance, no caching
- Know differences and use cases

**Compliance:**
- Data doesn't leave Region unless you move it
- Sovereign border considerations
- Regional rules and requirements

---

## Critical Exam Tips

**Remember:**
1. Know resilience level of each AWS service
2. Understand Region vs. AZ vs. Edge Location differences
3. Know when to use CloudFront vs. Global Accelerator
4. Understand compliance and data sovereignty
5. Know how to design for high availability across AZs
6. Understand disaster recovery across Regions
7. Know which services are bound to which infrastructure components

---
# AWS Cloud Practitioner Notes - Task Statement 3.3: Identify AWS Compute Services

## Amazon EC2 (Elastic Compute Cloud)

### What is Amazon EC2?

**Definition:**
- Virtualization as a Service
- Infrastructure as a Service (IaaS) product
- Provides significant value to AWS accounts

### Fundamentals: What is Virtualization?

**Definition:**
- Running one or more operating systems on a piece of physical hardware (server)
- Each operating system is separate (along with their applications)
- Allows multiple different privileged applications to run on same hardware using software to make calls

**History Note:**
- Started with two different designs
- Has kept evolving
- Virtualization fundamentals content available if interested

---

## Amazon EC2 Architecture

### EC2 as Default Compute Service:

**EC2 Instances:**
- Virtual machines (VMs)
- Run on EC2 hosts

**EC2 Hosts:**
- Physical hardware or physical servers
- AWS manages these
- Either shared or dedicated

---

## EC2 Host Types

### 1. Shared Hosts

**Characteristics:**
- Default for EC2 hosts
- Shared among different AWS customers
- Customers do NOT get ownership of host hardware
- Pay for individual instances and resources

**Important Note:**
- When using shared host: Your instance is isolated from other AWS customers

### 2. Dedicated Hosts

**Characteristics:**
- Pay for entire EC2 host
- NOT just the instances running on that host
- Do NOT share it
- Pay for entire host regardless of how many instances you spin up

---

## EC2 Instance Resilience

### Availability Zone Resilient Service:

**Why:**
- EC2 hosts sit in Availability Zone
- If that AZ fails: Host and instances running on host also fail

---

## EC2 Storage

### Instance Store (Local Storage)

**Characteristics:**
- EC2 hosts inside AZ have local storage called instance store
- **KEY UNDERSTANDING:** Instance store is TEMPORARY storage

**Critical Warning:**
- If EC2 instance moves off host to another host
- Storage in instance store is LOST

---

## EC2 Networking

### Elastic Network Interface (ENI)

**How It Works:**
1. EC2 instance launched into specific subnet inside Amazon VPC
2. Primary Elastic Network Interface provisioned into that subnet
3. Mapped to physical hardware of that EC2 host for that AZ
4. Can add multiple different ENIs to EC2 instances

---

## Amazon EBS (Elastic Block Store)

### What is EBS?

**Purpose:**
- Lets you access volumes of persistent storage

### Network Architecture:

**Inside Amazon VPC:**
- Data network set up for Elastic Network Interfaces
- Storage network to connect to EBS volumes

### EBS Resilience:

**Availability Zone Resilient Service:**
- Can have different EBS volumes running in different subnets for different EC2 instances
- **CANNOT** connect EC2 instances to EBS volume in different Availability Zone or subnet

---

## EC2 Instance Types

### What You Get When Choosing and Launching EC2 Instance:

**Resources:**
- Raw amount of CPU
- Memory
- Local storage
- Type of storage

### Important Considerations:

**1. Performance:**
- Be aware of performance for each instance type
- Each instance type provides storage bandwidth
- Each instance type provides network bandwidth
- Need to ensure enough bandwidth with chosen instance type

**2. Resource Ratios:**
- Amount of resource you get for each raw amount
- Example: Instance suitable for compute
  - Gives more CPU
  - Gives less memory
- Example: Instance suitable for memory
  - Gives more memory
  - Gives less compute

**3. Additional Features:**
- Different instance types have additional capabilities
- Example: GPU for graphic processing

**Key Understanding:**
- Know your AWS account structure
- Know your goals
- Know your design
- Then choose appropriate instance type

---

## Five EC2 Instance Categories

### 1. General Purpose

**Use Case:**
- Great for default steady state workloads
- Even resource ratios
- Should be used as default unless you have specific requirements

### 2. Compute Optimized

**Use Cases:**
- Designed for high-performance computing
- Media processing
- Machine learning
- Gaming
- Scientific modeling
- And more

**Characteristics:**
- Resource ratios usually more CPU than memory
- Provide access to higher performance CPUs

### 3. Memory Optimized

**Use Cases:**
- Great for processing large in-memory datasets
- Database workloads

**Characteristics:**
- Resource ratios usually more memory than CPU

### 4. Accelerated Computing

**Use Cases:**
- Designed for specific requirements
- Hardware GPU
- Field Programmable Gate Arrays (FPGAs)

### 5. Storage Optimized

**Use Cases:**
- Designed for applications using:
  - Data warehousing
  - Analytic workloads
  - Elasticsearch
  - SQL
  - Random I/Os

---

## Burstable Instances

### How They Work:

**Characteristics:**
- Instances have normal CPU loads that are low
- Given allocation of burst credits
- Allows you to burst up
- Then return to normal level

**Benefits:**
- Usually cheaper
- Great option for variable workloads

---

## Amazon Machine Images (AMIs)

### For the Exam:

**Know:**
- You can create custom AMIs for Amazon EC2 instances

### Golden AMI:

**Definition:**
- AMI that contains:
  - Latest security patches
  - Software
  - Configuration
  - Software agents needed for:
    - Logging
    - Security
    - Maintenance
    - Performance monitoring

---

## EC2 Instance Metadata

### Question: Where to Find Instance Information?

**Options:**
- Instance metadata
- Instance user data
- AMI

**Answer: Instance Metadata**

### Instance Metadata:

**Definition:**
- Data about your instance
- Can use to configure or manage instance

**What You Can Get:**
- Instance ID
- Public key
- Public IP address
- Other information

**How to Access:**
- Using http://169.254.169.254/latest/meta-data

### Instance User Data:

**Purpose:**
- Used to perform common automated configuration tasks
- Run custom scripts after instance starts

**What It Does NOT Contain:**
- Instance ID
- Public keys
- Public IP address of EC2 instance

---

## Containers

### What You Need to Know for Exam:

**Understanding:**
- What containers are
- What benefits container computing provides

### EC2 vs. Containers - Key Difference:

**Amazon EC2:**
- Guest operating system on EC2 instances takes up a lot of space
- Resources consuming memory and disk space
- Leaves just a little bit of space for applications
- Many instances using same operating system
- Lots of resources consumed
- Lots of usage
- Lots of duplication

**Containers:**
- Designed to handle it differently

### Container Architecture:

**Structure:**
1. Hardware (bottom layer)
2. One operating system on top of hardware (only one OS)
3. Container engine on top of OS
4. Container runs as process within host operating system

**Benefits:**
- Can use host OS for networking and more
- More efficient resource usage
- Less duplication

---

## Amazon ECS (Elastic Container Service)

### What is ECS?

**Definition:**
- Service that accepts containers along with instructions
- Instructions on where and how to run those containers

**Characteristics:**
- AWS managed container-based compute service
- Container orchestration service

---

## Amazon EKS (Elastic Kubernetes Service)

### What is EKS?

**Definition:**
- Allows you to run AWS-powered Kubernetes on Amazon EC2 instances

---

## AWS Lambda

### What is Lambda?

**Definition:**
- Function as a Service (FaaS) product

### How It Works:

**Lambda Functions:**
- Accepts functions (small piece of code written in a language)
- Use a runtime (Python, Java, Node.js, etc.)
- Billed for duration of execution

**Event-Driven:**
- Lambda is event-driven service
- Lambda functions invoked on event occurring

**Process:**
1. Develop code in a language
2. Pick runtime using that language
3. Execute code based on triggering of an event

**Serverless:**
- Lambda is considered serverless
- Great compute alternative for serverless architecture

---

## AWS Compute Options Summary

### Multiple Choices:

**1. AWS Lambda:**
- Functions

**2. Amazon Elastic Beanstalk:**
- Application stacks

**3. Amazon ECS:**
- Container management

**4. EC2:**
- Traditional virtual machines

**Many compute options within AWS available**

---

## High Availability and Scalability

### Achieving HA, Fault Tolerance, and Elasticity:

**Tools Used:**
- Auto scaling
- Load balancers

### Auto Scaling Groups:

**Purpose:**
- How to configure Amazon EC2 to scale automatically based on different criteria

### Load Balancing:

**Definition:**
- Method used to distribute incoming connections across group of servers or services

**How It Works:**
- Incoming connections made to load balancer
- Load balancer distributes them to servers or services

---

## AWS Load Balancers

### Four Choices:

**1. Classic Load Balancer**

**2. Application Load Balancer**

**3. Network Load Balancer**

**4. Gateway Load Balancer**

### Elastic Load Balancer (ELB) Family:

**What They Are:**
- These four make up family of Elastic Load Balancers
- Great to pair with auto scaling groups
- Enhance:
  - High availability
  - Fault tolerance
  - Scalability of application

### Load Balancer Architecture:

**Important Understanding:**
- When you create load balancer: Creating one entity, one load balancer
- Actually creates an ELB node

**High Availability:**
- Load balancer node should be placed in each AZ that load balancer uses

---

## Exam Preparation Summary

### What You Need to Know:

**1. EC2 Instance Types:**
- Appropriate use of different EC2 instance types

**2. Container Options:**
- Appropriate use of different container options

**3. Serverless Compute:**
- Appropriate use of different serverless compute options

**4. Auto Scaling:**
- Understand that auto scaling provides elasticity

**5. Load Balancing:**
- How to use auto scaling and load balancing together

---

## Key Exam Concepts

### Critical Understanding:

**EC2:**
- IaaS product
- AZ resilient service
- Instance store is temporary (lost if instance moves)
- EBS is persistent but AZ-specific
- Five instance categories (General Purpose, Compute, Memory, Accelerated, Storage)
- Burstable instances for variable workloads
- Shared vs. Dedicated hosts

**Containers:**
- More efficient than traditional VMs
- ECS: AWS managed container orchestration
- EKS: Kubernetes on AWS

**Lambda:**
- FaaS, serverless
- Event-driven
- Billed by execution duration

**HA and Scaling:**
- Auto scaling provides elasticity
- Load balancers distribute traffic
- Four types of load balancers
- Use together for HA, fault tolerance, scalability

**Instance Metadata:**
- Access at http://169.254.169.254/latest/meta-data
- Contains instance information
- Different from user data (which runs scripts)

---
# AWS Cloud Practitioner Notes - Task Statement 3.4: Identify AWS Database Services

## Database Fundamentals

### Important for Exam:
- Should understand what a database is
- Should understand how it works

---

## Amazon RDS (Relational Database Service)

### What is RDS?

**Definition:**
- Database as a Service (DBaaS)
- Provides managed database instances

### What AWS Manages:
- AWS handles the management
- Physical hardware
- Operating system
- And more

### What You Get:
- Access to managed database instance
- Lots of benefits
- Performance enhancements

### Supported Database Engines:
- MySQL
- MariaDB
- PostgreSQL
- Oracle
- Microsoft SQL Server
- Amazon Aurora

**You can pick which database engine works with your application requirements**

### RDS Instance Characteristics:

**Similar to EC2:**
- Comes in different types
- Different sizes
- Different families (like EC2 instances)

**Availability Zone Options:**
- Can be in one AZ
- Can be in multiple AZs

**Storage:**
- Allocate storage for instance to use
- Dedicated storage for that database instance

**Security:**
- Access controlled through security groups

---

## RDS Availability Configurations

### Single AZ Configuration:

**Vulnerability:**
- RDS instances in single AZ can be vulnerable to failure in that single AZ
- Instance and storage are in single AZ

### Multi-AZ Configuration:

**How It Works:**
- Allocates secondary hardware in different AZ
- Second database instance called standby replica instance
- Uses synchronous replication from primary to standby instance

---

## RDS Read Replicas

### What Are Read Replicas?

**Definition:**
- Read-only replica of your RDS database instance

### Two Main Benefits:
1. Performance benefits
2. Availability benefits

### Characteristics:
- For read operations
- Data replicated asynchronously

---

## Replication Types - Critical for Exam

### Synchronous Replication:

**Where Used:**
- Multi-AZ configurations

**How It Works:**
- Data written to primary instance
- Replicated to standby replica at same time

### Asynchronous Replication:

**Where Used:**
- Read replicas

### Exam Tip:
- **See "asynchronous"** → Think read replicas
- **See "synchronous"** → Choose for multi-AZ environment or scenario

---

## Amazon Aurora

### Key Differences from RDS:

**Has quite a few differences and improvements over Amazon RDS**

### 1. Architecture Difference:

**Aurora Architecture:**
- Uses base architecture of a cluster
- Compatible with MySQL and PostgreSQL engines
- Made up of:
  - Single primary instance
  - Zero or more read replicas

**Key Difference from RDS:**
- Aurora read replicas provide:
  - Benefits of reads
  - Benefits of multi-AZ
- Can be used to improve availability AND read operations on cluster

### 2. Storage Difference:

**Aurora Storage:**
- Does NOT use local storage for compute
- Uses shared cluster volume
- Provides:
  - Faster provisioning
  - Improved availability
  - Better performance

---

## Aurora Serverless

### What It Is:
- Version of Amazon Aurora database product
- Do NOT have to provision or manage database instances

### How It Works:

**Storage:**
- Provides same shared cluster storage
- Six copies of data across three AZs

**Capacity:**
- Do NOT provision cluster the same way
- Use ACUs (Aurora Capacity Units)
- ACU provides:
  - Certain amount of compute
  - Corresponding amount of memory

**Scaling:**
- Choose minimum ACU and maximum ACU
- Aurora Serverless cluster scales between minimum and maximum value
- Adds and removes capacity based on load

**Cool Feature:**
- ACU can go down to zero
- Can be paused after period of inactivity
- Great cost savings: When paused, only pay for storage

---

## Aurora Global Databases

### What It Is:
- Feature of Aurora provisioned clusters

### Capabilities:
- Allows data to be replicated globally

### Benefits:

**1. Recovery Improvements:**
- Significant recovery point objective (RPO) improvements
- Significant recovery time objective (RTO) improvements
- For business continuity and disaster recovery planning

**2. Performance Improvements:**
- For customers with data located closer to them
- In read-only form

**Replication:**
- Occurs at storage layer
- Generally less than 1 second between all AWS Regions

---

## Amazon DynamoDB

### What is DynamoDB?

**Definition:**
- NoSQL Database as a Service product
- Public service (sits in AWS Public Zone)

### What AWS Manages:
- AWS manages DynamoDB for you
- Do NOT need to manage servers or infrastructure

### Data Types Supported:
- Simple key-value data
- Structured data

### Scaling Options:

**Two Modes:**
1. Provisioned capacity with manual controls
2. On-demand mode (handles scaling for you)

### Resilience:

**Standard:**
- Highly resilient across multiple AZs in a Region

**Global Tables:**
- Can configure for global resilience
- Extra cost

---

## In-Memory Databases

### Amazon ElastiCache

**What It Is:**
- Managed in-memory cache
- For performance improvements for reads

**Supported Caching Engines:**
- Redis
- memcacheD

**Exam Tip:**
- If you see memcacheD or Redis → Answer is probably ElastiCache

**Use Cases:**

**1. Caching:**
- Designed to store reads
- Deliver results from in-memory caching
- Improves performance
- Instead of consulting database each time for reads:
  - Cache results
  - Deliver results quicker

**2. Session Management:**
- Can store user session states
- Mentioned in Domain 1 under scaling and high availability
- Can be used as performance-enhancing tool
- Can be used with fault-tolerant architectures

**Can Be Used With DynamoDB:**
- ElastiCache can be used with DynamoDB
- But AWS created DAX specifically for DynamoDB

---

## Amazon DynamoDB Accelerator (DAX)

### What is DAX?

**Purpose:**
- Created to be used specifically with DynamoDB

### Why DAX Exists:

**DynamoDB Characteristics:**
- Designed to be low-maintenance
- High-performing database
- Provides access to data in milliseconds

**DAX Purpose:**
- Some edge locations need data faster (microseconds)
- For high-read sessions
- Provides in-memory cache for DynamoDB

### Exam Tip:

**When to Use DAX:**
- Designed for latency-sensitive workloads
- Designed for high-read workloads

**Exam Question:**
- "What is best caching product to use with DynamoDB?"
- **Answer: DAX**

### When NOT to Use DAX:
- NOT great for applications that need strongly consistent reads
- More for eventually consistent reads

---

## Amazon Redshift

### What is Redshift?

**Definition:**
- Petabyte-scale data warehousing solution from AWS
- Column-based database engine
- For analytic workloads

### OLTP vs. OLAP:

**Most RDS Databases:**
- Used for OLTP (Online Transaction Processing)

**Redshift:**
- Designed for OLAP (Online Analytical Processing)
- NOT the type of database where you update individual records

### Use Case:
- Data warehousing analytics
- Everything stored in columns

### Column-Based vs. Row-Based:

**Column-Based Databases (Redshift):**
- Great at queries
- All data is in columns
- Great for analytics

**Row-Based Databases:**
- Great for transaction-type processing

### Technical Details:

**Based On:**
- PostgreSQL
- But is online analytical processing
- NOT used for online transactional processing

**Architecture:**
- Uses cluster architecture
- Unloads and uploads data to S3

**Data Sources:**
- Can accept data from:
  - DynamoDB
  - Database Migration Service
  - Other databases
  - Amazon Kinesis

**Redshift Spectrum:**
- Can perform queries directly against S3

### Exam Tip - Keywords:
- **Redshift** = Data warehouse
- Used for analytical and summarization transactions
- Can scale to almost any workload needed
- Petabyte-scale database

---

## Database Migration Tools

### AWS Snow Family

**Purpose:**
- Services to migrate large amounts of data in and out of AWS

**What It Includes:**
- AWS Snowcone
- AWS Snowball
- AWS Snowmobile

**Characteristics:**
- Collection of physical devices
- Help migrate large amounts of data into and out of cloud
- Without depending on networks
- Helps apply AWS services for:
  - Analytics
  - File systems
  - Archives

### Example Question:

**Scenario:**
- Move terabytes to petabytes of data into AWS
- Using appliances with storage and compute capabilities

**Answer: AWS Snowball Edge**

### AWS Snowball Edge:

**What It Is:**
- Data migration and edge computing device

**Two Options:**
1. Snowball Edge Storage Optimized
2. Snowball Edge Compute Optimized

**Capabilities:**
- Supports specific Amazon EC2 instance types
- Supports AWS Lambda functions
- Customers can:
  - Develop and test in AWS
  - Deploy applications on devices in remote locations
  - Collect, pre-process, and return data

**Common Use Cases:**
- Data migration
- Data transport
- Image collation
- IoT sensor stream capture
- Machine learning

### Snow Family Comparison:

**AWS Snowcone:**
- For 8 terabytes

**AWS Snowball Edge:**
- For terabytes to petabytes

**AWS Snowmobile:**
- For petabytes to exabytes

---

## AWS Database Migration Service (DMS)

### What is DMS?

**Definition:**
- Managed service capable of both:
  - Data migration
  - Schema conversion

### Traditional Migration Methods:

**1. Backup and Restore:**
- Stop all I/O operations on database
- Take backup
- Do restore
- Update applications to new database endpoint
- Requires full outage during migration

**2. Replication:**
- Configure replication instance between source and target database
- Allow replication to replicate all existing data
- Migrate any new transactions
- Usually has very little downtime
- Simply update application to point to new endpoint
- **Problems:** Very admin intensive, difficult to set up right

### How DMS Works:

**AWS Solution:**
- DMS handles overhead and configuration for you

**Process:**
1. Create replication instance
2. Define source endpoint
3. Define target endpoint
4. Include any required authentication
5. All data migrated from source to target
6. Operations continue on source database
7. Migrate to target when ready

### AWS Schema Conversion Tool:

**Purpose:**
- Helps transform between different database engines for migration

### DMS Use Cases:
- Scaling resources up or down with little downtime
- Migrating databases from on-premises to AWS
- Migrating from AWS to on-premises
- Migrating from other cloud platforms
- Schema Conversion Tool allows moving data between different database engines

---

## AWS DataSync

### What is DataSync?

**Purpose:**
- Makes it simple and fast to move large amounts of data online

**Between:**
- On-premises storage
- And:
  - Amazon S3
  - Amazon EFS
  - Amazon FSx for Windows File Server

### Why Use DataSync:

**Problem:**
- Manual tasks related to data transfers:
  - Slow down migrations
  - Burden IT operations

**Solution - DataSync Automatically Handles:**
- Scripting copy jobs
- Scheduling transfers
- Monitoring transfers
- Validating data
- Optimizing network utilization

### Performance:
- Can transfer hundreds of terabytes and millions of files
- Speeds up to 10 times faster than open-source tools
- Over internet or AWS Direct Connect links

### Use Cases:
- Migrate active datasets or archives to AWS
- Transfer data to cloud for timely analysis and processing
- Replicate data to AWS for business continuity

---

## Database Services - Key Study Areas

### Major Focus:

**Differentiate Between Services:**
- Which services fit specific scenarios

**Comparisons Needed:**

**1. Comparing Services to Each Other:**
- Amazon RDS
- Amazon DynamoDB
- Amazon Redshift

**2. Comparing to Self-Managed:**
- Compare managed services to managing own database on EC2 instances

### Questions to Consider:

**For Managed Services:**
1. What advantages from utilizing managed service?
2. How does managed service differ from database engine installed on instance?
   - Customability
   - Management
   - Performance
3. What are limitations of each style of database?
4. How do services fit into your builds (or hypothetical builds)?
5. What role could each play?

**Remember:** No one-size-fits-all solution

### Varying Levels of Management:

**Compare:**
- Amazon DynamoDB management
- Amazon RDS management
- Amazon EKS management
- AWS Fargate management
- And others

**Evaluate:**
- Where benefits lie
- How to use in conjunction with each other in architecture
- What they complement or replace
- How topics come into play:
  - Availability
  - Failover
  - Data consistency

### Features and Customization:
- Features of each database service useful for matching requirements
- Customization options help match different scenarios and use cases

---

## Exam Preparation Summary

### Critical Concepts:

**RDS:**
- Managed relational database
- Multi-AZ (synchronous replication)
- Read replicas (asynchronous replication)
- Supports multiple database engines

**Aurora:**
- Cluster architecture
- Shared cluster volume
- Aurora Serverless (ACUs, can pause)
- Aurora Global Databases (< 1 second replication)

**DynamoDB:**
- NoSQL, public service
- Key-value and structured data
- Provisioned or on-demand
- Global tables for global resilience

**ElastiCache:**
- In-memory cache
- Redis or memcacheD
- For performance and session management

**DAX:**
- Specifically for DynamoDB
- Microsecond latency
- High-read workloads
- Eventually consistent reads

**Redshift:**
- Data warehouse (OLAP)
- Column-based
- Petabyte-scale
- For analytics

**Migration Tools:**
- Snow Family (physical devices)
- DMS (Database Migration Service)
- Schema Conversion Tool
- DataSync (online data transfer)

---

# AWS Cloud Practitioner Notes - Task Statement 3.5: Identify AWS Network Services

## Networking Fundamentals Importance

### Critical Foundation:
- Always recommend understanding networking fundamentals
- Everything you do in AWS uses networking
- When communicating with AWS
- When creating connections between on-premises and AWS

### Why It Matters:
- Solid network design is foundation of any environment
- Designing and configuring networking is different in AWS than on-premises

---

## Amazon VPC (Virtual Private Cloud)

### What is Amazon VPC?

**Definition:**
- Virtual Private Cloud
- Basically your very own data center in the cloud

**Capabilities:**
- Provision own Amazon VPC in logically isolated section of AWS
- Launch different resources
- Create own Virtual Private Network
- Complete control over virtual networking environment

**Control Includes:**
- Choosing own IP address ranges
- Creating own subnets
- Configuring access with route tables
- Configuring network gateways

### Security Layers in VPC:

**Multiple Different Layers:**
- Network Access Control Lists (NACLs)
- Security Groups
- Configure to control who and what can access resources inside Amazon VPC

### What VPC Is Used For:
- Create private networks in AWS
- Private services run from Amazon VPC

**Connectivity:**
- Connect Amazon VPCs from AWS private network to on-premises (hybrid environment)
- Connect to other cloud platforms (multi-cloud environment)

---

## VPC Regional Characteristics

### Regional Service:

**When You Create VPC:**
- In one Region
- In one AWS account
- Makes VPC a regional service

**Resilience:**
- VPCs operate resiliently
- By operating in multiple Availability Zones in specific Region

### Default Privacy:

**By Default:**
- Amazon VPC is isolated and private
- Until you explicitly grant public access

**One Exception - Default Amazon VPC:**
- Need to know this for exam

---

## Two Types of Amazon VPCs

### 1. Default VPC

**Characteristics:**
- Can have only ONE default Amazon VPC per Region
- Created by AWS when you create AWS account
- AWS sets up configuration for you

**Configuration:**
- Each default VPC comes with one VPC CIDR range
- CIDR range = given range of IP addresses
- VPC CIDR defines start and end range of IP addresses default VPC can use

**How CIDR Works:**
- Everything inside Amazon VPC uses CIDR range
- All communications TO Amazon VPC need to use VPC CIDR
- Outgoing communications will be FROM VPC CIDR

**Default Configuration:**
- All default Amazon VPCs configured same way
- Configured to have one subnet located in each AZ of that Region
- Each subnet uses part of IP address range of VPC CIDR

**Resilience Example:**
- If one AZ fails: Subnet in that AZ also fails
- But: Other subnets in other AZs still operating

### 2. Custom VPCs

**Characteristics:**
- Configured by you
- You responsible for all configurations
- By default: Isolated and private

---

## VPC Components

### VPC Router

**What It Is:**
- Every Amazon VPC has VPC router
- Highly available
- Moves traffic from somewhere to somewhere else

**How It Works:**
- Runs in all AZs that Amazon VPC uses
- Has network interface in each subnet in Amazon VPC
- Uses Network+1 address (part of networking fundamentals)

**Management:**
- Never need to worry about VPC router
- Just works
- Managed by AWS
- Routes traffic between subnets in Amazon VPC

**Control:**
- Can control router by:
  - Creating route tables
  - Associate route table with subnet
  - Add rules to allow traffic in and out of subnets

### Route Tables

**Main Route Table:**
- Each Amazon VPC has main route table associated with subnets
- If you don't explicitly associate new route table with subnet: VPC uses main route table

**Association Rules:**
- Subnet can only have ONE route table associated at a time
- But: Can use one route table for many different subnets in Amazon VPC

---

## Internet Gateway

### Characteristics:

**Limitations:**
- Amazon VPC can only have ONE internet gateway at a time
- For default Amazon VPC: Internet gateway already attached

**Resilience:**
- Regional resilient service
- Highly available

**Location:**
- Sits on edge of:
  - Amazon VPC
  - AWS public zone
  - Internet

**Function:**
- Manages traffic between:
  - Amazon VPC
  - AWS public zone
  - Internet

**Why Only One:**
- Reason for one public route table: Internet gateway is per Amazon VPC
- One internet gateway works across all AZs

### Creating New Internet Gateway:

**Steps:**
1. Create new internet gateway
2. Must attach it to Amazon VPC (not automatically attached)
3. Add route to route table to allow traffic to and from internet gateway

**Public Subnet:**
- If you add internet gateway route to subnet: Becomes public subnet
- Now has access to AWS public zone and open internet

---

## Network Access Control Lists (NACLs)

### What Are NACLs?

**Definition:**
- Type of security filter (like firewall)
- Can filter traffic as it enters and leaves subnet

### Attachment:
- Attached at subnet level

**Default Configuration:**
- Default network ACL created for default Amazon VPC
- Associated with all subnets by default

### When NACLs Are Used:

**Traffic Management:**
- Used for traffic entering or leaving subnet
- Associated with subnet (NOT with resources)
- Only manage traffic crossing subnet boundary

### Stateless Characteristic:

**Important - Covered in Domain 2:**
- Network ACLs are stateless
- If you add rule for inbound traffic: Must also add same rule for outbound traffic
- Only see traffic going one way

**Two Rules Required:**
- Allow inbound rule: Must also allow outbound rule
- NACL must explicitly see traffic allowed inbound is also allowed out
- See traffic as two separate streams
- Must have two rules (one for each stream)

---

## Security Groups

### What Are Security Groups?

**Another Security Feature:**
- Unlike network ACLs: NOT attached to subnet
- Attached to Elastic Network Interface (ENI) of AWS resources in subnet

### How They Differ from NACLs:

**Location:**
- Sit at boundary of instance (instead of subnet)

**Rules:**
- Have inbound and outbound rules

**Stateful Characteristic:**
- Security groups are stateful
- If traffic allowed in: Traffic automatically allowed back out
- See both inbound and outbound traffic as part of same stream

---

## Network Address Translation (NAT)

### What is NAT?

**Definition:**
- Network Address Translation
- Process of giving private resource outgoing access to internet

### Internet Gateway Example:

**Static NAT:**
- Internet gateway performs type of NAT called static NAT

**How It Works:**
1. Internet gateway allocates resource with public IPv4 IP address
2. When data/packets leave resource and pass through internet gateway:
   - Gateway switches source IP address from private to public
   - Sends packet on
3. When packet returns:
   - Switches destination address from public back to private

### NAT Gateway Purpose:

**What It Does:**
- Gives private CIDR range outgoing internet access
- Access to AWS public zone

**Traffic Flow:**
- When private resources initiate traffic with NAT gateway: Can receive responses back in
- Outside traffic from internet: CANNOT initiate traffic inbound

**Use Case:**
- Allow private resources access to internet or AWS public zones

**Why Private Service Needs Internet:**
- Most common reason: Software updates

---

## VPC Communication Services

### VPC Peering

**What It Is:**
- Way to link multiple Amazon VPCs together
- Allows direct communications between two isolated sites
- Uses their private IP addresses

**Capabilities:**
- Can span AWS accounts
- Can span Regions
- Data shared is encrypted using AWS global infrastructure

---

## VPC Endpoints

### What Are VPC Endpoints?

**Definition:**
- Gateway objects created inside Amazon VPC
- Similar to internet gateway and NAT gateways
- Allow instances inside Amazon VPC to connect with AWS public services
- Without need of gateway

### Two Types of Endpoints (Know for Exam):

**1. Gateway Endpoints**

**Use:**
- For AWS public services
- Remember: Some AWS services are public services (sit in AWS public zone)

**When to Use:**
- Want to connect to public services like S3 or DynamoDB
- From private instance or subnet
- That does not have access to internet
- Does not have NAT gateway set up

**Services:**
- S3
- DynamoDB

**2. Interface Endpoints**

**Use:**
- For everything else
- Must pick correct endpoint depending on AWS service

**How They Work:**
- Use DNS (not routing with prefix list)
- For all other services besides S3 and DynamoDB

---

## AWS PrivateLink

### What is PrivateLink?

**Definition:**
- VPC endpoint service

**Problem It Solves:**
- Need to expose application to other Amazon VPCs in other AWS accounts
- Does not require VPC peering or other gateways

---

## VPN Connection

### What is VPN?

**Definition:**
- Hardware Virtual Private Network connection
- Between on-premises data center and Amazon VPC
- Use AWS as extension of current data center or environment

**Remember:**
- From earlier lesson: This is called hybrid environment

### AWS VPN Service:

**What It Offers:**
- Service to configure hardware VPN
- Highly available virtual private connection
- Between Amazon VPC and on-premises networks

**How It Works:**
- VPNs use public internet as transit route
- For on-premises and Amazon VPC
- Offers fully encrypted route
- From on-premises network to Amazon VPC

---

## AWS Direct Connect

### What is Direct Connect?

**Definition:**
- Dedicated physical connection
- Between on-premises network and AWS

**Exam Keyword:**
- "Dedicated" = keyword for Direct Connect

### VPN vs. Direct Connect:

**VPN:**
- Virtual private connection
- Over public internet

**Direct Connect:**
- Physical piece of fiber
- Running between on-premises network and AWS network
- Physical or cross-connect connection
- Between AWS router and another router

**Infrastructure:**
- AWS has number of Direct Connect locations
- Distributed globally

---

## Amazon Route 53

### DNS Fundamental:

**Need to Know:**
- DNS = Domain Name System

### What is Route 53?

**Definition:**
- AWS's managed DNS product

**Two Main Functions:**
1. Register domains
2. Host zones on managed nameservers

### Service Characteristics:

**Global Service:**
- One single database
- Replicated between Regions
- Globally resilient service

**Resilience:**
- Can tolerate failure of one or more Regions
- Continue to operate

### How DNS Works:

**Purpose:**
- Service used to help discover other services on internet
- Translates addresses:
  - From language computers understand
  - To language humans understand
  - And back again

**Example:**
1. We type: amazon.com
2. Computers use: IP addresses
3. DNS translates: Words → IP addresses
4. Finds location
5. Sends location back
6. Translates: IP address → Words we understand

### Routing Policies:

**For High Availability and Resilience:**
- Failover routing policy
- Weighted routing policy
- Latency routing policy

---

## Edge Services

### Already Covered:
- CloudFront
- Global Accelerator

---

## Exam Preparation Summary

### What You Must Know:

**1. Features and Configurations:**
- How to take advantage of features, controls, and configurations
- To build privacy and security into environments

**2. Connectivity:**
- What you can do to provide connectivity to Amazon VPCs:
  - From internet
  - From on-premises location

**3. When to Use What:**
- When to use VPN
- When to use Direct Connect
- When to use Amazon Route 53
- For different use cases

---

## Critical Exam Concepts

### VPC Basics:
- Virtual private cloud (your data center in cloud)
- Regional service
- Default VPC (one per Region, created by AWS)
- Custom VPC (configured by you, private by default)
- VPC CIDR range defines IP addresses

### Security:
- NACLs: Subnet level, stateless, two rules needed
- Security Groups: Resource/ENI level, stateful, return traffic automatic
- Both control traffic but work differently

### Connectivity Components:
- VPC Router: Highly available, routes between subnets
- Internet Gateway: One per VPC, regional resilient
- NAT Gateway: Gives private resources outgoing internet access
- Route Tables: Control traffic routing

### VPC Communication:
- VPC Peering: Link VPCs together
- VPC Endpoints: Connect to AWS public services without gateway
  - Gateway endpoints: S3, DynamoDB
  - Interface endpoints: Everything else
- PrivateLink: Expose apps to other VPCs without peering

### Hybrid Connectivity:
- VPN: Virtual connection over public internet, encrypted
- Direct Connect: Physical dedicated connection (keyword: "dedicated")

### DNS:
- Route 53: Managed DNS, globally resilient
- Domain registration and zone hosting
- Routing policies for HA (failover, weighted, latency)

### Public vs. Private Subnets:
- Public subnet: Has route to internet gateway
- Private subnet: No direct internet access (can use NAT gateway)

---
# AWS Cloud Practitioner Notes - Task Statement 3.6: Identify AWS Storage Services

## Cloud Storage Fundamentals

### What is Cloud Storage?

**Definition:**
- Cloud computing model that stores data through cloud computing provider
- Provider manages and operates data storage as a service
- Provides agility, global scale, and durability
- Any time, anywhere data access

### How Cloud Storage Works:

**Purchase Model:**
- Purchased from third-party cloud vendor
- Vendor owns and operates data storage capacity
- Delivers over internet
- Pay-as-you-go model

**Vendor Management:**
- Manage capacity
- Manage security
- Manage durability
- Make data accessible to applications all around world

---

## Benefits of Cloud Storage

**Key Benefits:**
1. No hardware or storage to provision
2. On-demand capacity, performance, and retention
3. Storage lifecycle management to move data to lower cost tiers
4. Only pay for storage you need and use

---

## Cloud Storage Requirements

**Critical Requirements:**
- Durability: Ensure data is safe
- Availability: Ensure data is available when needed
- Security: Ensure data is secure

---

## Three Types of Cloud Storage

### Important for Exam:

**1. Object Storage**

**2. File Storage**

**3. Block Storage**

**Each offers:**
- Own advantages
- Own use cases

---

## Object Storage - Amazon S3

### S3 Characteristics:

**Service Type:**
- Global resilient service
- Global storage platform
- Run in every AWS Region

**Data Storage:**
- Data stored in specific Region
- Can be accessed from anywhere

**Service Location:**
- Amazon S3 is public service
- Runs from AWS public zone

### Resilience and Replication:

**Within Region:**
- Data stored in S3 replicated across different AZs in that Region
- Can tolerate failure of an AZ

**Between Regions:**
- Can also replicate data between Regions

### Capacity and Access:

**Storage:**
- Designed to store virtually unlimited amount of data
- **Keyword for exam:** Unlimited amount of data

**Users:**
- Multiple users can access data in S3

---

## S3 Buckets and Objects

### Buckets:

**What They Are:**
- Hold objects like a container

**Naming:**
- Must add globally unique name when creating bucket
- No bucket can have same name as another bucket
- Anywhere in world, any Region

### Objects:

**What They Can Be:**
- Videos
- Pictures
- Files
- Large datasets
- And more

**Size:**
- From 0 bytes to 5 terabytes

---

## S3 Compliance

### Regional Considerations:

**When You Store Objects:**
- S3 bucket is in specific Region
- Laws and rules of that Region apply to S3 bucket

---

## S3 Versioning

### Question: Preventing Accidental Overwrites/Deletes

**Answer: Enable S3 Versioning**

**How It Works:**
- Enable during bucket creation
- Every time you upload object: Automatically creates version
- If accidentally overwrite object: Can still restore previous version using versioning

---

## S3 Features

### Comprehensive Feature Set:

**Organization and Management:**
- Append metadata tags to objects
- Move and store data across S3 storage classes
- Configure and enforce data access controls
- Secure data against unauthorized users
- Run big data analytics
- Monitor data at object and bucket levels
- View storage usage and activity trends across organizations

**Access Methods:**
- Through S3 access points
- Directly through bucket hostname

---

## S3 Storage Classes

### Important for Exam:

**Take time to understand:**
- Different S3 storage classes
- Use cases for each

### Example Question:

**Scenario:**
- Most cost-effective storage class for archives
- Long-term storage
- Need retrieval time of less than 12 hours
- Options: S3 Glacier or S3 Glacier Deep Archive?

**Answer: Amazon S3 Glacier Deep Archive**

**Why:**
- Lowest cost storage class
- Supports long-term retention
- Data can be restored within 12 hours

### Key Understanding:

**S3 as Object Store:**
- If asked to choose object store system: Choose Amazon S3
- S3 IS object store system
- S3 is NOT file system (like Amazon EFS)
- S3 is NOT block storage system (like Amazon EBS)

---

## File Storage - Amazon EFS

### What is File Storage?

**Use Case:**
- Some applications need to access shared files
- Require a file system
- Often supported with Network Attached Storage (NAS) server

### Amazon EFS Characteristics:

**Ideal Use Cases:**
- Large content repositories
- Development environments
- Media stores
- User home directories

**Why Useful:**
- Provides network-based file systems
- Can be mounted with Linux EC2 instances
- Can be used by multiple instances at same time

**Storage Location:**
- Data stored outside Amazon EC2 instance
- Sits inside Amazon VPC
- Provides scaling and self-healing properties

**Access Methods:**
- VPN
- Direct Connect
- VPC Peering

**Lifecycle Policies:**
- Can move data between two different storage classes in Amazon EFS

**Keyword:** Linux = Amazon EFS

---

## Amazon FSx for Windows

### Why It Exists:

**Problem:**
- Amazon EFS is for Linux
- Cannot use Amazon EFS for Windows

**Solution:**
- AWS created FSx for Windows

### FSx for Windows Characteristics:

**What It Is:**
- Fully managed Windows file system share drive
- Supports Server Message Block (SMB) protocol
- Supports Windows Network Technology File System

**Features:**
- Supports Active Directory integration
- Supports Access Control Lists (ACLs)
- Built on Solid State Drive (SSD)
- Highly scalable distributed file system for Windows
- Managed by AWS

**Performance:**
- Can scale up to 10 gigabytes per second
- Millions of IOPS

**Availability:**
- Highly available
- Can be configured for multi-AZ
- Can be accessed from on-premises
- Data backed up daily to S3

---

## Amazon FSx for Lustre

### What is Lustre?

**Definition:**
- Type of parallel distributed file system
- For large-scale computing

**Name Origin:**
- Linux + Cluster = Lustre
- Helps remember it's for Linux instances and cluster (large-scale computing)

### Use Cases - Important for Exam:

**Great For:**
- Machine learning
- High-performance computing
- Sub-millisecond latency

**Specific Workloads:**
- File systems to perform video processing
- Financial modeling
- Design automation
- Anything needing high level of distribution

---

## Block Storage - Amazon EBS

### What is Block Storage?

**Use Case:**
- Enterprise applications like databases
- Require dedicated low-latency storage for each host
- Comparable to:
  - Direct-Attached Storage (DAS)
  - Storage Area Network (SAN)

**Amazon EBS:**
- Provisioned with each virtual server
- Offers ultra-low latency required for high-performance workloads

---

## Storage Types: Instance Store vs. EBS

### Instance Store (Direct-Attached/Local-Attached Storage):

**What It Is:**
- Physical disks directly connected to device
- Directly connected to Amazon EC2 host
- Called Instance Store

**Advantages:**
- Really fast (attached to hardware)

**Issues:**
- If disk fails: Storage can be lost
- If hardware fails: Storage can be lost
- If instance moves between EC2 hosts: Storage can be lost

### Amazon EBS (Network Attached Storage):

**What It Is:**
- Volumes created and attached to EC2 instance over network

**Comparison to Instance Store:**
- Not as fast as Instance Store
- But: Highly resilient
- Separate from instance hardware
- Issues with EC2 host will NOT impact EBS

---

## Ephemeral vs. Persistent Storage

### Ephemeral Storage:

**Definition:**
- Storage that is temporary
- Cannot rely on to be persistent

**Example:**
- Instance Store

### Persistent Storage:

**Definition:**
- Storage that persists

**Example:**
- Amazon EBS

---

## EBS as Block Storage

### How EBS Works:

**Presentation:**
- Volume presented to OS as collection of blocks
- No structure
- Just collection of addressable blocks

**Can Be Mounted:**
- File systems can be created on top of block storage

**Boot Volume:**
- Can boot off EBS volume
- Why most EC2 instances use EBS volume as boot volume
- Stores operating system

---

## EBS Volume Types

### Question: Best Volume for Most Workloads?

**Answer: General Purpose SSD**

### Four EBS Volume Types:

**1. General Purpose SSD**

**Characteristics:**
- Recommended for most workloads
- Can be used as system boot volume
- Best for development and test environments

**2. Provisioned IOPS SSD**

**Characteristics:**
- For critical business applications
- Require sustained IOPS performance
- Best for large database workloads

**3. Throughput Optimized HDD**

**Characteristics:**
- For streaming workloads
- Requiring consistent, fast throughput at low price
- Great for:
  - Big data
  - Data warehouses
  - Log processing
- **Cannot be boot volume**

**4. Cold HDD**

**Characteristics:**
- For throughput-oriented storage
- Large volumes of data infrequently accessed
- Scenarios where lowest storage cost is important
- **Cannot be boot volume**

### EBS Snapshots:

**Purpose:**
- Create point-in-time backup

---

## AWS Storage Gateway

### What is Storage Gateway?

**Definition:**
- Cached file system for AWS
- Service that connects on-premises data center storage to AWS storage service

**Use Cases:**
- Migrate part or all of storage platform to AWS
- Extend storage platform to AWS

**How It Works:**
- Virtual appliance run on on-premises virtualization platform
- Can run on: VMware, ESXi, EC2, etc.
- Download and configure on on-premises location
- Talks to AWS over internet

---

## Three Types of Storage Gateway

### 1. File Gateway

**What It Does:**
- Stores files as objects in S3
- Has local cache for most recently accessed data on-site

**Use Case:**
- Great option for Windows
- Accessible using SMB protocol
- When upload data: Stored in S3

### 2. Volume Gateway

**How It Works:**
- Configured same way as File Gateway
- Download virtual machine image
- Access volumes (not file shares)
- Volumes accessed over iSCSI protocol

**iSCSI:**
- Internet Small Computer Systems Interface
- Internet protocol-based storage networking standard
- Links data storage facilities
- Provides block-level access to storage devices
- Carries SCSI commands over TCP/IP network
- Generally used with SAN products
- Network Attached Storage
- Works great with servers

**Two Options:**

**a) Gateway Stored Volumes:**
- Store all data on volume gateway appliance itself
- Snapshots taken into AWS and stored on S3
- Great when you want:
  - Data on-premises
  - Snapshots and backups in S3

**b) Gateway Cached Volumes:**
- Store primary copies of data in AWS
- Downloads and caches frequently accessed data on volume gateway itself

### 3. Virtual Tape Library (VTL) Gateway

**What It Does:**
- Present virtual tape library over iSCSI
- To any compatible backup software

**Characteristics:**
- Very high administrative overhead
- Costly
- Should be stored off-site for disaster recovery and best practices
- Presents virtual tape drive
- Stored in S3
- Can use for migration of data into AWS over period of time

---

## Storage Backups

### Importance:

**Critical For:**
- Ensure data is protected
- Ensure data is accessible

**Challenge:**
- Keeping up with increasing capacity requirements

**Cloud Storage Benefits:**
- Low cost
- High durability
- Extreme scale
- For backup and recovery solutions

---

## Amazon S3 for Backups

### Storage Classes:

**Full Range Available:**
- Trade-offs between:
  - Price
  - Durability
  - Performance
  - Speed of access

**Each Storage Class Offers:**
- Different cost
- Different performance
- Different retrieval speed
- Different resilience

**Why Great Choice:**
- Low-cost storage for backups

### S3 Object Lifecycle Management:

**Embedded Data Management Policies:**
- Automatically migrate data to lower cost tiers
- Based on frequency or time settings

### Archive Vaults:

**Glacier and Glacier Deep Archive:**
- Can be created to comply with legal or regulatory requirements

**Benefits:**
- Tremendous scale possibilities
- Industries that benefit:
  - Financial services (high volumes of data, long-term retention needs)
  - Healthcare (high volumes of data, long-term retention needs)
  - Media (high volumes of data, long-term retention needs)

---

## AWS Backup

### What is AWS Backup?

**Definition:**
- Fully managed service
- Helps centralize and automate data protection
- Meet compliance requirements
- Across AWS services and on-premises

### Capabilities:

**Configuration:**
- Configure backup policies
- Monitor activity for AWS resources in one place

**Automation:**
- Automate backup tasks
- Consolidate backup tasks
- Previously performed service by service

**Simplification:**
- Removes need to create custom scripts
- Removes need for manual processes

---

## Exam Preparation Summary

### Storage Service Variations:

**Vary In:**
- Use cases
- Functionality
- Optimizations
- Management
- And more

### What You Should Understand:

**1. How Services Work:**
- Not only how services operate
- Not only their limitations
- But also their actual usage

**2. Communication:**
- How services communicate
- How they might work with each other
- How they fit into types of architectures you will build

---

## Key Exam Concepts

### Object Storage (S3):
- Public service, global resilient
- Unlimited data (keyword)
- Buckets (containers) and objects (0 bytes to 5 TB)
- Versioning prevents accidental overwrites/deletes
- Multiple storage classes (Glacier Deep Archive = lowest cost)
- Object store (not file system, not block storage)

### File Storage:
- **EFS:** Linux, network-based, multi-instance access
- **FSx for Windows:** Windows, SMB, Active Directory
- **FSx for Lustre:** Linux, HPC, machine learning, sub-millisecond latency

### Block Storage (EBS):
- Network attached, persistent
- Instance Store: Fast but ephemeral (temporary)
- Four volume types:
  - General Purpose SSD (most workloads, can boot)
  - Provisioned IOPS SSD (critical apps, databases)
  - Throughput Optimized HDD (streaming, cannot boot)
  - Cold HDD (infrequent access, cannot boot)

### Storage Gateway:
- Connects on-premises to AWS
- Three types:
  - File Gateway (files as objects in S3)
  - Volume Gateway (iSCSI volumes)
  - VTL Gateway (virtual tape library)

### Backups:
- S3 for low-cost backups
- Lifecycle policies for automatic tiering
- Glacier/Deep Archive for archives
- AWS Backup for centralized, automated protection

---

# AWS Cloud Practitioner Notes - Task Statement 3.7: Identify AWS AI, ML, and Analytics Services

## Machine Learning and AI Fundamentals

### What is Machine Learning?

**Definition:**
- Science of developing algorithms and statistical models
- Computer systems use to perform tasks without explicit instructions
- Relies on patterns and inference instead
- Uses ML algorithms to process large quantities of historical data
- Identifies data patterns
- Predicts outcomes more accurately from given input dataset

**Example:**
- Train medical application to diagnose cancer from x-ray images
- By storing millions of scanned images
- And corresponding diagnoses

### What is Artificial Intelligence?

**Definition:**
- Field of computer science dedicated to solving cognitive problems
- Commonly associated with human intelligence
- Such as:
  - Learning
  - Problem solving
  - Pattern recognition

---

## Three Levels of ML Services in AWS

### For Workloads in AWS:

**Three Different Levels:**
1. Artificial Intelligence Services
2. Machine Learning Services
3. Machine Learning Frameworks and Infrastructure Services

### Use Cases:
- Anomaly detection
- Fraud detection
- Customer churn
- Content personalization
- Recommendation engine

---

## Level 1: AI Services

### What They Provide:

**Fully Managed Services:**
- Quickly add ML capabilities to workloads using API calls
- Build powerful, intelligent applications

**Capabilities:**
- Computer vision
- Speech
- Natural language
- Chatbots
- Predictions
- Recommendations

### Based On:
- Pre-trained machine learning models
- Automatically trained machine learning models
- Deep learning models
- **Don't need machine learning knowledge to use them**

---

## AI Services - Specific Services

### Know These at High Level:

**Amazon Translate:**
- Translate or localize text content

**Amazon Polly:**
- Text-to-speech conversion

**Amazon Lex:**
- Building conversational chatbots

**Amazon Rekognition:**
- Add image and video analysis to applications

**Instruction:**
- Dive deeper into all AI services

---

## Level 2: Machine Learning Services

### What They Provide:

**Managed Services and Resources:**
- For machine learning
- For developers, data scientists, and researchers

### Amazon SageMaker

**Focus Service for This Level:**

**What It Does:**
- Enables developers and data scientists to:
  - Quickly and easily build ML models
  - Train ML models
  - Deploy ML models
  - At any scale

**Instruction:**
- Dive deeper into SageMaker

---

## Amazon CodeWhisperer

### New ML Service:

**What It Is:**
- Machine learning-powered code generator
- Provides code recommendations in real time
- Can scan code to highlight and define security issues

**Exam Note:**
- Probably will not appear on exam for few months
- But included for awareness

---

## Level 3: ML Frameworks and Infrastructure

### Open-Source Frameworks Available:

**Can Use:**
- TensorFlow
- PyTorch
- Apache MXNet

### Deep Learning AMI and Deep Learning Containers:

**Characteristics:**
- Have multiple ML frameworks pre-installed
- Optimized for performance
- Ready to be launched on powerful ML-optimized compute infrastructure

**Example Infrastructure:**
- Amazon EC2 P3 instances
- Amazon EC2 P3dn instances
- Provides boost of speed and efficiency to ML workloads

---

## Amazon Machine Learning

### Data Sources:

**Can Create ML Models Based On Data Stored In:**
- S3
- Amazon Redshift
- Amazon RDS

### Example Use Cases:

**AI Services:**
- Sentiment analysis of customer reviews on retail website

**Managed ML Services:**
- Build custom model using own data
- Predict future sales

---

## Example Exam Question - AI Services

### Question:

**Scenario:**
- Which AWS service adds visual analysis features to application?
- To search, verify, and organize potentially millions of images?

### Analysis:

**First Recognition:**
- Looking for AI Services level service

**Possible Confusion:**
- First thought might be Amazon SageMaker
- But remember: SageMaker is ML Services level service

**Correct Answer: Amazon Rekognition**

**Why:**
- Can add image and video analysis to applications
- Provide image or video to Rekognition API
- Service can identify:
  - Objects
  - People
  - Text
  - And more

---

## Data Analytics Fundamentals

### What is Data Analytics?

**Definition:**
- Converts raw data into actionable insights

**Benefits:**
- Helps companies gain more visibility
- Deeper understanding of processes and services
- Detailed insights into customer experience
- Detailed insights into customer problems
- Connects insights with actions to:
  - Create personalized customer experiences
  - Build related digital products
  - Optimize operations
  - Increase employee productivity

---

## Amazon Athena

### What is Athena?

**Definition:**
- Interactive query service
- Analyze and query data stored in S3
- Using standard SQL

### Serverless Characteristics:

**Why Considered Serverless:**
- Do not have to provision anything
- Pay per query or per terabyte scanned
- No need to set up complex Extract, Transform, Load (ETL) processes
- Works directly with data stored in S3

### Use Cases:

**Great For:**
- Query log files
- Generate reports
- Analyze cost and usage reports stored in S3
- Run queries on clickstream data

---

## Amazon Macie

### Exam Tip - PII Recognition:

**If Question Asks:**
- Which AWS service helps with Personally Identifiable Information (PII)?
- **Choose Macie**

**Memory Aid:**
- Macie has an "I"
- PII has an "I"

### What is PII?

**Definition:**
- Personal data used to establish individual's identity

**Includes:**
- Name
- Home address
- Email address
- Social Security number
- Driver's license number
- Passport number
- Date of birth
- Bank account information
- Credit card information
- And more

**Why Important:**
- Data needs to be kept secure
- So it is not used or exploited

### What Macie Does:

**AWS Security Service:**
- Uses machine learning to:
  - Discover sensitive data stored in S3
  - Classify sensitive data stored in S3
  - Protect sensitive data stored in S3
- Uses AI to recognize if S3 objects contain sensitive PII data

**Features:**
- Provides dashboards
- Provides reports
- Provides alerts
- Works directly with data stored in S3
- Can analyze AWS CloudTrail logs

### Exam Remember:
- **Athena:** Query service
- **Macie:** Security service (uses ML and AI to protect PII)

---

## Athena vs. Redshift

### Athena Characteristics:

**What It Does:**
- Can query huge datasets in S3
- No preparation needed
- Only pay for data that is queried

**Schema Differences:**

**Regular Databases:**
- Must create table structure in advance
- Must create data structure in advance (schema)
- Once you have schema: Put data into schema
- Schema cannot be easily changed after creation

**Athena:**
- Data stays in S3 in whatever format it's put in
- Supports multiple data formats:
  - Parquet
  - XML
  - JSON
  - CSV
  - And more

---

## Amazon Redshift (Review)

### Characteristics (Covered Earlier):

**What It Is:**
- Petabyte-scale data warehousing solution from AWS
- Column-based database engine
- For analytical workloads
- Designed for Online Analytical Processing (OLAP)

**Architecture:**
- Uses cluster architecture
- Unloads and uploads data to S3

**Data Sources:**
- Can accept data from:
  - DynamoDB
  - DMS (Database Migration Service)
  - Other databases
  - Amazon Kinesis

### Redshift Spectrum:

**What It Does:**
- Perform queries directly against S3

**Differences from Athena:**
- With Redshift Spectrum: Must have Redshift cluster
- Do NOT need to load data into Redshift
- Can simply query directly from S3

**Athena Comparison:**
- Athena is serverless
- No instance to provision

---

## Amazon Kinesis

### What is Kinesis?

**Definition:**
- Processes and analyzes streaming data at any scale
- Fully managed service

**Capabilities:**
- Ingest real-time data:
  - Video
  - Audio
  - Application logs
  - Website clickstreams
  - IoT data
- For machine learning, analytics, and other applications

**Keyword for Exam:** Real-time = Kinesis

### Example Use Case:

**Scenario:**
- Mobile application tracks and streams what users tap on
- Which areas of application are most used
- All of this is streamed
- Few hundred users: Stream of data easy to handle
- Jumps to millions of users: Need Kinesis

**Solution:**
- Use Kinesis to ingest huge quantities of data in real time
- Remember: Fully managed scalable service

### Kinesis Family:

**Dive Deeper Into:**
- Kinesis Data Firehose
- Kinesis Data Analytics

---

## AWS Glue

### What is AWS Glue?

**Definition:**
- Serverless data integration service
- Makes it easy for analytics users to:
  - Discover data
  - Prepare data
  - Move data
  - Integrate data from multiple sources

### Use Cases:
- Analytics
- Machine learning
- Application development

### Why Important:

**First Step:**
- Preparing data to obtain quality results
- First step in analytics or ML project

### Additional Features:

**Productivity and Data Operations Tooling:**
- Authoring
- Running jobs
- Implementing business workflows

**Capabilities:**
- Visually create, run, and monitor ETL pipelines
- Load data into data lakes
- Immediately search and query cataloged data using:
  - Amazon Athena
  - Amazon Elastic MapReduce (EMR)
  - Amazon Redshift Spectrum

---

## Amazon QuickSight

### What is QuickSight?

**Definition:**
- Fast business intelligence service
- Delivers insights to everyone in organization

**Fully Managed Service:**
- Create and publish interactive dashboards
- Includes machine learning insights

---

## Amazon EMR (Elastic MapReduce)

### Example Exam Question:

**Question:**
- Which AWS service supports business intelligence tools?
- Such as Apache Spark
- To perform data transformation workloads and analytics?

**Analysis:**

**Is it QuickSight?**
- No (even though we just mentioned QuickSight with business intelligence)

**Is it Amazon OpenSearch?**
- No
- OpenSearch is type of database and search engine
- Does not support Apache business intelligence tools
- Cannot perform ETL jobs using these tools alone

**Correct Answer: Amazon EMR**

### What is EMR?

**Definition:**
- Web service that enables businesses, researchers, data analysts, and developers
- To process vast amounts of data

**How It Works:**
- Utilizes hosted Apache Hadoop framework
- Running on infrastructure of:
  - Amazon EC2
  - Amazon S3

### Capabilities:

**Can Handle:**
- Securely and reliably handle broad sets of big data use cases

**Use Cases:**
- Machine learning
- Data transformations
- Financial simulation
- Scientific simulation
- Bioinformatics
- Log analysis
- Deep learning

---

## Exam Preparation Summary

### AI Services Level:

**Characteristics:**
- Fully managed
- Pre-trained models
- No ML knowledge needed
- API calls

**Key Services:**
- Translate (text translation)
- Polly (text-to-speech)
- Lex (chatbots)
- Rekognition (image/video analysis)

### ML Services Level:

**Key Service:**
- SageMaker (build, train, deploy ML models)
- CodeWhisperer (code generation, security scanning)

### ML Frameworks Level:

**Components:**
- Open-source frameworks (TensorFlow, PyTorch, MXNet)
- Deep Learning AMI
- Deep Learning Containers
- EC2 P3 instances

### Analytics Services:

**Amazon Athena:**
- Query service for S3
- Serverless
- Standard SQL
- No preparation needed
- Multiple data formats

**Amazon Macie:**
- Security service
- PII detection and protection
- Uses ML and AI
- Works with S3
- Keyword: PII = Macie

**Amazon Kinesis:**
- Real-time streaming data
- Fully managed
- Keyword: Real-time

**AWS Glue:**
- Serverless data integration
- ETL pipelines
- Data preparation

**Amazon QuickSight:**
- Business intelligence
- Interactive dashboards
- ML insights

**Amazon EMR:**
- Big data processing
- Apache Hadoop framework
- Data transformations
- Supports Apache Spark

**Redshift vs. Athena:**
- Redshift: Data warehouse, cluster architecture, OLAP
- Redshift Spectrum: Query S3, needs cluster
- Athena: Serverless, query S3, no cluster needed

---

## Critical Exam Tips

**Service Selection:**
1. Image/video analysis → Rekognition
2. PII protection → Macie
3. Query S3 with SQL → Athena
4. Real-time streaming → Kinesis
5. Build ML models → SageMaker
6. Business intelligence dashboards → QuickSight
7. Big data processing → EMR
8. Data preparation/ETL → Glue

**Keywords:**
- Real-time = Kinesis
- PII = Macie
- Serverless query = Athena
- Data warehouse = Redshift
- Visual analysis = Rekognition

---

# AWS Cloud Practitioner Notes - Task Statement 3.8: Identify Services from Other In-Scope AWS Service Categories

## AWS Monitoring and Observability Services

### Foundation: AWS Well-Architected Framework

**Best Practice:**
- Stay current
- Continual improvement of designs

**Critical for Continuous Improvement:**
- Track and respond to key metrics
- For applications and infrastructure in environment

---

## Key Monitoring Services

### Amazon CloudWatch

**What You Need to Know:**
- How to use CloudWatch to observe what's happening in systems
- Can trigger automated actions based on key metrics using CloudWatch alarms

### AWS X-Ray

**What You Need to Know:**
- How to use X-Ray to observe what's happening in systems

### Amazon EventBridge

**What You Need to Know:**
- How to respond in near real-time to changes in environment

---

## Application Integration Services

### What is Application Integration on AWS?

**Definition:**
- Suite of services that enable communication
- Between decoupled components within:
  - Microservices
  - Distributed systems
  - Serverless applications

### Key Services - Ensure Depth:

**1. Amazon EventBridge**

**2. Amazon Simple Notification Service (SNS)**

**3. Amazon Simple Queue Service (SQS)**

**4. Load Balancing**
- To decouple workloads

---

## Scaling and Visibility

### Why Visibility Matters:

**In Order to Scale:**
- Need visibility

### CloudWatch Basics to Understand:

**Components:**
- CloudWatch metrics
- CloudWatch alarms
- CloudWatch dashboards

### Auto Scaling Integration:

**How Metrics Used:**
- As basis for Amazon EC2 Auto Scaling

**Alarms and EventBridge:**
- Add automations
- Add alerts
- Add remediations
- For scaling events based on alarms created in CloudWatch

**How Alarms Trigger:**
- When metric (such as EC2 CPU utilization) crosses certain threshold
- For defined amount of time

**Important to Know:**
- How to choose what metrics to monitor for scaling
- Very familiar for real world
- Important if interested in AWS Certified Solutions Architect Associate exam

---

## Amazon SQS (Simple Queue Service)

### What is SQS?

**Definition:**
- Queuing system
- Provides fully managed highly available message queues

**Use Case:**
- Inter-process, servers, and services messaging

### How a Queue Works:

**Process:**
1. Have a queue
2. Add message to queue
3. Something else retrieves messages from that queue

**Result:**
- Offers asynchronous way to talk between two components of application

---

## SQS Polling Types

### Two Types of Polling:

**1. Short Polling**

**How It Works:**
- Single API call to check queue for messages
- Get messages available in queue (up to maximum of 10 messages)
- Or get no messages
- Responds immediately to any messages in queue

**Issue:**
- Need to constantly send API calls to check queue for messages
- Consumes lot of API calls

**2. Long Polling**

**How It Works:**
- Same process to check for messages as short polling
- But: Wait for certain amount of time
- That time known as WaitTimeSeconds

**Advantages:**
- More efficient
- Lot less API calls to queue
- Lot less empty API calls

---

## SQS Queue Types

### Two Different Types:

**1. Standard Queues**

**Characteristics:**
- AWS original
- Distributed and scalable to nearly unlimited message volume
- Order of message NOT guaranteed (best-effort)
- Messages guaranteed to be delivered at least once
- Sometimes messages delivered more than once
- Can have duplicate messages
- Can have out of order messages
- Great performance

**2. FIFO Queues (First In, First Out)**

**Why Introduced:**
- To solve Standard queue problems

**Characteristics:**
- Guarantee messages delivered in order received
- Only ever delivered once
- Duplicates do NOT occur

---

## SQS Architecture and Keywords

### When to Use SQS:

**Use Case:**
- Need to decouple two different parts of system

**Exam Keywords:**
- **"Decouple"** → Think SQS
- **"Asynchronous messaging"** → Think SQS
- **"Independent scaling of application"** → Think SQS

**If you see these on exam: Correct answer might be SQS**

---

## Amazon SNS (Simple Notification Service)

### What is SNS?

**Definition:**
- Highly available, durable, and secure pub-sub messaging
- Public AWS service (need network connectivity)
- Accessible wherever network connectivity is available

### What SNS Does:

**Function:**
- Coordinates sending and delivery of messages

### Used By Many AWS Services:

**Examples:**
- **CloudWatch:** When alarms change states
- **Auto Scaling Groups:** Can send notifications to topic when scaling event occurs
- **CloudFormation:** When stacks change state
- And more

---

## Business Application Services

### What Are Business Application Services?

**Definition:**
- Services that improve agility and lower cost

### Amazon Connect

**What It Is:**
- Contact center
- Helps provide customer service for voice and chat
- Across customers and agents

### Amazon SES (Simple Email Service)

**What It Is:**
- Cost-effective, flexible, and scalable email service
- Send mail from within any application
- Send emails securely, globally, and at scale

---

## SNS vs. SES - Exam Question

### Example Question Scenario:

**From AWS Certified Database Specialty Practice Exam:**
- Question trying to choose between Amazon SNS and Amazon SES
- Asking for notification with:
  - Immediate delivery
  - Least effort to configure

**Important Exam Tip:**
- **Ensure you understand exactly what question is asking**
- When reviewing questions and answer responses

**When to Choose SES:**
- Great choice if you need email to come from custom domain

---

## Customer Engagement Services

### What Are They Used For?

**Purpose:**
- Help create best customer experience across entire lifecycle

### AWS Provides:

**1. AWS Activate for Startups**
- Provides eligible startups with:
  - Free tools
  - Resources
  - Content
- Designed to simplify every step of startup journey

**2. AWS IQ**
- Connects you to AWS certified expert
- For hands-on help for AWS projects

**3. AWS Managed Services**
- Infrastructure operations management for AWS
- Enterprise service
- Provides ongoing management of AWS infrastructure

**4. AWS Support**
- Range of plans
- Provide access to tools and expertise
- Support success and operational health of AWS solutions

**AWS Support Plans Provide:**
- 24/7 access to customer service
- AWS documentation
- Technical papers
- Support forums
- Technical support and more resources to plan, deploy, and improve AWS environment
- Can choose support plan for your AWS use cases

---

## Developer Services

### What Are Developer Services?

**Definition:**
- Services and tools designed to help developers:
  - Practice DevOps
  - Deliver
  - Deploy

### AWS Developer Services:

**List of Services:**
- AWS AppConfig
- AWS Cloud9
- AWS CloudShell
- AWS CodeArtifact
- AWS CodeBuild
- AWS CodeCommit
- AWS CodeDeploy
- AWS CodePipeline
- AWS CodeStar
- AWS X-Ray

**Question to Consider:**
- How familiar are you with these services?
- Ensure you dive deeper

---

## End-User Computing Services

### What Are They?

**Purpose:**
- Provide secure access to applications and desktops needed

### AWS Services:

**1. Amazon AppStream 2.0**
- Fully managed application streaming service
- Provides users with instant access to desktop applications from anywhere

**2. Amazon WorkSpaces**
- Helps provision virtual cloud-based desktops for users (known as WorkSpaces)
- Support for:
  - Microsoft Windows
  - Amazon Linux
  - Ubuntu Linux

**3. Amazon WorkSpaces Web**
- On-demand, fully managed, Linux-based service
- Designed to facilitate secure browser access to:
  - Internal websites
  - Software-as-a-service applications

---

## Front-End Web and Mobile Services

### Purpose:
- Help developers develop workflows
- Deliver and deploy securely

### AWS Amplify

**What It Is:**
- Complete solution
- Lets front-end web and mobile developers:
  - Easily build
  - Ship
  - Host full-stack applications on AWS

### AWS AppSync

**What It Provides:**
- Robust, scalable GraphQL interface for application developers
- Combine data from multiple sources:
  - Amazon DynamoDB
  - AWS Lambda
  - HTTP APIs

---

## IoT Services

### What Are IoT Services Used For?

**Purpose:**
- Help securely connect and manage devices
- Collect and analyze device data
- Build and deploy solutions

### AWS IoT Core

**What It Provides:**
- Device software
- Can help integrate IoT devices into AWS IoT-based solutions

### AWS IoT Greengrass

**What It Is:**
- Software that extends cloud capabilities to local devices

**Capabilities:**
- Collect and analyze data closer to source of information
- React autonomously to local events
- Communicate securely with each other on local networks
- Local devices can also:
  - Communicate securely with AWS IoT Core
  - Export IoT data to AWS

---

## Task Statement Summary

### What You Need to Ensure:

**1. Service Selection:**
- Can choose appropriate service for requirements and use cases

**2. Support Options:**
- Choose appropriate support options for business

---

## Exam Preparation Summary

### Monitoring and Observability:
- **CloudWatch:** Metrics, alarms, dashboards, trigger automated actions
- **X-Ray:** Observe system behavior
- **EventBridge:** Near real-time responses to environment changes

### Application Integration:
- **SQS:** Queuing, decoupling, asynchronous messaging
  - Standard: Nearly unlimited, best-effort order, possible duplicates
  - FIFO: Ordered, no duplicates
  - Keywords: decouple, asynchronous messaging, independent scaling
- **SNS:** Pub-sub messaging, coordinates sending/delivery
- **Load Balancing:** Decouple workloads

### Auto Scaling:
- Based on CloudWatch metrics
- Alarms trigger when thresholds crossed
- EventBridge for automation and alerts
- Know how to choose metrics for scaling

### Business Applications:
- **Amazon Connect:** Contact center (voice/chat)
- **Amazon SES:** Email service, custom domains

### Customer Engagement:
- **AWS Activate:** For startups
- **AWS IQ:** Connect to AWS certified experts
- **AWS Managed Services:** Infrastructure operations management
- **AWS Support:** 24/7 access, documentation, technical papers

### Developer Services:
- Multiple Code* services (CodeBuild, CodeCommit, CodeDeploy, CodePipeline, etc.)
- AWS Cloud9, CloudShell
- AWS X-Ray

### End-User Computing:
- **AppStream 2.0:** Application streaming
- **WorkSpaces:** Virtual desktops
- **WorkSpaces Web:** Secure browser access

### Front-End/Mobile:
- **AWS Amplify:** Full-stack application development
- **AWS AppSync:** GraphQL interface, combine data sources

### IoT:
- **AWS IoT Core:** Connect and manage devices
- **AWS IoT Greengrass:** Extend cloud to local devices, analyze data at edge

---

## Critical Exam Concepts

**Keywords to Remember:**
- Decouple, asynchronous messaging → SQS
- Pub-sub messaging → SNS
- Real-time responses → EventBridge
- Monitoring metrics → CloudWatch
- Custom domain email → SES

**Service Categories:**
- Understand what category each service belongs to
- Know use cases for each
- Be able to select appropriate service for scenario

**Support and Engagement:**
- Know different AWS support options
- Understand customer engagement services
- Know when to use each
---

## Domain 3 Complete - Summary

### Eight Task Statements Covered:

**3.1: Methods of Deploying and Operating**
- Access methods (Console, CLI, SDKs, IaC)
- Deployment models (public, private, hybrid, multi-cloud)
- Connectivity (VPN, Direct Connect, Internet)
- Public vs private AWS services

**3.2: AWS Global Infrastructure**
- Regions, Availability Zones, Edge Locations
- Resilience levels (global, regional, AZ)
- CloudFront vs Global Accelerator

**3.3: Compute Services**
- EC2 (instance types, categories, metadata)
- Containers (ECS, EKS)
- Lambda (serverless, FaaS)
- Load balancers and auto scaling

**3.4: Database Services**
- RDS (managed, multi-AZ, read replicas)
- Aurora (cluster, serverless, global)
- DynamoDB (NoSQL)
- Redshift (data warehouse)
- Migration tools (DMS, Snow Family, DataSync)

**3.5: Network Services**
- VPC (subnets, route tables, internet gateway)
- NACLs vs Security Groups
- NAT Gateway, VPC Peering, VPC Endpoints
- VPN vs Direct Connect
- Route 53 (DNS)

**3.6: Storage Services**
- S3 (object storage, storage classes)
- EBS (block storage, volume types)
- EFS and FSx (file storage)
- Storage Gateway

**3.7: AI/ML and Analytics**
- AI Services (Rekognition, Translate, Polly, Lex)
- ML Services (SageMaker)
- Analytics (Athena, Macie, Kinesis, Glue, QuickSight, EMR, Redshift)

**3.8: Other In-Scope Services**
- Monitoring (CloudWatch, X-Ray, EventBridge)
- Application Integration (SQS, SNS)
- Business Applications (Connect, SES)
- Customer Engagement (Support, IQ, Managed Services)
- Developer Services
- End-User Computing
- Front-End/Mobile
- IoT
