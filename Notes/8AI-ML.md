# AWS Cloud Practitioner – Module 8: AI & ML

**Complete Exam-Focused Summary**

---

## 1. Why AI & ML Matter (Business Motivation)

* Businesses want to:

  * Predict demand (inventory forecasting)
  * Personalize recommendations
  * Detect trends and anomalies
* Traditional rule-based systems:

  * Static
  * Hard-coded
  * Poor at adapting to change
* AI/ML uses **data + learning** to make **dynamic, intelligent decisions**. 

---

## 2. What is Artificial Intelligence (AI)?

* **AI** is the broad field of creating systems that perform **human-like tasks**:

  * Understanding language
  * Recognizing speech or images
  * Making decisions
* Examples:

  * Conversational kiosks
  * Voice assistants
  * Intelligent recommendation engines

AI = **big umbrella** concept. 

---

## 3. What is Machine Learning (ML)?

* **ML is a subset of AI**.
* Machines learn patterns from **historical data**, not hard-coded rules.
* Core ML process:

  1. Collect data
  2. Train a model
  3. Use the model to make predictions (inference)

### Key Benefit

* Systems improve automatically as more data is collected.

Example:

* Personalized product recommendations instead of fixed “if-else” rules. 

---

## 4. Data Requirements for AI/ML (VERY IMPORTANT)

* AI/ML success depends on:

  * Large volumes of data
  * Clean, well-organized data
* Data sources:

  * Sales
  * Logs
  * Sensors
  * User activity
  * Social media

❗ Poor data → poor predictions (exam favorite concept). 

---

## 5. AWS AI/ML Stack – Three-Tier Model (EXAM CORE)

AWS provides **three levels** of AI/ML services.

---

### Tier 1: Pre-built AI Services (No ML Expertise Needed)

* Ready-to-use
* Pre-trained models
* Fastest time to value

#### Examples:

* **Amazon Comprehend** – sentiment & text analysis
* **Amazon Polly** – text-to-speech
* **Amazon Transcribe** – speech-to-text
* **Amazon Translate** – language translation
* **Amazon Rekognition** – image/video analysis
* **Amazon Textract** – extract text from documents
* **Amazon Lex** – chatbots
* **Amazon Personalize** – recommendations

✅ Use when you want **AI without building ML models**. 

---

### Tier 2: ML Services – Amazon SageMaker AI

* For **custom ML models**
* Fully managed end-to-end ML platform

#### SageMaker Capabilities:

* Data preparation
* Model training
* Experiment tracking
* Deployment
* Monitoring

Use when:

* You want custom models
* But don’t want to manage infrastructure 

---

### Tier 3: ML Frameworks & Infrastructure

* For advanced, specialized ML workloads
* Requires deep ML expertise

#### Examples:

* TensorFlow / PyTorch on EC2
* ML-optimized EC2 (GPU, Trainium, Inferentia)
* Amazon EMR for large-scale ML processing

Use when:

* You need full control and custom research-level solutions 

---

## 6. When to Use Which AI/ML Tier (EXAM TABLE)

| Requirement       | AWS Solution          |
| ----------------- | --------------------- |
| Fast AI features  | Pre-built AI Services |
| Custom ML models  | Amazon SageMaker      |
| Advanced ML infra | Frameworks & EC2      |

---

## 7. Deep Learning & Generative AI

### Deep Learning

* Uses **multi-layer neural networks**
* Excels at:

  * Vision
  * Speech
  * Language understanding

### Generative AI

* A type of deep learning
* Can **create new content**:

  * Text
  * Images
  * Music
  * Code

Powered by:

* **Foundation Models (FMs)**
* **Large Language Models (LLMs)** 

---

## 8. Generative AI on AWS (HIGH EXAM VALUE)

### Amazon SageMaker JumpStart

* Hub of:

  * Pre-trained ML & generative models
* Rapid deployment
* Optional fine-tuning

### Amazon Bedrock

* Fully managed service to:

  * Access multiple foundation models via one API
* Secure, enterprise-ready
* No infrastructure management

### Amazon Q

* AI assistant powered by generative AI

#### Variants:

* **Amazon Q Business** – internal business assistant
* **Amazon Q Developer** – coding assistant



---

## 9. Key Generative AI Definitions (MEMORIZE)

| Term             | Meaning                               |
| ---------------- | ------------------------------------- |
| Deep Learning    | ML using multi-layer neural networks  |
| Generative AI    | AI that creates new content           |
| Foundation Model | Large pre-trained multi-purpose model |
| LLM              | Language-focused foundation model     |

---

## 10. Introduction to Data Analytics

* Data analytics:

  * Explains **what happened**
  * Identifies trends and insights
* Still essential alongside AI/ML
* Best for:

  * Historical analysis
  * Smaller datasets
  * Transparency & explainability 

---

## 11. Data Lakes, ETL & Pipelines

### Data Lake

* Centralized storage for **all data types**
* Typically built on **Amazon S3**

### ETL / ELT

* **ETL**: Extract → Transform → Load
* **ELT**: Extract → Load → Transform
* Pipelines automate these steps

Clean data = foundation for analytics & ML. 

---

## 12. AWS Analytics Services (EXAM IMPORTANT)

| Stage         | AWS Services               |
| ------------- | -------------------------- |
| Ingestion     | Kinesis, Firehose          |
| Storage       | Amazon S3, Amazon Redshift |
| Processing    | AWS Glue, Amazon EMR       |
| Querying      | Amazon Athena              |
| Visualization | Amazon QuickSight          |
| Search & Logs | Amazon OpenSearch          |

---

## 13. End-to-End Analytics + ML Workflow (REAL EXAM SCENARIO)

Typical flow:

1. App data → DynamoDB
2. Stream data → Kinesis / Firehose
3. Transform → AWS Lambda
4. Store → Amazon S3 (data lake)
5. Catalog → AWS Glue
6. Query → Amazon Athena
7. Train models → Amazon SageMaker
8. Visualize → QuickSight

Same data supports:

* Analytics
* BI
* ML training



---

## 14. Final Exam Takeaways (CRITICAL)

* AI ≠ ML (ML is a subset)
* Data quality matters more than algorithms
* AWS AI/ML is **tiered**
* Use pre-built AI for speed
* Use SageMaker for custom ML
* Generative AI uses foundation models
* Analytics + ML work **together**, not separately

---
