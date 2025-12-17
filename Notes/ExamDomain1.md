# AWS Cloud Practitioner Notes - Domain 1: Cloud Concepts

## Module Overview

**Domain 1 Components:**
- Cloud concepts covering AWS, benefits, design principles, migration, and economics
- Divided into 4 task statements

**Task Statements:**
1. Task Statement 1.1: Define the benefits of the AWS Cloud
2. Task Statement 1.2: Identify design principles of the AWS Cloud
3. Task Statement 1.3: Understand the benefits of and strategies for migration to the AWS Cloud
4. Task Statement 1.4: Understand concepts of cloud economics

**What Each Task Statement Covers:**
- Task Statement 1: AWS fundamentals, what is AWS, what makes cloud computing "cloud"
- Task Statement 2: Design principles for AWS, AWS Well-Architected Framework, best practices, core strategies for architecting systems
- Task Statement 3: Reducing database costs, improving availability during migration, AWS storage services, understanding data types and appropriate data stores
- Task Statement 4: Cloud economics concepts, methods for running cost-optimized environments

---

## Task Statement 1.1: Define the Benefits of the AWS Cloud

### What is AWS?

**AWS Definition (per Amazon):**
- Amazon Web Services is the world's most comprehensive and broadly adopted cloud
- Offers over 200 fully featured services from data centers globally
- Used by millions of customers including fastest growing startups, largest enterprises, and leading government agencies
- Purpose: Lower costs, become more agile, innovate faster

**Key AWS Benefits:**
- Powers infrastructure
- Increases agility
- Lowers costs

### What is Cloud Computing?

**Five Criteria for Cloud Computing:**

**1. On-Demand Self-Service**
- Ability to provision compute features/capabilities on demand when needed
- Resources include: servers, databases, network, storage, and more
- Must be able to provision without human intervention or interaction
- AWS provides this through:
  - Console
  - Command line
  - Application Programming Interfaces (APIs)
- No need to request or ask anyone - with correct permissions, you can start building immediately

**2. Network Connectivity**
- Must have network connectivity to access and provision needed resources
- AWS provides access through:
  - AWS Management Console
  - Command line
  - HTTP
  - HTTPS
  - VPN
  - SSH
  - And more

**3. Resource Pooling**
- Definition: AWS provides pooled resources to serve multiple different AWS customers
- AWS has thousands of servers, databases, and more available for on-demand provisioning
- Resources are available to all customers
- Key characteristic: Customers do not know the exact location of pooled resources
- Example with EC2:
  - You can select the AWS Region
  - AWS chooses any data center in that Region
  - You can choose Availability Zone if desired (will be discussed later)
- AWS procures thousands of resources for customers
- Uses economies of scale:
  - Larger scale of resources allows AWS to offer economies at scale to customers
  - AWS passes savings to customers
  - Provides resources needed to scale and grow
  - More detail covered in cost optimization section

**4. Elasticity**
- Definition: The ability to scale with demand
- When demand increases: scale up AWS resources
- When demand decreases: scale resources back down
- Will be discussed throughout the course

**5. Monitored and Billed Resource Usage**
- Resource usage in AWS accounts can be monitored and billed
- Benefits:
  - No longer pre-provisioning or procuring storage, servers, compute, etc.
  - No need to estimate demands
  - Services monitored for usage and billed accordingly
  - Scale resources to meet demand instead of being over- or under-provisioned
- **Biggest cost optimization benefit: Only pay for what you use**

### AWS Global Infrastructure

**Overview:**
- Collection of smaller groupings of infrastructure
- Connected by a global high-speed network
- Allows design of resilient and highly available systems
- Will be covered in depth in Domain 3

**Key Components to Understand:**
- AWS Regions
- Availability Zones
- Edge locations

---

## High Availability, Fault Tolerance, and Disaster Recovery

### High Availability

**Definition:**
- Way to design systems to keep them up and running and providing service as often as possible
- Designed so if a system component fails, failure can be replaced or fixed quickly
- Maximizes system's online time

**Important Clarifications:**
- Does NOT stop failures from happening
- Does NOT mean zero downtime or outages
- Responds to failures to fix them as soon as possible

**Example Scenario:**
- Single server running application used by employees
- If server goes down: employees cannot work (outage occurs)
- High availability design options:
  - Option 1: Quickly spin up new server to failover to
  - Option 2: Run two servers - one active, one standby
