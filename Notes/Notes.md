---
# AWS Cloud Practitioner – FINAL EXAM SYLLABUS SUMMARY
---

# ✅ DOMAIN 1: Cloud Concepts (≈24%)

> **Focus:** What cloud is, why it exists, and why AWS is better than traditional IT.

---

## 1. What is Cloud Computing?

**Definition (EXAM-FRIENDLY):**
Cloud computing is the **on-demand delivery of IT resources** (compute, storage, databases, networking) over the internet with **pay-as-you-go pricing**.

Key characteristics:

* On-demand provisioning
* Pay only for what you use
* Scalable and elastic
* No physical hardware ownership
* Global access via internet

---

## 2. Benefits of Cloud Computing (VERY IMPORTANT)

AWS cloud benefits you must remember:

* **Scalability** – ability to grow over time
* **Elasticity** – automatic scale up/down based on demand
* **Cost savings** – no upfront investment
* **Speed & agility** – launch resources in minutes
* **Global reach** – deploy worldwide quickly
* **High availability & fault tolerance**

📌 Exam style:
“Which benefit allows you to handle sudden traffic spikes?” → **Elasticity**

---

## 3. Cloud Deployment Models

You must recognize these terms (no deep design questions):

* **Public Cloud** – shared infrastructure (AWS)
* **Private Cloud** – dedicated to one organization
* **Hybrid Cloud** – on-prem + cloud
* **Multi-Cloud** – multiple cloud providers

📌 Exam style:
“A company uses AWS and on-prem together” → **Hybrid cloud**

---

## 4. Cloud Economics (NO MATH, ONLY CONCEPT)

* **CapEx (Capital Expenditure)**
  Buy servers upfront (traditional IT)

* **OpEx (Operational Expenditure)**
  Pay monthly for usage (AWS)

* **Fixed cost vs Variable cost**

  * On-prem → fixed
  * AWS → variable

📌 Exam style:
“Which pricing model reduces upfront investment?” → **OpEx**

---

## 5. AWS Global Infrastructure (HIGH LEVEL)

Core terms:

* **Region** – geographic area
* **Availability Zone (AZ)** – isolated data center group
* **Edge Location** – content delivery (CloudFront)

Why it matters:

* High availability
* Fault tolerance
* Disaster recovery
* Low latency

---

## 6. AWS Well-Architected Framework (HIGH LEVEL ONLY)

Purpose:

* Evaluate if architecture is **secure, reliable, efficient, and cost-effective**

Six pillars (just recognition):

* Operational Excellence
* Security
* Reliability
* Performance Efficiency
* Cost Optimization
* Sustainability

📌 Exam style:
“Which framework helps evaluate best practices?” → **Well-Architected Framework**

---

## 7. Cloud Adoption & Migration (CONCEPTUAL)

* Businesses migrate to:

  * Reduce cost
  * Improve scalability
  * Modernize apps

High-level strategies:

* Lift-and-shift
* Replatform
* Refactor

📌 Exam style:
“Which approach moves apps with minimal changes?” → **Rehost (lift-and-shift)**

---

# ✅ DOMAIN 2: Security & Compliance (≈30%)

🔥 **MOST IMPORTANT DOMAIN**

---

## 1. Shared Responsibility Model (ALWAYS ASKED)

### AWS is responsible for:

* Physical data centers
* Hardware
* Networking
* Global infrastructure
  👉 **Security OF the cloud**

### Customer is responsible for:

* Data
* OS patching (EC2)
* IAM users & permissions
* Application security
  👉 **Security IN the cloud**

📌 Exam style:
“Who patches the OS on EC2?” → **Customer**

---

## 2. Identity & Access Management (IAM)

### Root User

* Full access
* Should NOT be used daily
* MFA must be enabled

### IAM Components

* **Users** – people/apps
* **Groups** – collection of users
* **Roles** – temporary access (VERY IMPORTANT)
* **Policies** – permissions (JSON)

### Principle of Least Privilege

* Give minimum required access only

📌 Exam style:
“Best practice for permissions?” → **Least privilege**

---

## 3. Authentication vs Authorization

* **Authentication** → Who are you?
* **Authorization** → What can you do?

---

## 4. Compliance & Governance (HIGH LEVEL)

You must **recognize names**, not rules:

* HIPAA – healthcare
* PCI-DSS – credit cards
* ISO – international standards
* SOC – auditing standards
* Data residency / sovereignty – data location laws

📌 Exam style:
“Which service provides compliance reports?” → **AWS Artifact**

---

## 5. Basic Security Services (RECOGNITION ONLY)

* **Security Groups** – instance-level firewall
* **AWS Shield** – DDoS protection
* **AWS WAF** – web firewall
* **AWS KMS** – encryption keys
* **Amazon GuardDuty** – threat detection
* **Amazon Macie** – sensitive data discovery

---

# ✅ DOMAIN 3: Cloud Technology & Services (≈34%)

🔥 **BIGGEST DOMAIN**

> You must know **WHAT service to use**, not **HOW to configure**.

---

## 1. Compute Services

### Amazon EC2

* Virtual servers
* Full control
* You manage OS

Use when:

* Custom workloads
* Full control needed

---

### AWS Lambda

* Serverless
* Event-driven
* No server management
* Pay per execution

Use when:

* Short-running tasks
* Event-based workloads

📌 Exam style:
“Which service runs code without servers?” → **Lambda**

---

## 2. Storage Services

### Amazon S3

* Object storage
* Highly durable
* Used for:

  * Backups
  * Static websites
  * Archives

---

### Amazon EBS

* Block storage
* Attached to EC2
* Persistent storage

📌 Exam style:
“Where store static files?” → **S3**

---

## 3. Database Services

### Amazon RDS

* Managed relational databases
* SQL-based

### Amazon DynamoDB

* NoSQL
* Serverless
* Millisecond latency

📌 Exam style:
“Which database is serverless NoSQL?” → **DynamoDB**

---

## 4. Networking Services

* **Amazon VPC** – isolated network
* **Route 53** – DNS service
* **CloudFront** – CDN

📌 Exam style:
“Which service reduces latency globally?” → **CloudFront**

---

## 5. Containers (HIGH LEVEL)

* **Amazon ECS** – container orchestration
* **Amazon EKS** – Kubernetes
* **AWS Fargate** – serverless containers

---

## 6. Analytics, ML & Integration (RECOGNITION)

* **Athena** – query S3
* **Kinesis** – streaming data
* **SageMaker** – machine learning
* **SQS** – message queue
* **SNS** – notifications
* **EventBridge** – event routing

📌 Exam style:
“Which service decouples apps?” → **SQS**

---

## 7. Monitoring

* **CloudWatch** – metrics, logs, alarms
* **CloudTrail** – API activity auditing

📌 Exam style:
“Who did what in AWS?” → **CloudTrail**

---

# ✅ DOMAIN 4: Billing, Pricing & Support (≈12%)

---

## 1. AWS Pricing Basics

* **Pay-as-you-go**
* No upfront cost
* Pay only for usage

---

## 2. Free Tier

* 12 months free for selected services
* Limited usage

---

## 3. Cost Management Tools

* **Billing Dashboard** – invoices
* **AWS Budgets** – alerts
* **Cost Explorer** – analyze usage
* **Pricing Calculator** – estimate costs

---

## 4. AWS Support Plans (EXAM FAVORITE)

| Plan       | Key Feature                  |
| ---------- | ---------------------------- |
| Basic      | Free, docs & forums          |
| Developer  | Email support                |
| Business   | Phone + full Trusted Advisor |
| Enterprise | Dedicated TAM                |

📌 Exam style:
“Which plan gives a TAM?” → **Enterprise**

---

## 5. Trusted Advisor

Checks:

* Cost optimization
* Security
* Performance
* Fault tolerance
* Service limits

---
# Get to know AWS services and best practices by exploring AWS whitepapers relevant to your exam.

### **Whitepapers**

* **[Overview of Amazon Web Services](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/introduction.html)**
* **[AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)**
* **[AWS Shared Responsibility Model](https://docs.aws.amazon.com/whitepapers/latest/aws-risk-and-compliance/shared-responsibility-model.html)**
* **[AWS Pricing](https://aws.amazon.com/pricing/?aws-products-pricing.sort-by=item.additionalFields.productNameLowercase&aws-products-pricing.sort-order=asc&awsf.Free%20Tier%20Type=*all&awsf.tech-category=*all)**
* **[Compare AWS Support Plans](https://aws.amazon.com/premiumsupport/plans/)**

---

