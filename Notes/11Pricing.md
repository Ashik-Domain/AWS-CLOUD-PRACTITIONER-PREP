# AWS Cloud Practitioner – Module 11: Pricing & Support

**Complete Exam-Focused Summary**

---

## 1. Understanding AWS Pricing (FOUNDATION)

AWS pricing works like a **utility bill**:

* You pay **only for what you use**
* No upfront infrastructure cost
* No long-term lock-in unless you choose to commit

Cost control requires:

* Understanding pricing models
* Monitoring usage continuously
* Choosing the right support & optimization tools 

---

## 2. Three Fundamental AWS Pricing Principles (EXAM CORE)

| Principle              | Meaning                     |
| ---------------------- | --------------------------- |
| Pay as you go          | Pay only for actual usage   |
| Save when you commit   | Commit to usage → discounts |
| Pay less by using more | Volume-based tiered pricing |

Examples:

* On-Demand EC2 → Pay as you go
* Reserved Instances / Savings Plans → Save when you commit
* S3 tiered storage → Pay less by using more 

---

## 3. Primary AWS Cost Drivers (VERY IMPORTANT)

### 1️⃣ Compute

* Services: EC2, Lambda, ECS
* Charged by:

  * Time (seconds / hours)
  * Instance type
  * Pricing model (On-Demand, Reserved, Spot)

### 2️⃣ Storage

* Services: S3, EBS, Glacier
* Charged by:

  * Amount of data stored
  * Duration
  * Storage class

### 3️⃣ Data Transfer

* **Inbound → Free**
* **Within same Region → Mostly free**
* **Outbound → Charged per GB**

📌 **Exam rule**: Data transfer *out* of AWS usually costs money. 

---

## 4. Pricing Examples (REAL-LIFE SCENARIOS)

### EC2 Pricing Includes:

* Instance runtime
* Attached EBS storage
* Data transfer out

### S3 Pricing Includes:

* Storage size
* Requests
* Retrieval (Glacier classes)
* Replication
* Transfer acceleration

---

## 5. AWS Billing Models

| Model                  | Description                 |
| ---------------------- | --------------------------- |
| Single account billing | One account, one bill       |
| Consolidated billing   | Multiple accounts, one bill |

* Consolidated billing is enabled using **AWS Organizations**
* Aggregates usage for **volume discounts** 

---

## 6. AWS Pricing & Cost Management Tools (EXAM FAVORITE)

### AWS Billing Dashboard

* View:

  * Current charges
  * Invoices
  * Forecasts
* Payment & billing center

### AWS Budgets

* Set:

  * Cost budgets
  * Usage budgets
  * RI / Savings Plan budgets
* Get alerts when thresholds are crossed

### AWS Cost Explorer

* Analyze historical usage
* Visualize trends
* Forecast future costs
* Identify optimization opportunities

### AWS Pricing Calculator

* Estimate costs **before deployment**
* Compare configurations
* Planning & budgeting tool 

---

## 7. Cost Optimization Strategies (HIGH SCORING)

### Compute

* Rightsizing
* Auto Scaling
* Spot Instances (up to 90% cheaper)
* Savings Plans

### Storage

* Choose correct S3 storage class
* Lifecycle policies
* Compression
* Delete unused data

### Networking

* Minimize cross-AZ & internet traffic
* Use VPC Endpoints

📌 Cost optimization often **improves performance** too. 

---

## 8. AWS Support Plans (EXAM MUST-KNOW)

### Basic Support (Free)

* Documentation
* Forums
* Billing support
* **Core Trusted Advisor checks**
* AWS Health Dashboard

### Developer Support

* Email support
* Best for testing & dev
* Response:

  * < 24 hrs general
  * < 12 hrs impaired

### Business Support

* 24/7 phone + email
* **Full Trusted Advisor**
* Response:

  * < 1 hr production outage

### Enterprise On-Ramp

* Faster response
* Pool of Technical Account Managers (TAMs)

### Enterprise Support

* **Dedicated TAM**
* Proactive guidance
* Response:

  * < 15 minutes (critical)



---

## 9. Support Plans Comparison (EXAM TABLE)

| Plan               | Best For          | TAM       | Critical Response |
| ------------------ | ----------------- | --------- | ----------------- |
| Basic              | Learning          | ❌         | N/A               |
| Developer          | Dev/Test          | ❌         | 12 hrs            |
| Business           | Production        | ❌         | 1 hr              |
| Enterprise On-Ramp | Business-critical | Pool      | 30 min            |
| Enterprise         | Mission-critical  | Dedicated | 15 min            |

---

## 10. AWS Marketplace & Partner Network

### AWS Marketplace

* Pre-built third-party software
* SaaS, ML models, analytics tools
* Integrated billing
* Faster deployment

### AWS Partner Network (APN)

* AWS-certified partners
* Consulting & technical expertise
* Industry-specific solutions

Use Marketplace for **software**, APN for **people & expertise**. 

---

## 11. Cloud in Real Life – Cost Mindset

AWS cost management is like running a business:

* Track expenses
* Reduce waste
* Automate scaling
* Forecast growth
* Choose support wisely

---

## 12. Final Exam Takeaways (MEMORIZE)

* Pay as you go
* Save when you commit
* Compute, storage, data transfer = main costs
* Inbound data is free
* Use Cost Explorer for analysis
* Use Budgets for alerts
* Pricing Calculator before deployment
* Enterprise Support = Dedicated TAM
* Marketplace = third-party software

---