- If server goes down with two-server setup:
  - Failover to second server
  - Employees may need to log back in
  - Brief downtime may occur (acceptable in high availability design)

**Goal of High Availability:**
- Reduce outages
- Stay operational
- Fast, automatic recovery is best
- Usually has some downtime, even if very brief

### Fault Tolerance

**Definition:**
- The actual ability of a system to keep operating in the event of a failure
- System continues operating even when one or more components fail
- Must continue to operate through faults

**Key Difference from High Availability:**
- Fault tolerance continues operating during failure (no downtime)
- High availability responds to failure (may have brief downtime)

**Example Scenario:**
- Design uses two active servers serving one application
- If one server goes down:
  - Second server already active
  - Continues serving employees
  - NO downtime occurs

**Characteristics:**
- Operates to minimize failures
- Continues to operate through failure
- Usually more expensive than high availability designs

### Disaster Recovery

**How It Differs:**
- High availability and fault tolerance: Design systems to operate through disaster
- Disaster recovery: Plan for and respond to disasters

**Key Points:**
- Crucial to have a disaster recovery plan
- Worst time to recover is in the middle of a disaster
- Requires:
  - Pre-planning
  - Steps to complete disaster recovery process
- When disaster occurs: already have plan to recover systems quickly

**Course Coverage:**
- Will continue discussing high availability, fault tolerance, and disaster recovery throughout course
- Will cover which AWS services are good options for one, both, or all three

---

## Elasticity and Scaling

### Scaling Overview

**Definition:**
- The ability of a system to increase or decrease based on load
- Systems scale when they need to grow or shrink depending on load
- Involves adding or removing resources to/from a system

**Two Types of Scaling:**

### 1. Vertical Scaling

**Definition:**
- Resizing instances to a larger size

**Example Scenario:**
- Have an Amazon EC2 instance of particular size
- Instance cannot keep up with increased demand
- Instance runs slowly or crashes (worst case)
- Solution: Resize to larger instance (e.g., T2 micro → T2 medium or larger)
- Adds more CPU and memory to handle increased demand

**Issues with Vertical Scaling:**
- Small disruption occurs (instance needs reboot when resized)
- Cost increases with larger instance sizes
- Should review AWS Well-Architected Framework cost optimization pillar
- Important to right-size instances from the beginning

**Benefits of Vertical Scaling:**
- Usually no application modifications needed
- Works for all applications

### 2. Horizontal Scaling

**Definition:**
- Adding more instances of the same size to handle load

**Design:**
- Instead of increasing instance size, add more instances
- One copy of application per instance
- Use load balancer to distribute load across instances
- Designed to fix issues with vertical scaling

**Considerations:**

**Session Management:**
- Issue: Don't want to interrupt customer sessions
- Single server: All sessions stored on one server
- Multiple servers: Sessions can shift between instances
- Load balancer sends requests to different servers
- Solution: Use sticky sessions feature
- Prevents losing session when switching between servers
- Works when scaling in or scaling out

**Cost Benefits:**
- Usually less expensive than vertical scaling
- Uses smaller, cheaper instance sizes

### Elasticity

**Definition:**
- Using automation along with horizontal scaling to match capacity and supply with demand

**Key Concept:**
- Demand is rarely linear - usually increasing and decreasing
- Elasticity allows capacity to increase and decrease to meet ever-changing demand

**AWS Tools for Elasticity:**
- Launch configurations
- Auto scaling

**How It Works:**
- Scale out systems to match capacity to demand
- As demand increases: add additional resources
- As demand decreases: scale back in to fewer servers or even no servers

**Benefits:**
- Optimizes for performance efficiency
- Optimizes for operational excellence
- Optimizes for cost
- All are pillars of AWS Well-Architected Framework

---

## Exam Tips Summary

**Scaling Types:**
- **Vertical scaling:** Larger instance size
- **Horizontal scaling:** More instances of same size
- **Elasticity:** Automation + horizontal scaling to match capacity to demand
# AWS Cloud Practitioner Notes - Task Statement 1.2: Identify Design Principles of AWS

## AWS Well-Architected Framework Overview

### What is the AWS Well-Architected Framework?

**Definition:**
- AWS's best practices and core strategies for architecting systems in the cloud
- Helps design, build, and operate reliable, secure, efficient, and cost-effective systems
- Increases likelihood of success

### Six Pillars of the Well-Architected Framework:
1. Operational Excellence
2. Security
3. Reliability
4. Performance Efficiency
5. Cost Optimization
6. Sustainability

