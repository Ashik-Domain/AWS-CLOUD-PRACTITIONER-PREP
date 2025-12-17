# AWS Cloud Practitioner Notes - Domain 2: Security and Compliance

## Domain 2 Overview

### What Domain 2 Covers:
- AWS Shared Responsibility Model
- Security
- Access Management
- Compliance

### Key Aspect of Understanding AWS:
- Recognize who is responsible for what in regards to security
- Some technical details about how services are hosted or how data is stored can be abstracted from you
- **Important:** Abstraction does NOT mean you are not responsible for security in AWS

### Your Responsibilities:
- Identify when security measures need to be put in place
- Identify when security measures are already put in place by AWS for you

---

## Domain 2 Task Statements

### Four Task Statements:

**Task Statement 2.1:** Understand the AWS Shared Responsibility Model

**Task Statement 2.2:** Understand AWS Cloud security, governance, and compliance concepts

**Task Statement 2.3:** Identify AWS access management capabilities

**Task Statement 2.4:** Identify components and resources for security

---

## What Each Task Statement Covers

### Task Statement 2.1: AWS Shared Responsibility Model

**Focus:**
- Being a cloud practitioner means determining when you need to secure resources within AWS
- Understanding the depth to which you need to be involved for security
- **Important:** Depth of involvement can vary from service to service

### Task Statement 2.2: Security, Governance, and Compliance Concepts

**Focus:**
- Understanding security concepts
- Understanding governance concepts
- Understanding compliance concepts in AWS

### Task Statement 2.3: Access Management in AWS

**Key Point:**
- Level of responsibility customer assumes changes depending on service being used
- **You are ALWAYS responsible for access management to your environment**
- This responsibility does not change across services

### Task Statement 2.4: Securing Different AWS Services

**What You Need to Know for Exam:**
- Do NOT need to know step-by-step directions on exactly how to enable security within AWS
- DO need to know generally what security features exist
- DO need to know when you are responsible for enabling them

---

## Course Structure for Domain 2

**Approach:**
- Each task statement will be addressed individually
- Breaking down knowledge and skills expected for success

---

## Key Concepts to Remember

### Security Responsibility in AWS:

**Understanding Abstraction:**
- AWS abstracts some technical details
- Abstraction ≠ No responsibility
- Must still identify and implement appropriate security measures

**Variable Responsibility:**
- Responsibility depth varies from service to service
- Must understand these variations for exam

**Constant Responsibility:**
- Access management is ALWAYS customer responsibility
- Regardless of which AWS service is being used

**General vs. Specific Knowledge:**
- For exam: Know what security features exist (general knowledge)
- For exam: Know when to enable them (general knowledge)
- Not required: Step-by-step implementation details (specific knowledge)

---

## Exam Preparation Focus

### What to Study:
1. **AWS Shared Responsibility Model**
   - What AWS is responsible for
   - What customer is responsible for
   - How responsibility varies by service

2. **Security, Governance, and Compliance**
   - Key concepts
   - How they apply in AWS

3. **Access Management**
   - Capabilities available
   - Customer's ongoing responsibilities

4. **Security Features and Resources**
   - What features exist
   - When to use them
   - Which services they apply to

---
## Notes for Success

**Important Mindset:**
- Security is a shared responsibility
- Know your role vs. AWS's role
- Understand that your role varies by service
- Always maintain access management control

**Exam Strategy:**
- Focus on understanding general security concepts
- Know when security is your responsibility
- Recognize when AWS handles security
- Understand access management is always your responsibility


# AWS Cloud Practitioner Notes - Task Statement 2.1: Understand the AWS Shared Responsibility Model

## What is the AWS Shared Responsibility Model?

### Definition:
- How AWS provides clarity around which areas of system security belong to AWS and which belong to the customer
- Provides clarity about which elements of infrastructure AWS manages
- Provides clarity about which elements customers are responsible for managing

### High-Level Principle:
- **AWS is responsible for:** Security OF the cloud
- **Customer is responsible for:** Security IN the cloud (your data, applications, etc.)

---

## AWS Global Infrastructure - Responsibility Breakdown

