# **📘 MODULE 2 — Compute in Cloud (FULL SUMMARY)**

### *(EC2 • Instance Types • AMI • Pricing • Scaling • Load Balancing • Messaging & Queuing)*

---

# **1. Amazon EC2 — Core Summary**

* EC2 provides **virtual servers** (instances) in the cloud.
* Much **faster, flexible, cost-effective** vs. on-prem servers.
* Launch, scale, or terminate instances in **minutes**.
* Pay only when instances are **running**.
* Uses a **hypervisor** for multi-tenancy & isolation.
* Full control of OS, networking, storage, and software stack.
* Vertical scaling = increase size; horizontal scaling = add more instances.

---

# **2. EC2 Instance Types**

### EC2 offers 5 major families:

1. **General Purpose** — balanced compute/memory/network (web apps, repos).
2. **Compute Optimized** — HPC, gaming, ML inference, scientific computation.
3. **Memory Optimized** — analytics, in-memory DBs, large dataset processing.
4. **Accelerated Computing** — GPUs, ML training, high graphics workloads.
5. **Storage Optimized** — high disk I/O, large databases, data warehousing.

---

# **3. How to Access AWS Resources (API-based)**

All AWS actions = API calls. Access methods:

### **1. AWS Management Console (GUI)**

* Easiest for beginners.
* Good for monitoring, billing, small tasks.
* Risk of human error; not ideal for automation.

### **2. AWS CLI**

* Text-based commands.
* Good for scripting, automation, repeatable infra.
* Requires CLI knowledge.

### **3. AWS SDK**

* Programmatic access (Python, Java, C#, etc.).
* Best for building cloud-enabled applications.
* Used for automation at scale.

### **4. Automation Importance**

* Reduces human mistakes.
* Enables reproducible deployments.

---

# **4. Shared Responsibility for EC2**

AWS — **security OF the cloud**
Customer — **security IN the cloud**

Customer must handle:

* OS updates, patches
* Firewall/security groups
* Data encryption
* IAM access

AWS handles:

* Physical infra, networking, hypervisor.

---

# **5. How to Launch an EC2 Instance (Steps)**

1. Open EC2 Console.
2. Click **Launch Instance**.
3. Configure:

   * Instance name
   * AMI
   * Instance type
   * Key pair (SSH)
   * Security groups (allow HTTP/SSH)
   * Storage (e.g., 8GB gp3)
   * User data (startup automation)
4. Launch instance.
5. Access via public IP.

---

# **6. AMI (Amazon Machine Image)**

Contains:

* OS
* Application software
* Architecture
* Permissions
* Storage configuration

### **Ways to use AMIs**

1. **Create your own** custom AMI.
2. **Use AWS-provided AMIs**.
3. **Buy AMIs from AWS Marketplace**.

### Benefits of AMIs

* Ensure **repeatability & consistency** across environments.

---

# **7. EC2 Pricing Models**

### **1. On-Demand**

* No commitment.
* Pay by second/hour.
* Best for short, unpredictable workloads.

### **2. Savings Plans**

* Commit ($/hour) for 1 or 3 years.
* Up to **72% savings**.
* Applies to EC2, Fargate, Lambda, SageMaker.

### **3. Reserved Instances**

* Commit to instance family & region.
* Up to **75% savings**.
* Good for predictable, steady workloads.

### **4. Spot Instances**

* Up to **90% cheaper**.
* AWS can interrupt with 2-min warning.
* Best for batch, analytics, fault-tolerant jobs.

### **5. Dedicated Hosts**

* Full physical server.
* Required for certain licenses/compliance.

### **6. Dedicated Instances**

* Hardware isolated from other customers.

### **7. Capacity Reservations**

* Reserve capacity in an AZ.
* Charged at On-demand rate regardless of use.

---

# **8. Cost Optimization Tips**

* On-Demand → irregular workloads.
* Savings Plans/RIs → predictable workloads.
* Spot Instances → interruptible jobs.
* Review usage via Cost Explorer.
* Avoid paying for idle instances.

---

# **9. Scaling & Elasticity**

### **Scalability**

* Add resources to handle growth.
* Long-term capacity planning.

### **Elasticity**

* Automatically adjust resources in real time.
* Prevents over-provisioning → saves cost.

### **Horizontal Scaling (Scale Out)**

* Add more instances.
* Best for stateless apps.

### **Vertical Scaling (Scale Up)**

* Increase instance size.
* Good for monoliths or unsharable workloads.

---

# **10. EC2 Auto Scaling**

Automatically changes number of instances based on load.

### Auto Scaling Group Settings:

* **Minimum capacity**
* **Desired capacity**
* **Maximum capacity**

### Types:

1. **Dynamic scaling** — responds to metrics.
2. **Predictive scaling** — anticipates patterns (AI-based).

---

# **11. Elastic Load Balancing (ELB)**

Solves traffic distribution problems.

### Benefits:

* Distributes traffic across multiple instances.
* Removes unhealthy instances automatically.
* Automatically scales with demand.
* Provides single DNS endpoint.
* Decouples application tiers.

### Routing Methods:

* Round Robin
* Least Connections
* Least Response Time
* IP Hash (sticky sessions)

### Works best when paired with Auto Scaling.

---

# **12. Messaging & Queuing in AWS**

Used for **decoupling** to avoid cascading failures.

## **1. Amazon SQS (Queue Service)**

* Fully managed queue.
* Producers send messages → consumers process later.
* Prevents data loss.
* Good for asynchronous processing.

## **2. Amazon SNS (Notification Service)**

* Publish/subscribe system.
* Sends messages to multiple subscribers instantly.
* Supports email, SMS, Lambda, HTTP endpoints.

## **3. Amazon EventBridge**

* Event routing bus.
* Supports event-driven architecture.
* Routes events between AWS services, apps, SaaS.
* Allows filtering, transformation, reliable delivery.

---

# **13. Monolithic vs. Microservices**

| Monolithic                  | Microservices             |
| --------------------------- | ------------------------- |
| Tightly coupled             | Loosely coupled           |
| Hard to scale independently | Each service scales alone |
| Single point of failure     | Failures isolated         |
| Slower deployments          | Faster deployments        |

---

# **14. When to Use What**

* **SQS** → async, delayed, buffer-based jobs.
* **SNS** → instant push notifications to many receivers.
* **EventBridge** → complex event workflow integration.

---


Just tell me!