### General Design Principles (Apply Across All Pillars)

**Core Design Principles to Facilitate Good Design:**
1. **Stop guessing your capacity**
   - Use auto scaling to ensure supply meets demand

2. **Test systems at production scale**

3. **Automate your architecture**
   - Makes experimentation easier

4. **Allow for evolutionary changes**
   - Use data to make needed changes

5. **Improve through game days**
   - Run tests to see systems at production level

### AWS Well-Architected Tool

**Purpose:**
- Reviews your workloads
- Compares workloads to latest AWS best practices for architectural design
- Best practices come directly from AWS Well-Architected Framework

**Resources:**
- Links provided for AWS Well-Architected Framework
- Links provided for the tool for deeper dive

---

## Pillar 1: Operational Excellence

### Definition:
- The ability to support development and run workloads effectively
- Gain insight into operations
- Continuously improve supporting processes and procedures to deliver business value

### Five Design Principles for Operational Excellence:
1. **Perform operations as code**
2. **Make frequent, small, reversible changes**
3. **Refine operations procedures frequently**
4. **Anticipate failure**
5. **Learn from all operational failures**

---

## Pillar 2: Security

### Definition:
- Encompasses the ability to protect data, systems, and assets
- Take advantage of cloud technologies to improve security

### Seven Design Principles for Security in the Cloud:
1. **Implement a strong identity foundation**
2. **Maintain traceability**
3. **Apply security at all layers**
4. **Automate security best practices**
5. **Protect data in transit and at rest**
6. **Keep people away from data**
7. **Prepare for security events**

---

## Pillar 3: Reliability

### Definition:
- Encompasses the ability of a workload to perform its intended function correctly and consistently when expected to
- Includes ability to operate and test the workload through its total lifecycle

### Five Design Principles for Reliability in the Cloud:
1. **Automatically recover from failure**
2. **Test recovery procedures**
3. **Scale horizontally to increase aggregate workload availability**
4. **Stop guessing capacity**
5. **Manage change in automation**

---

## Pillar 4: Performance Efficiency

### Definition:
- Includes the ability to use computing resources efficiently to meet system requirements
- Maintain that efficiency as demand changes and technologies evolve

### Five Design Principles for Performance Efficiency in the Cloud:
1. **Democratize advanced technologies**
2. **Go global in minutes**
3. **Use serverless architectures**
4. **Experiment more often**
5. **Consider mechanical sympathy**

---

## Pillar 5: Cost Optimization

### Definition:
- Includes the ability to run systems to deliver business value at the lowest price point

**Note:** Will be covered in detail under Domain 4: Billing, Pricing, and Support

---

## Pillar 6: Sustainability

### Definition:
- Focuses on environmental impacts
- Especially energy consumption and efficiency
- Important levers for architects to inform direct action to reduce resource usage

### Six Design Principles for Sustainability in the Cloud:
1. **Understand your impact**
2. **Establish sustainability goals**
3. **Maximize utilization**
4. **Anticipate and adopt new, more efficient hardware and software offerings**
5. **Use managed services**
6. **Reduce the downstream impact of your cloud workloads**

---

## Important Exam Considerations

### Why This Matters:
- Provides solid basis for understanding AWS
- Fundamental concepts are beneficial going into exam
- Important in real world, for this exam, AND for AWS Certified Solutions Architect Associate certification

### What to Expect on Exam:
- Questions asking which design principles for specific requirements or use cases
- Questions about which principles to choose when designing systems or solutions in AWS

### What You Need to Know:
- Understand best practices for ALL pillars
- Know how to design for failures
- Understand decoupling components (reinforces service-oriented architecture design principle)
- Implement elasticity using auto scaling
- Understand security
- Understand parallelization (necessary for building highly scalable applications in AWS)

---

## Key Concepts and Definitions

### Parallelization:
**Definition:**
- Similar to decoupling
- How to divide a job into its simplest form
- Distribute load to multiple components to handle demand

**Example:**
- Breaking down large datasets into smaller chunks
- Chunks can be processed simultaneously
- Provides faster processing times

### Thinking Parallel vs. Decoupling:
- Similar concepts but different applications
- Parallelization: Breaking down tasks for simultaneous processing
- Decoupling: Separating components for independent operation

---

## Advantages of AWS (Revisited)

**Key Benefits:**
- Ability to focus on services and designs (NOT servers and hardware)
- Fast implementation and launching of resources