### Level 1: Foundation Infrastructure (AWS Responsibility)

**Components:**
- Regions
- Availability Zones
- Edge locations around the world
- AWS global infrastructure hardware
- Hardware security

**AWS Customer Role:**
- No control over any of this
- Do not have to worry about this infrastructure

### Level 2: Service Categories (AWS Responsibility)

**Components:**
- Compute
- Storage
- Networking
- Databases
- And other foundational services

**AWS Responsibility:**
- Managing these services
- Security of these services and systems

### Level 3: Supporting Software (AWS Responsibility)

**Components:**
- Software that assists any of the service levels below it

**AWS Manages:**
- Regions
- Global infrastructure
- Hardware
- Network
- Level services (compute, databases, network, storage, etc.)
- Software used to provide these services

**Example: Amazon EC2 Instance**
**What AWS Manages:**
- Region and Availability Zone where instance runs
- Provisioning
- Security of compute, networking, and storage needed for instance
- Software for the instance (user interface, hypervisor)

---

## Customer Responsibilities (Security IN the Cloud)

### Where Customer Responsibility Begins:
- **Operating system and upwards**

### Customer is Responsible For:

**1. Data Encryption and Protection:**
- Client-side data encryption
- Data integrity
- Authentication
- Server-side encryption
- Protecting network traffic
- Encrypting data using SSL certificates

**2. Operating System and Configuration:**
- Operating system management
- Network configuration
- Firewall configurations

**3. Application Layer:**
- Application management
- Application security

**4. Identity and Access Management (IAM):**
- Controlling who has access to your account
- Controlling access to services in that account
- Managing user permissions

**5. Customer Data:**
- Securing customer data
- Backups of that data

---

## Determining Responsibility

### Cloud Practitioner Ability:
- Must be able to determine when to secure resources in AWS
- Must understand depth of involvement needed for security
- **Important:** This varies from service to service

### Example Question:
**Who is responsible for securing the data centers that host AWS services?**
- **Answer:** AWS (not the customer)
- This is the level of determination needed for the shared responsibility model

---

## How Responsibility Shifts by Service

### Key Concept:
- Customer's responsibility shifts depending on the service being used

### Example Scenario: MySQL Database

**Scenario 1: MySQL Database on Amazon RDS**
- **Question:** Who is responsible for patching the database engine?
- **Answer:** AWS is responsible for patching

**Scenario 2: MySQL Database on Amazon EC2**
- **Question:** Who is responsible for patching?
- **Answer:** Customer is responsible for patching

### Why the Difference?

**Managed vs. Unmanaged Services:**

**Amazon RDS (Managed Service):**
- AWS performs more security and management tasks
- Customer required to carry out LESS security and management tasks

**Amazon EC2 (Unmanaged Service):**
- Customer has more control over the service
- Customer is MORE responsible for security and management tasks

---

## Key Takeaways for Exam

### Critical Understanding:
**The level of responsibility the customer assumes changes depending on the service they're using**

### Services to Know Customer vs. AWS Responsibilities:
1. **Amazon RDS** (managed)
2. **Amazon EC2** (unmanaged)
3. **Amazon DynamoDB** (managed)
4. **AWS Lambda** (managed)
5. And more (these are just a few examples)

---

## Shared Responsibility Model - Visual Summary

### AWS Responsibilities (Security OF the Cloud):
- Physical infrastructure
- Hardware
- Global network
- Regions, Availability Zones, Edge Locations
- Foundational services (compute, storage, networking, databases)
- Hypervisor and underlying software
- For managed services: OS patching, database patching, infrastructure maintenance

### Customer Responsibilities (Security IN the Cloud):
- Operating system (for unmanaged services)
- Network and firewall configuration
- Platform and application management
- Identity and Access Management (IAM)
- Customer data
- Data encryption (client-side and server-side)
- Network traffic protection
- Authentication and authorization

### Shared Responsibilities:
- Patch management (varies by service)
- Configuration management (varies by service)
- Awareness and training

---

## Exam Preparation Tips

