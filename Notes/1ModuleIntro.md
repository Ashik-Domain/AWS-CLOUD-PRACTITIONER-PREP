

---

# **✨ Complete Summary of Module 1 — Cloud Fundamentals (AWS-Centric)**

## **1. Amazon’s Journey to AWS**

* Amazon built scalable internal IT systems in early 2000s.
* 2003: Realised they could offer these efficiencies to the world.
* 2004: Launched **Amazon SQS** — first public AWS service.
* 2006: Released **Amazon S3** and **EC2**, starting modern cloud computing.
* AWS rapidly expanded into databases, analytics, networking, and enterprise adoption.

---

## **2. What is Cloud Computing?**

* On-demand delivery of IT resources (compute, storage, databases, networking, software) over the internet.
* **Pay-as-you-go** pricing → no upfront cost, no long-term contracts.
* **Scalable and flexible** → instantly scale up/down.
* **Remote access** → manage resources from anywhere.
* Removes the need to own or manage hardware.
* Enables agility and rapid innovation.

---

## **3. How Cloud Works**

* Applications/data stored in provider-managed data centers.
* Users access via web interfaces or APIs.
* Resources can be provisioned or removed in seconds.
* Supports agility, faster experimentation, and quick deployment.

---

## **4. Benefits of Cloud Computing**

* Lower costs (operational instead of capital expenditure).
* No physical data-center maintenance.
* Global availability.
* High performance and security.
* Faster innovation.
* Unlimited scalability.

---

## **5. Types of Cloud Services**

* **IaaS** → Rent servers/storage/networks (EC2, EBS).
* **PaaS** → Platforms for building apps (Elastic Beanstalk).
* **SaaS** → Software delivered via internet (WorkMail).

---

## **6. Deployment Models**

* **Public Cloud** → Shared infrastructure (AWS).
* **Private Cloud** → Dedicated infra for one org.
* **Hybrid Cloud** → Combination of both.

---

## **7. AWS Global Infrastructure**

* AWS has data centers worldwide.
* Designed for **global reach**, **low latency**, and **high availability**.

---

## **8. Why Multiple Data Centers? (Analogy included)**

* Using only one is risky (disasters, failures).
* Analogy: Like having multiple coffee shops — if one closes, business continues.

---

## **9. High Availability**

* System remains available even if part fails.
* Built using redundant components across AZs.

---

## **10. Fault Tolerance**

* System continues to operate even during failures.
* More advanced than just high availability.
* Achieved through multi-AZ and multi-Region design.

---

## **11. AWS Regions**

* Physical geographic areas (e.g., ap-south-1).
* Each Region contains multiple AZs.

---

## **12. AWS Availability Zones (AZs)**

* One or more data centers with:

  * Independent power
  * Independent networking
  * Independent cooling
* Designed for low-latency, fault-tolerant architecture.

---

## **13. Best Practice for HA**

* Always deploy across **multiple AZs**.
* Ensures continuity even if one AZ fails.

---

## **14. Multi-Region Architecture**

* For disaster recovery or ultra-high availability.
* If one Region fails entirely, the second Region keeps the app alive.

---

## **15. AWS Shared Responsibility Model**

### **AWS Responsibility → Security *of* the Cloud**

* Protects infrastructure (hardware, software, networking, physical facilities).
* Handles physical access control and isolation.

### **Customer Responsibility → Security *in* the Cloud**

* Managing data security.
* Setting up IAM policies.
* Patching OS and applications (for IaaS).
* Encrypting data.
* Configuring firewalls and networks.

### **Shared Responsibilities**

* Depends on service type (IaaS vs PaaS vs SaaS).
* Encryption, network protection, OS management may shift.

---

## **16. Customer Responsibilities (Extra Explained)**

* Decide what data to store.
* Who can access it.
* Manage access lifecycle (grant, manage, revoke).
* Client-side encryption and data privacy.

---

## **17. Real-Life Example: E-commerce on AWS**

* **Global Reach:** Deploy in multiple Regions for worldwide customers.
* **Startup Friendly:** Low upfront cost, high speed.
* **High Availability:** Multi-AZ application setup.
* **Fault Tolerance:** If one AZ fails, app stays online.
* **Shared Responsibility:**

  * AWS → infra security
  * Company → secure user data, authentication, compliance (e.g., PCI DSS)

---

## **18. AWS as Building Blocks**

* AWS services combine like Lego blocks.
* Developers build apps without worrying about underlying hardware.

---