---

## Action Items for Exam Preparation:

1. **Read the AWS Well-Architected Framework documentation**
2. **Build solutions using these principles**
3. **Ensure understanding of:**
   - Designing for failures
   - Decoupling components
   - Implementing elasticity
   - Security practices
   - Parallelization techniques
4. **Review best practices for all six pillars**

---
# AWS Cloud Practitioner Notes - Task Statement 1.3: Understand Benefits of and Strategies for Migration to AWS

## AWS Cloud Adoption Framework (CAF)

### What is AWS Cloud Adoption Framework?

**Key Distinction:**
- Different from AWS Well-Architected Framework (covered in previous lesson)

**Definition:**
- Provides comprehensive approach to cloud
- Identifies specific organizational capabilities for successful cloud transformations
- Capabilities provide best practice guidance
- Helps improve cloud readiness

### Six Perspectives of AWS CAF

**Capabilities are grouped into six perspectives:**
1. **Business**
2. **People**
3. **Governance**
4. **Platforms**
5. **Security**
6. **Operations**

### How to Use AWS CAF

**Three Main Uses:**
1. Identify and prioritize transformation opportunities
2. Evaluate and improve your cloud readiness
3. Iteratively evolve your transformation roadmap

### Benefits of Using AWS CAF

**Four Key Benefits:**

1. **Reduce business risk**
   - Through improved reliability
   - Increased performance
   - Enhanced security

2. **Increase operational efficiency**
   - Reduce costs
   - Increase productivity

3. **Grow business**
   - Create new products and services
   - Reach new customers
   - Reach new markets

4. **Improve performance**
   - Improve sustainability
   - Improve transparency

---

## Cloud Adoption Strategies

### Stages of Adoption

**Organizations can be in different stages when migrating to AWS:**

**1. Project Stage**
- Evaluating if migrating to AWS meets specific requirements and needs

**2. Foundation Stage**
- Migration to AWS begins
- Move a few production applications to AWS
- Deploy initial framework for landing zone to non-production environment

**3. Migration Stage**
- Define roles for cloud operations
- Establish Cloud Center of Excellence (CCOE)
- Prepare for long-term cloud operations instead of on-premises operations

**4. Reinvention Stage**
- All new projects start in AWS

**Important Note:**
- Assessment of where you and your organization sits is completed before migration begins
- Determines which stage of adoption you are at

---

## Seven Migration Strategies (The 7 R's)

### 1. Retire
**Use Case:**
- Applications you want to decommission or retire

### 2. Retain
**Use Case:**
- Applications you want to keep in source environment
- Applications that are not ready to migrate

### 3. Rehost (Lift and Shift)
**Use Case:**
- Migrate applications without making any changes to the application

### 4. Relocate
**Use Case:**
- Large number of servers made up of one or more applications

### 5. Repurchase (Drop and Shop)
**Use Case:**
- Applications with different version or product
- Provides more value than existing infrastructure

### 6. Replatform (Lift, Tinker, and Shift)
**Use Case:**
- Applications that need some level of optimization
- To operate efficiently or take advantage of AWS capabilities

### 7. Refactor (Re-architect)
**Use Case:**
- Applications you want to migrate to AWS
- Take full advantage of cloud-native features
- Improve agility, performance, and scalability

---

## AWS Services for Migration

### Exam Focus Areas:
- Know how to identify appropriate migration strategies
- Database replication using AWS Database Migration Service
- AWS Snowball (will be covered in depth in later lesson)

---

## Migration Scenario Examples

### Example 1: Financial Application Migration

**Scenario:**
- Migrating application that stores financial information to AWS
- Requires low latency access
- Data is constantly changing

**Service Options Presented:**
- Amazon Elastic File System (EFS)
- AWS Snowball Edge
- Amazon Simple Storage Service (S3)
- Amazon Relational Database Service (RDS)

**Analysis:**

**Amazon S3:**
- Always a good choice
- NOT best for low latency requirement
- Sits in public zone
- Located outside Amazon VPC
- Could have more latency

**AWS Snowball Edge:**
- Used for migration when moving large amounts of data into or out of AWS
- Not appropriate for this scenario

**Best Choices: Amazon EFS and Amazon RDS**

**Amazon RDS:**
- Managed database service
- Provides scalable relational database
- Fast performance
- High availability
- Security

**Amazon EFS:**
- Provides scalable file storage with Amazon EC2 instances
- Storage capacity is elastic