### What You Must Know:
1. **General principle:** AWS = OF the cloud, Customer = IN the cloud
2. **How responsibility shifts** between managed and unmanaged services
3. **Specific responsibilities** for key services (RDS, EC2, DynamoDB, Lambda)
4. **Always customer responsibility:** IAM, customer data, data encryption, application security
5. **Always AWS responsibility:** Physical infrastructure, global network, foundational services

### Study Strategy:
- For each AWS service you learn, identify:
  - Is it managed or unmanaged?
  - What does AWS handle?
  - What does the customer handle?

---

# AWS Cloud Practitioner Notes - Task Statement 2.2: Understand AWS Cloud Security, Governance, and Compliance Concepts

## Security and Compliance in Design Decisions

### Key Principle:
- Must ensure security and compliance are considered when making design decisions

### Connection to Domain 1:
- Previously discussed choosing AWS Regions
- Must understand compliance needs among:
  - Geographic locations
  - Industries

---

## AWS Compliance

### What AWS Compliance Provides:

**1. Understanding Controls:**
- Helps understand controls in place at AWS
- Maintains security and data protection in AWS

**2. Assurance Programs:**
- Provide templates
- Provide control mappings
- Help customers establish compliance of their environments running on AWS

### Important for All Roles:
- Even if you're not building solutions on AWS
- Should be aware of how to find information about security and compliance
- Should know what services exist to support security and compliance plans

---

## Finding Compliance Information

### AWS Artifact

**What It Is:**
- Service that provides on-demand access to AWS security and compliance documents and reports

**Example Scenario:**
- Building solution requiring GDPR (General Data Protection Regulation) compliance
- Want to use Amazon DynamoDB to store data
- Question: How do you know if DynamoDB is GDPR compliant?
- Answer: Use AWS Artifact to find compliance information

### Important Note on Compliance Questions:

**How Questions Are Asked:**
- Exam asks: "Where to find compliance information?"
- Exam does NOT ask: "Is service X compliant with standard Y?"

**Reason:**
- Each individual AWS service has differences regarding compliance
- One service may require one set of actions for compliance standard
- Another service may require different set of actions for same compliance standard

### What You Need to Know for Exam:
- **DO need to know:** Where to find compliance information (AWS Artifact)
- **DO need to know:** Compliance requirements vary from service to service
- **DO NOT need to memorize:** Every single compliance program and which AWS services meet those requirements

---

## Protecting Systems and Information

### Main Goal:
- Protect systems and information

### High-Level Understanding Required:
- Be prepared to answer questions about different ways compliance and security can be achieved
- From a high-level perspective

---

## AWS Security Services

### How to Secure Resources on AWS

**Question to Consider:**
- What if you want to add more security to your network beyond:
  - Security groups
  - Network Access Control Lists (NACLs)
- What other AWS services can you use?

### Key Security Services:

**1. Amazon GuardDuty**
- **Type:** Threat detection service
- **Purpose:** 
  - Monitor for malicious activity
  - Monitor for unauthorized behavior

**2. AWS WAF (Web Application Firewall)**
- **Type:** Web application firewall
- **Purpose:**
  - Help protect applications from common exploits
  - Prevent exploits that could:
    - Impact application availability
    - Compromise security
    - Consume excessive resources

**3. AWS Shield**
- **Type:** Managed DDoS protection service
- **Purpose:**
  - Protect resources from Distributed Denial of Service (DDoS) attacks
  - Safeguard applications running on AWS

**4. Other Security Services:**
- Amazon Inspector
- AWS Security Hub
- And more

---

## Encryption Fundamentals

### Importance:
- Definite fundamental needed for certification and real world
- Available: deeper dive into encryption fundamentals

### Key Concept:
- Encryption is NOT a singular thing done one time
- Many different ways to use encryption techniques

### Two Main Types of Encryption:

**1. Encryption of Data in Transit**
- **Definition:** Data as it moves between two different places

**2. Encryption of Data at Rest**
- **Definition:** Stored data

### Why Cloud Practitioners Need to Know the Difference:
- Helps select AWS services that support the level of encryption needed

### Encryption Responsibility:

**Important Considerations:**
1. Identify who enables encryption for different AWS services
2. Links back to AWS Shared Responsibility Model
3. Requires AWS service-specific knowledge

**Resources:**
- Information on encryption available in:
  - AWS whitepapers
  - AWS documentation

---

## Logging, Auditing, and Reporting

### Types of Activity in AWS Account:

**1. Internal Activity:**
- AWS users creating AWS resources
- AWS users modifying AWS resources

**2. External Activity:**
- External users accessing AWS resources
- External users using AWS resources
- Example: Sending request to backend web server

### What You Should Understand:

**About Logs:**
- What logs are
- Logs can be used to:
  - Troubleshoot activity in AWS account
  - Audit activity in AWS account

---

## AWS Monitoring and Auditing Services

### Making Distinctions Between Services:

**1. Amazon CloudWatch**
- **Purpose:** Monitoring and collecting operational data
- **Use Case:** Performance metrics, system monitoring

**2. AWS CloudTrail**
- **Purpose:** Log events related to AWS resource creation and management
- **Use Case:** Governance, compliance, operational auditing, risk auditing
- **Function:**
  - Continuously monitors account activity
  - Retains account activity related to actions across AWS infrastructure

**Example Question:**
- "What AWS service identifies an IAM user who deleted an Amazon EC2 instance in production environment?"
- **Answer:** CloudTrail

**CloudTrail Trail for Multi-Regions:**
- Best way to keep track of all activities in AWS account
- Can create CloudTrail trail for multi-Regions

**3. AWS Config**
- **Purpose:** 
  - Take inventory of current configurations
  - Audit resources to ensure they maintain correct configurations
- **Use Case:** Configuration compliance, resource tracking

**4. AWS Audit Manager**
- Another service for auditing
- Don't need to understand the logs or data these services create
- Should be able to:
  - Explain what the services do
  - Explain their use cases
  - Understand the difference between them

---

## Service Comparison Summary

| Service | Primary Purpose | Key Use Case |
|---------|----------------|--------------|
| **CloudWatch** | Monitoring operational data | Performance metrics, system health |
| **CloudTrail** | Logging API calls and resource management | Who did what, when (auditing) |
| **Config** | Configuration tracking and compliance | Resource inventory, configuration audit |
| **Audit Manager** | Compliance auditing | Audit preparation and management |

---

## Least-Privileged Access

### Important Security Concept:

**Principle:**
- Not every person using AWS account should have same level of permissions

**Best Practice:**
- Follow concept of least-privileged access
- Only give people the level of access they need
- Nothing more

**Why This Matters:**
- Reduces security risk
- Limits potential damage from compromised accounts
- Follows security best practices

---

## Exam Preparation Summary

### What You Must Know:

**1. Compliance:**
- Where to find compliance information (AWS Artifact)
- Compliance requirements vary by service
- Don't need to memorize all compliance programs

**2. Security Services:**
- GuardDuty: Threat detection
- AWS WAF: Web application firewall
- AWS Shield: DDoS protection
- Inspector, Security Hub, and others exist

**3. Encryption:**
- Difference between data in transit and data at rest
- Who enables encryption (ties to Shared Responsibility Model)
- Service-specific encryption requirements

**4. Logging and Auditing:**
- CloudWatch: Monitoring operational data
- CloudTrail: Logging resource creation/management, API calls
- Config: Configuration inventory and audit
- Audit Manager: Compliance auditing
- Know the differences and use cases

**5. Access Management:**
- Principle of least-privileged access
- Only give necessary permissions

---

## Key Takeaways

**High-Level Understanding:**
- Know where to find information
- Understand service purposes and use cases
- Don't need deep technical implementation details

**Security First:**
- Security and compliance must be considered in design decisions
- Multiple services available for different security needs
- Encryption is fundamental

**Auditing and Compliance:**
- Know which service to use for what type of logging/auditing
- Understand CloudTrail for tracking "who did what"
- Use AWS Artifact for compliance documentation

---
# AWS Cloud Practitioner Notes - Task Statement 2.3: Identify AWS Access Management Capabilities

