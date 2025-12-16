# AWS Cloud Practitioner – Module 6: Storage
**Complete Exam-Focused Summary**
---

## 1. Importance of Storage in AWS

* Storage is used to retain:

  * Operational data
  * Application data
  * Backups and archives
  * Sensitive and compliance-driven data
* Different data types require **different storage models** based on:

  * Performance
  * Cost
  * Durability
  * Access patterns
* AWS provides **multiple storage services**, each optimized for a specific use case. 

---

## 2. Types of Storage in AWS (FOUNDATIONAL)

AWS storage is broadly categorized into:

1. **Block Storage**
2. **Object Storage**
3. **File Storage**

This classification is **frequently tested**.

## 3. Block Storage

### What is Block Storage?

* Data is split into fixed-size **blocks**.
* Only changed blocks are updated → **high performance**.
* Typically attached to a single compute resource.

### AWS Block Storage Services

* **EC2 Instance Store**
* **Amazon Elastic Block Store (EBS)**

### Use Cases

* Databases
* Operating systems
* Applications requiring frequent read/write operations

### Instance Store vs EBS (EXAM FAVORITE)

| Feature     | Instance Store | Amazon EBS       |
| ----------- | -------------- | ---------------- |
| Persistence | ❌ No           | ✅ Yes            |
| Attachment  | Physical host  | Network-attached |
| Backups     | ❌ No           | ✅ Snapshots      |
| Cost        | Included       | Separate         |
| Use Case    | Temporary data | Critical data    |

---

## 4. Amazon EC2 Instance Store

### Key Characteristics

* **Ephemeral (temporary)** storage.
* Physically attached to the EC2 host.
* Data is **lost** when instance:

  * Stops
  * Terminates
* Included in EC2 cost.

### Best For

* Cache
* Buffers
* Scratch data
* Temporary files

❌ **Never use for critical or persistent data**. 

---

## 5. Amazon Elastic Block Store (Amazon EBS)

### Key Characteristics

* **Persistent block storage** for EC2.
* Network-attached (independent of EC2 host).
* Data **survives stop/terminate** of instances.
* Supports:

  * Snapshots (incremental backups)
  * Encryption
  * Volume resizing
  * Performance tuning

### Best For

* Databases
* Application data
* Backup storage
* Disaster recovery

### Exam Trap

* EBS volumes are **AZ-scoped**, but snapshots can be used to move data across AZs/Regions. 

---

## 6. Instance Store vs EBS (VERY IMPORTANT)

| Feature           | Instance Store | Amazon EBS      |
| ----------------- | -------------- | --------------- |
| Persistence       | ❌ No           | ✅ Yes           |
| Data Loss on Stop | Yes            | No              |
| Attachment        | Physical host  | Network         |
| Backup            | Not supported  | Snapshots       |
| Use Case          | Temp data      | Databases, apps |

---

## 7. Object Storage – Amazon S3

### What is Object Storage?

* Stores data as **objects**:

  * Data
  * Metadata
  * Unique key
* Entire object must be rewritten on update.
* Flat structure (buckets, not folders).

### Amazon S3 Key Facts

* Fully managed, global service.
* Durability: **99.999999999% (11 nines)**.
* Max object size: **5 TB**.
* Unlimited total storage.
* Buckets are **region-specific** and **globally named**.
* Private by default. 

---

## 8. Amazon S3 Use Cases

* Static website hosting
* Backups & archives
* Media storage
* Logs
* Data lakes
* Compliance data retention

### Core S3 Features

* Versioning
* Lifecycle policies
* Encryption (at rest & in transit)
* Bucket policies & IAM access
* Presigned URLs
* Audit logging with CloudTrail 

---

## 9. Amazon S3 Storage Classes (HIGH EXAM WEIGHT)

### Key Idea

* Choose storage class based on **access frequency + cost**.
* Can mix classes in one bucket.
* Use **Lifecycle Policies** or **Intelligent-Tiering**.

### Main Storage Classes

* **S3 Standard** → frequent access
* **S3 Intelligent-Tiering** → unknown/changing access
* **S3 Standard-IA** → infrequent, fast access
* **S3 One Zone-IA** → cheaper, single AZ
* **S3 Express One Zone** → ultra-low latency
* **S3 Glacier Instant Retrieval** → archive, ms access
* **S3 Glacier Flexible Retrieval** → minutes to hours
* **S3 Glacier Deep Archive** → lowest cost, ~12 hrs retrieval
* **S3 Outposts** → on-prem S3 via AWS Outposts 

---

## 10. S3 Lifecycle Management

* Automates:

  * Transition to cheaper storage
  * Object deletion (expiration)
* Example:

  * Day 0 → Standard
  * Day 30 → Standard-IA
  * Day 90 → Glacier
  * Day 365 → Delete
* Critical for **cost optimization questions**. 

---

## 11. File Storage on AWS

### What is File Storage?

* Hierarchical structure (folders/files).
* Shared access by multiple systems.
* Minimal application changes.

### AWS File Storage Services

* **Amazon EFS**
* **Amazon FSx** 

---

## 12. Amazon Elastic File System (EFS)

### Key Characteristics

* Managed **NFS file system**.
* Supports **multiple EC2 instances concurrently**.
* Automatically scales up/down.
* Multi-AZ by default (high availability).

### Storage Classes

* EFS Standard / Standard-IA
* EFS One Zone / One Zone-IA
* EFS Archive (lowest cost, cold data)

### Best For

* Shared file systems
* Content management
* Analytics
* Media processing 

---

## 13. Amazon FSx

### What is FSx?

* Managed file systems for **specific enterprise workloads**.
* Supports:

  * Windows File Server
  * Lustre
  * NetApp ONTAP
  * OpenZFS

### Common Use Cases

* Windows file shares
* High-performance computing (HPC)
* Machine learning
* Enterprise migrations 

---

## 14. Hybrid Storage – AWS Storage Gateway

### What it Does

* Connects **on-premises environments** to AWS storage.
* Caches frequently accessed data locally.

### Gateway Types

1. **S3 File Gateway** → file-based access to S3
2. **Volume Gateway**

   * Cached mode
   * Stored mode
3. **Tape Gateway** → virtual tapes backed by S3/Glacier

### Use Cases

* Backup
* Archiving
* Hybrid cloud storage
* Gradual cloud migration 

---

## 15. Elastic Disaster Recovery (AWS DRS)

### Purpose

* Continuous block-level replication to AWS.
* Rapid recovery of physical & virtual servers.

### Benefits

* Minimal downtime
* Cost-effective DR
* No secondary data center needed
* Non-disruptive DR testing

### Exam Angle

* Used for **business continuity and disaster recovery**. 

---

## 16. Shared Responsibility Model – Storage

* **AWS**:

  * Hardware
  * Durability
  * Infrastructure
  * Availability
* **Customer**:

  * Data
  * Access control
  * Encryption configuration
  * Backup strategy 

---

## 17. Final Exam Takeaways (VERY IMPORTANT)

* **S3 ≠ EBS ≠ EFS**
* Databases → **EBS**
* Static content & backups → **S3**
* Shared file access → **EFS**
* Temporary data → **Instance Store**
* Long-term archives → **S3 Glacier / Deep Archive**
* Hybrid storage → **Storage Gateway**
* Disaster recovery → **Elastic Disaster Recovery**

---