---

### Example 2: NoSQL Database Migration

**Scenario:**
- Migrating NoSQL database
- Must ensure database is scalable, fast, and reliable

**Service Options Presented:**
- Amazon S3
- Amazon RDS
- Amazon Redshift
- Amazon DynamoDB

**Correct Answer: Amazon DynamoDB**

**Amazon DynamoDB:**
- Fully managed NoSQL database service
- Provides fast and predictable performance with scalability
- **Keywords for exam:** NoSQL and non-relational = DynamoDB
- **Keyword for exam:** Relational = Amazon RDS
- Key-value and document database
- Stores JSON-type documents

---

### Example 3: Microsoft SQL Server Migration

**Scenario:**
- Need to launch Microsoft SQL Server database in AWS
- Must be cost optimized
- Only standard license for SQL Server required

**Options Presented:**
1. Amazon Aurora database running SQL Server + buy standard license from AWS License Manager Service
2. RDS instance running SQL Server with standard SQL license
3. Launch Amazon EC2 instance, install SQL Server, purchase standard license from Microsoft
4. Use Windows Server with SQL Server Standard AMI (no need to buy or manage own license)

**Correct Answer: Option 4 - Windows Server with SQL Server Standard AMI**

**Explanation:**

**AWS Amazon Machine Images (AMIs):**
- AWS offers multiple AMIs for Amazon EC2 instances
- If launching EC2 instance using Windows AMI:
  - Can choose one bundled with SQL Server Standard
  - Do not need to purchase own license from Microsoft

**Why Not Other Options:**