## User and Identity Management

### Why Control User Access?

**Key Principle:**
- Not everyone who uses AWS account needs same level of access
- Need way to control level of access to control how people use AWS services within account

**Example:**
- Analyst: Likely won't need administrator access for Amazon EC2
- Systems Administrator: May need administrator access for Amazon EC2

### Principle of Least Privilege

**Definition:**
- Only give users exactly the level of access they need to do their work
- Nothing more

**Importance:**
- Fundamental security concept
- Critical for exam and real-world implementation

---

## AWS Identity and Access Management (IAM)

### What You Need to Know:
1. Features of AWS IAM
2. How it enables you to control access to AWS account
3. When to use different aspects of IAM based on use case

### Fundamental Knowledge Required:
- User and identity management
- Security fundamentals
- AWS IAM knowledge

---

## AWS Accounts

### Why Understanding AWS Accounts is Crucial:

**Range of Complexity:**
- Simple systems: Operating in single AWS account
- Complex systems: Using tens or even hundreds of AWS accounts

### What is an AWS Account?

**Functions:**
1. Where you provision your services
2. Where AWS services log their usage
3. Where you can log into environment
4. Services you provision generate a bill
5. Bill is charged to payment method chosen when creating account

**Connection to Cloud Computing:**
- Remember: This is the fifth criteria of cloud computing (covered in first lesson)

### AWS Account Ownership:

**Important Points:**
- When you create AWS account, it is yours and only yours
- Yours until you grant access to others
- AWS accounts by default do NOT have permissions
- Must explicitly grant permissions

---

## AWS Account Root User

### What is the Root User?

**Definition:**
- Sign-in identity created when you create AWS account
- Has complete access to all AWS services and resources in the account

### Root User Characteristics:

**Access Level:**
- Complete and unrestricted access to all resources in AWS account

**Critical Warning:**
- Should NOT be using this user to carry out daily tasks in AWS

### Why Root User Protection is Critical:

**Due to unrestricted access:**
- Every cloud practitioner must know:
  1. How to protect root users
  2. When to use the root user
  3. When NOT to use the root user

---

## Protecting the Root User

### Methods to Lock Down Root User:

**1. Multi-Factor Authentication (MFA)**
- Enable MFA for root user

**2. Secure Credential Storage**
- Securely lock away root user credentials

**3. Credential Rotation**
- Rotate access keys
- Rotate password for root user

**4. Avoid Daily Use**
- Do NOT use root user for daily tasks
- AWS recommendation: Configure admin user in AWS IAM Identity Center
- Use admin user to perform daily tasks and access AWS resources

---

## Root User Tasks

### Limited Number of Tasks Requiring Root User Access:

**Tasks You Can Perform as Root User:**
1. Change your account settings
2. Restore IAM user permissions
3. Activate IAM access to Billing and Management console
4. Create account alias in IAM (substitutes account ID in web address for IAM users)
5. And more (limited list)

**Exam Focus:**
- Know which tasks you can perform as root user of account

---

## AWS IAM Features

### Four Main Features:

**1. IAM Users**
**2. IAM Groups**
**3. IAM Roles**
**4. IAM Policies**

---

## IAM Users

### What You Should Know:

**User Characteristics:**
- Have associated usernames and passwords
- Have access keys for programmatic access
- Can have MFA enabled for login
- Can enforce password complexity
- Can enforce access key rotation
- Can enforce password rotation

### Organizing Users:

**IAM Groups:**
- Can organize users into groups
- Affects permissions when AWS actions are taken

---

## IAM Permissions and Policies

### How Permissions Work in AWS:

**IAM Policies:**
- Can be applied to:
  - Users
  - Groups
  - Roles
- Impact entity's access based on policy

### Understanding Impact:
- Need to know how applying policies affects access

---

## IAM Roles

### Very Important for Exam:

**What are Roles?**
- Temporary credentials
- Can be assumed by various entities
- Have many use cases

### Common Use Cases:

**1. User Access:**
- User can assume role to gain temporary access to permissions

**2. Programmatic Access:**
- Program can assume role to gain access to AWS credentials
- Makes AWS API calls

**3. Cross-Account Access:**
- Use roles for cross-account access

**4. AWS Service Permissions:**
- Provide AWS services permissions to do certain actions

**5. External Entity Permissions:**
- Give outside entities permissions to perform actions in AWS account

### Key Question:
**When is it better to use IAM role rather than IAM user?**
- Important distinction to understand for exam

---

## Amazon Cognito

### Use Case Question:

**Scenario:**
- Need to provide temporary AWS credentials for:
  - Users authenticated through social media logins
  - Guest users who do not require authentication

**Answer: Amazon Cognito Identity Pool**

### Amazon Cognito Services:

**1. Amazon Cognito Identity Pool**
- Provides temporary AWS credentials
- Enables access for authenticated and unauthenticated identities
- Use for the scenario above

**2. Amazon Cognito User Pool**
- User directory in Amazon Cognito
- Does NOT enable access to unauthenticated identities
- Different use case from Identity Pool

---

## IAM Policies - Deep Dive

### Types of IAM Policies:

**1. Managed Policies**
- AWS creates and manages these
- Cannot be modified by customers

**2. Unmanaged (Customer Managed) Policies**
- Customers create and manage these
- Can be edited and modified by customers

### What You Should Know:
- Difference between two types of policies
- Who can create each type of policy
- Who can edit or modify each type of policy

---

## IAM Policy Simulator

### What It Is:
- AWS service to test and troubleshoot IAM and resource-based policies

### Use Case:
- Testing policies before implementation
- Troubleshooting policy issues

---

## Amazon S3 Security

### Scenario 1: Bucket Access Control

**Question:**
- Need to add security to Amazon S3 bucket
- Only allow access for specific users
- Options: IAM role, IAM user policy, or bucket policy?

**Answer: Bucket Policy or User Policy**

### Bucket Policies vs. User Policies:

**Bucket Policies:**
- Type of resource-based policy
- Differ from IAM roles
- Added to bucket to grant permissions
- Grant other AWS accounts or IAM users access permissions for:
  - The bucket
  - Objects in the bucket
- Uses JSON-based access policy language

**User Policies:**
- Policies that allow IAM user access to one of your buckets
- Uses JSON-based access policy language

**Both are Access Policy Options:**
- Both available to grant permission to Amazon S3 resources
- Both use JSON-based access policy language

---

### Scenario 2: Preventing Unauthorized Deletion

**Question:**
- Object accidentally deleted from S3 bucket
- What can you implement to prevent unauthorized deletion of other objects?

**Answer: MFA Delete**

**How to Implement:**
1. Must enable versioning for objects first
2. Configure MFA delete on S3 bucket
3. Adds extra layer of protection

**Important:**
- Versioning must be enabled BEFORE configuring MFA delete

---

## Exam Preparation Summary

### Key Areas to Master:

**1. User and Identity Management:**
- Why it's needed
- Principle of least privilege
- How to control access

**2. AWS Accounts:**
- What they are
- How they work
- Default permissions (none until granted)
- Ownership and access control

**3. Root User:**
- What it is
- Complete unrestricted access
- When to use (limited tasks)
- When NOT to use (daily tasks)
- How to protect (MFA, secure storage, rotation, avoid daily use)

**4. IAM Features:**
- Users (credentials, MFA, rotation)
- Groups (organization, permissions)
- Roles (temporary, use cases, when to use vs. users)
- Policies (managed vs. unmanaged, who creates/edits)

**5. Amazon Cognito:**
- Identity Pool (temporary credentials, authenticated/unauthenticated)
- User Pool (user directory, authenticated only)

**6. IAM Policies:**
- Types: Managed vs. Unmanaged
- IAM Policy Simulator
- Resource-based policies

**7. S3 Security:**
- Bucket policies vs. User policies
- MFA Delete
- Versioning requirement

---

## Critical Exam Concepts

**Always Remember:**
1. Principle of least privilege
2. Root user should NOT be used for daily tasks
3. Roles provide temporary credentials
4. Roles vs. Users - know when to use which
5. Policies can be applied to users, groups, or roles
6. MFA adds extra security layer
7. Versioning must be enabled before MFA delete
8. Cognito Identity Pool for temporary credentials