**Amazon RDS Option:**
- Could work (RDS database instance running SQL Server Standard with license purchase)
- Question asks for cost optimization
- Amazon RDS costs MORE than Amazon EC2 (because it's a managed service)

**Amazon Aurora Option:**
- Aurora only supports MySQL and PostgreSQL
- Does NOT support SQL Server

---

## Data Backups and Storage

### Focus Area:
- Need plan in place to store data once migrated
- Understand cost storage options for AWS storage services

### Amazon S3 Glacier Storage Classes

**Characteristics:**
- Designed to be lowest-cost Amazon S3 storage classes
- Allows archiving large amounts of data at very low cost

**Considerations:**
- Must consider retrieval fees
- Must consider retrieval times

---

## Exam Preparation Summary

**Key Knowledge Areas:**
1. **AWS Cloud Adoption Framework:**
   - Six perspectives
   - How to use it
   - Benefits

2. **Cloud Adoption Stages:**
   - Project
   - Foundation
   - Migration
   - Reinvention

3. **Seven Migration Strategies (7 R's):**
   - Retire
   - Retain
   - Rehost
   - Relocate
   - Repurchase
   - Replatform
   - Refactor

4. **AWS Services for Migration:**
   - Database Migration Service
   - Snowball
   - Storage services (S3, EFS, RDS, DynamoDB, etc.)

5. **Service Selection Criteria:**
   - Know keywords (NoSQL = DynamoDB, Relational = RDS)
   - Understand cost optimization
   - Know latency considerations
   - Understand licensing options

6. **Data Backup and Storage:**
   - Understand cost storage options
   - Know retrieval fees and times for different storage classes

---
# AWS Cloud Practitioner Notes - Task Statement 1.4: Understand Concepts of Cloud Economics

## Shifting Technical Resources from On-Premises

### What AWS Helps You Move Away From:
- On-premises infrastructure management
- Server acquisition and maintenance
- Space management
- Cooling systems
- All other data center operations and requirements

---

## AWS Well-Architected Framework - Cost Optimization Design Principles

### Key Recommendations:

1. **Adopt the consumption model**
   - Only pay for what you consume

2. **Stop spending money on data centers**
   - Eliminate data center operations costs

3. **Measure overall efficiency**

4. **Analyze and track cost and usage**

5. **Use AWS-managed services**
   - Reduces overall cost of ownership

### Why AWS Offers Lower Costs:
- **Economies of scale**

---

## Benefits of Freeing Up Technical Resources

### When You Stop Spending on Data Centers and Pay for Consumption:

**Technical resources become available to prioritize:**
1. Optimizing resource utilization
2. Creating more efficient applications
3. Developing better end-user experience
4. Other areas that help organization streamline operations
5. Activities that generate more revenue

---

## Total Cost of Ownership (TCO) - Four Parts

### 1. Operational Expenses (OpEx)

**Definition:**
- Day-to-day operating costs

**Examples:**
- Utilities
- Printer toner
- Coffee
- Snacks

### 2. Capital Expenses (CapEx)

**Definition:**
- Costs associated with creating longer-term benefits

**Examples:**
- Purchasing a building
- Servers
- Printer (that uses the toner mentioned in OpEx)
- Power backups

**Characteristics:**
- Generally purchased once
- Expected to aid organization for years

### 3. Labor Costs

**Definition:**
- Staffing costs for on-premises environment or data center

**Examples:**
- Network operation center technicians who handle:
  - Installation
  - Configuration
  - Troubleshooting
  - Management of servers and infrastructure

### 4. Software Licensing Costs

**Important Considerations When Moving to AWS:**

**Questions to Ask:**
- How will current software licenses be affected by move to AWS?
- Can licenses be transferred?
- Do they require different kinds of licenses?
- Can you forego current license in favor of one managed by AWS?

**Key Point:**
- All these and other questions should be considered when evaluating economics of operating in cloud

---

## Cost Reduction Strategies

### Important Understanding for Exam:

**Migration Reality:**
- NOT usually a one-to-one transition
- Some applications can be moved directly to AWS
- Often additional things need to be considered to be most economical

### Key Cost Reduction Areas:

**1. Benchmarking and Performance Testing**
- Establish benchmarking and performance testing
- Instead of focusing on provisioning for peak demand

**2. Automation**
- Can help reduce costs
- Example: Cost savings from scaling horizontally to meet demands
- Instead of running on-premises at peak capacity when not in peak demand

**3. Data Segmentation and Targeted Reporting**
- Can help reduce scope of compliance
- Save time during audits

**4. Managed Services**
- Strongly consider using managed services
- Helps reduce technical workload
- Reduces costs for variety of different use cases

---

## Key Exam Focus Areas

### Deep Dive Topics:

1. **Right Sizing**
   - Covered in AWS Well-Architected Framework

2. **Adding Automation**
   - Covered in AWS Well-Architected Framework

3. **Ensuring Compliance is Met**
   - Reducing compliance scope
   - Covered in AWS Well-Architected Framework

4. **Using AWS Managed Services**
   - Covered in AWS Well-Architected Framework

---

## Critical Exam Tip

### Capital Expenses vs. Variable Expenses:

**When migrating from on-premises to AWS:**
- You are **trading capital expenses (CapEx) for variable expenses**

**What This Means:**
- On-premises: Large upfront capital investments (CapEx)
- AWS: Pay-as-you-go variable expenses (OpEx)

---

## Course Structure Going Forward

### What's Next:
- **Domain 3:** Cloud Technology and Services
  - Will dive deeper into AWS services

### Learning Approach:
- Various services, benefits, tools, and features mentioned throughout
- A lot to remember and understand
- Course will continue to:
  - Identify keywords for different services
  - Take topics and concepts and build on each of them

### Study Advice:
- The deeper you dive into fundamentals, benefits of AWS, and cloud economics
- The more it will all make sense for:
  - Certification exam
  - Real world applications

---

## Summary of Domain 1: Cloud Concepts

### Four Task Statements Covered:

**1. Task Statement 1.1: Define Benefits of AWS Cloud**
- What is AWS
- What is cloud computing (5 criteria)
- AWS global infrastructure
- High availability, fault tolerance, disaster recovery
- Elasticity and scaling

**2. Task Statement 1.2: Identify Design Principles**
- AWS Well-Architected Framework
- Six pillars and their design principles
- Key concepts: parallelization, decoupling

**3. Task Statement 1.3: Migration Benefits and Strategies**
- AWS Cloud Adoption Framework (CAF)
- Four stages of adoption
- Seven migration strategies (7 R's)
- AWS services for migration
- Data backup and storage considerations

**4. Task Statement 1.4: Cloud Economics**
- Total Cost of Ownership (TCO)
- OpEx vs. CapEx
- Cost reduction strategies
- Right sizing, automation, compliance, managed services

---

## Key Takeaways for Exam

**Remember:**
1. AWS offers lower costs through economies of scale
2. Pay only for what you consume (consumption model)
3. Trading CapEx for variable expenses when moving to AWS
4. Automation and horizontal scaling reduce costs
5. Managed services reduce technical workload and costs
6. Right sizing is critical for cost optimization
7. Understand all four parts of TCO

---