---
# AWS Cloud Practitioner Notes - Task Statement 2.4: Identify Components and Resources for Security Support

## Role of Cloud Practitioner in Security

### Important to Remember:
- As cloud practitioner, you likely will NOT be building out security solutions yourself
- You WILL be guiding people towards solutions that meet their needs

### What You Must Know:
1. What security services exist
2. How to find more information on them

---

## Network Security Services

### What You Need to Know:
- Basic functionality for AWS security services
- Use cases for these services
- Differences between them

**Important Note:**
- Do NOT need to know specifics of how these work in-depth
- SHOULD know enough to answer questions about:
  - When to use each one
  - Their function

---

## Network Access Control Lists (NACLs)

### What Are NACLs?

**Definition:**
- Act as firewall to control traffic traversing your subnet

**Use Case:**
- What can you use to secure your Amazon VPC subnets?
- Answer: Network Access Control Lists

### NACL Characteristics:

**1. Association:**
- Associated with subnets
- NOT associated with resources

**2. Traffic Management:**
- Used for traffic entering or leaving subnet
- Only manage traffic crossing subnet boundary

**Example - When NACLs DON'T Apply:**
- Two Amazon EC2 instances in Amazon VPC communicating with each other
- NACL has NO involvement
- Communication between instances is not crossing subnet boundary

**3. Stateless:**
- Only see traffic going one way
- Traffic seen as two separate, different streams
- Must have two rules (one for each stream)

**Rules Required:**
- If you allow inbound rule: Must also allow outbound rule
- NACL must explicitly see that traffic allowed inbound is also allowed out
- If you do NOT add outbound rule: Traffic only allowed in

---

## Security Groups

### What Are Security Groups?

**Definition:**
- Secure resource-level network

**What They Protect:**
- Amazon EC2 instances
- Amazon RDS instances
- Other AWS resources

### Security Group Characteristics:

**1. Association:**
- Do NOT operate at subnet level
- Operate at resource's Elastic Network Interface (ENI) level

**2. Rules:**
- Have inbound and outbound rules

**3. Stateful:**
- If traffic is allowed in: Traffic automatically allowed back out
- See both inbound and outbound traffic as part of same stream

**4. AWS Resource Recognition:**
- Can recognize AWS resources
- Can add rules for other security groups
- Can add rule for security group themselves

**5. Implicit Deny:**
- Have hidden explicit deny
- Anything not explicitly allowed is denied

**CRITICAL FOR EXAM:**
- Security groups CANNOT explicitly deny
- If you need to explicitly deny: Must use Network Access Control List

**6. Accepted Rules:**
- IP addresses
- IP address ranges
- Security group IDs (as source or destination for inbound and outbound rules)

---

## Security Groups vs. Network Access Control Lists

### Comparison Summary:

| Feature | Security Groups | Network ACLs |
|---------|----------------|--------------|
| **Level** | Resource (ENI) | Subnet |
| **State** | Stateful | Stateless |
| **Rules** | Return traffic automatic | Must explicitly allow both directions |
| **Deny** | Implicit deny only (cannot explicitly deny) | Can explicitly deny |
| **Recognition** | Recognizes AWS resources and security groups | Works with IP addresses only |
| **Association** | Associated with resources | Associated with subnets |

---

## AWS WAF (Web Application Firewall)

### Use Case Question:

**Scenario:**
- Need to create rules to filter web traffic based on conditions such as:
  - IP addresses
  - HTTP headers
  - Custom URLs

**Answer: AWS WAF**

### What AWS WAF Does:
- Helps control traffic with rules you define
- Blocks common attack patterns such as:
  - SQL injections
  - Cross-site scripting

---

## Security Assessment and Penetration Testing

### Question:
**Can you conduct security assessment and penetration testing without prior approval against AWS resources?**

**Answer:**
- Yes, but only for certain services

### Important Note:
- Not all AWS services allow penetration testing without approval
- Know which services have restrictions

---

## AWS Security Recommendation Services

### Services That Provide Security Recommendations:

**1. AWS Trusted Advisor**
- Provides recommendations around security
- Also provides recommendations for other areas (cost, performance, etc.)

**2. Amazon Inspector**
- Provides security recommendations
- Automated security assessment service

### Exam Awareness:
- Should be aware these services exist
- Understand they provide security recommendations

---

## Third-Party Security Solutions

### Important Recognition:
- Sometimes solution to security and compliance needs could be third-party software or tools

### AWS Marketplace

**Question:**
- Where can you find available third-party software to deploy in AWS account?

**Answer: AWS Marketplace**

### Exam Knowledge Required:
- Know what exists at high level for AWS services
- Know types of solutions you can find via AWS Marketplace
- Important knowledge for exam

---

## Resources for Security Information

### Places to Find Security Information:

**1. AWS Knowledge Center**
- Find answers to your questions

**2. Security Center**
- Information related to security in AWS

**3. AWS Security Blogs**
- Should be comfortable reading these

**4. AWS Security Forum**
- Use to find information
- Community discussions

**5. AWS Documentation**
- Best practices
- General information
- Use cases
- Information on what services exist
- How services work

**6. AWS Whitepapers**
- Deeper dives into topics
- Comprehensive security information

**7. AWS Official Documentation**
- General information
- Service-specific details

---

## Exam Preparation Strategy

### What You Should Be Comfortable With:

**1. Finding Information:**
- Know where to look for security information
- Multiple resources available

**2. Research Skills:**
- Able to identify resources to dive deeper into cloud topics when necessary
- Know which resource to use for what type of information

**3. Service Knowledge:**
- High-level understanding of AWS security services
- Know use cases
- Know differences between services

---

## Key Security Concepts Summary

### Network Security:

**NACLs:**
- Subnet level
- Stateless
- Can explicitly deny
- Two rules needed (inbound + outbound)
- Controls traffic crossing subnet boundary

**Security Groups:**
- Resource/ENI level
- Stateful
- Cannot explicitly deny (implicit deny only)
- Return traffic automatic
- Recognizes AWS resources

**AWS WAF:**
- Web application firewall
- Filters web traffic
- Blocks common attack patterns

### Assessment and Recommendations:

**Penetration Testing:**
- Allowed for certain services
- May require approval for others

**Recommendation Services:**
- Trusted Advisor
- Amazon Inspector

### Resources:

**Third-Party Solutions:**
- Available via AWS Marketplace

**Information Sources:**
- Knowledge Center
- Security Center
- Security Blogs
- Security Forum
- Documentation
- Whitepapers

---

## Exam Tips

**Critical Distinctions:**
1. Security Groups vs. NACLs - know the differences
2. Security Groups CANNOT explicitly deny
3. NACLs are stateless, Security Groups are stateful
4. Know when to use AWS WAF
5. Know where to find third-party solutions (Marketplace)
6. Know resources for security information
7. Understand which services provide security recommendations

**Study Focus:**
- High-level understanding of services
- Use cases and differences
- Where to find information
- When to use each service
---

## Domain 2 Complete - Summary

### Four Task Statements Covered:

**Task Statement 2.1: AWS Shared Responsibility Model**
- AWS: Security OF the cloud
- Customer: Security IN the cloud
- Responsibility varies by service (managed vs. unmanaged)

**Task Statement 2.2: Security, Governance, and Compliance**
- AWS Artifact for compliance information
- Security services (GuardDuty, WAF, Shield, Inspector, Security Hub)
- Encryption (in transit vs. at rest)
- Logging and auditing (CloudWatch, CloudTrail, Config, Audit Manager)
- Least-privileged access

**Task Statement 2.3: Access Management**
- Root user protection
- IAM features (users, groups, roles, policies)
- Principle of least privilege
- Amazon Cognito
- S3 security (bucket policies, MFA delete)

**Task Statement 2.4: Security Components and Resources**
- Network security (NACLs vs. Security Groups)
- AWS WAF
- Penetration testing
- Recommendation services
- AWS Marketplace
- Security information resources
