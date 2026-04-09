# ☁️ Day 1 — AWS Fundamentals & Cloud Computing Basics

---

## 📌 Overview

On Day 1, I explored the core principles of cloud computing and the evolution of AWS as the world's leading cloud provider. The goal was to understand how cloud architecture solves traditional infrastructure challenges — covering pricing models, deployment models, service models, and AWS history.

---

## 📚 Topics Covered

- [AWS Pricing Models](#-aws-pricing-models)
- [Cloud Deployment Models](#-cloud-deployment-models)
- [Cloud Service Models — IaaS, PaaS, SaaS](#-cloud-service-models)
- [AWS History & Key Milestones](#-aws-history--key-milestones)

---

## 💰 AWS Pricing Models

AWS charges based on consumption. The model you choose determines your rate.

| Model | Discount vs On-Demand | Commitment | Best For |
|---|---|---|---|
| **Pay-as-you-go** | None (highest rate) | None | Beginners, unpredictable workloads |
| **Reserved Instances** | Up to 72% off | 1 or 3 years | Stable, long-running workloads |
| **Spot Instances** | Up to 90% off | None (interruptible) | Batch jobs, fault-tolerant workloads |
| **Savings Plans** | Up to 66% off | 1 or 3 years (spend commit) | Teams with predictable spend |
| **Free Tier** | 100% free (within limits) | None | Learning and experimentation |

### Key Insight
- **Pay-as-you-go** — default mode, most flexible, most expensive per hour. No upfront cost, no lock-in.
- **Reserved Instances** — you commit to a specific instance type for 1–3 years; AWS discounts you heavily.
- **Spot Instances** — AWS sells spare capacity at steep discounts. Caveat: AWS can reclaim them with 2 minutes' notice.
- **Savings Plans** — commit to a minimum hourly spend (e.g., $10/hr) rather than a specific instance type. More flexible than RIs.
- **Free Tier** — 12 months of limited free access to EC2, S3, Lambda, and more for new accounts.

> **For startups and learners:** Start with Pay-as-you-go. Graduate to Savings Plans once your workload is predictable. Use Spot Instances aggressively for any workload that can tolerate interruption.

---

## 🏗️ Cloud Deployment Models

| Model | Who Owns Hardware | Cost Profile | Best For |
|---|---|---|---|
| **On-premises** | You | High upfront, slow to scale | Government, regulated industries, legacy systems |
| **Cloud** | AWS / Provider | Pay per use, scales fast | Startups, variable workloads, global apps |
| **Hybrid** | Both | Moderate, complex to manage | Enterprises, compliance-heavy orgs, cloud migration phase |

### When to Use Each

- **On-premises** — when data sovereignty, compliance, or air-gapped security is non-negotiable (defense, banking, healthcare).
- **Cloud** — when speed, scale, and cost efficiency matter more than full hardware control. Default choice for modern startups.
- **Hybrid** — when you have existing on-prem infrastructure you can't or won't move, but still want to burst into the cloud for variable loads.

---

## 🧱 Cloud Service Models

Think of it as a spectrum of *how much AWS manages for you*.

```
You manage less  ◄─────────────────────────────────► You manage more
     SaaS              PaaS                IaaS
```

### IaaS — Infrastructure as a Service
AWS provides raw compute, storage, and networking. You manage everything above: OS, runtime, application, data.

- Maximum control, maximum responsibility.
- **AWS examples:** EC2 (virtual servers), S3 (object storage), VPC (networking)

### PaaS — Platform as a Service
AWS manages infrastructure AND the platform layer (OS, runtime, scaling). You focus on writing and deploying code only.

- No server patching. No manual load balancer config.
- **AWS examples:** Elastic Beanstalk (managed app deployment), Lambda (serverless functions), RDS (managed relational databases)

### SaaS — Software as a Service
A fully finished application. You log in and use it — zero infrastructure concern.

- **AWS examples:** Amazon WorkMail (email), Amazon Chime (video meetings), Amazon Connect (cloud call center)

---

## 🕰️ AWS History & Key Milestones

AWS didn't start as a cloud product. It started as Amazon's internal solution to its own infrastructure chaos — and became the backbone of the internet.

| Year | Milestone |
|---|---|
| **2002** | Amazon begins building internal web services to solve its own scaling problems |
| **2006** | AWS launches publicly with **S3** (object storage) and **EC2** (virtual servers) — the birth of commercial cloud computing |
| **2008** | Elastic Block Store (EBS) launches; AWS expands to multiple global regions |
| **2009** | **RDS** launches — managed relational databases, no DBA required |
| **2012** | First **AWS re:Invent** conference; **DynamoDB** (managed NoSQL) goes generally available |
| **2014** | **Lambda** launches — serverless computing, pay per function execution, no servers to manage |
| **2016** | AWS surpasses **$10 billion** in annual revenue, more profitable than Amazon's retail business |
| **2017–2020** | ML services surge: **SageMaker**, Rekognition, Comprehend — AWS becomes the default AI/ML platform |
| **2023–present** | **Bedrock** (foundation models as a service) and **Amazon Q** (enterprise AI) launch; AWS pivots into generative AI infrastructure |

> Today, AWS holds approximately **30–32% of the global cloud market** — more than Microsoft Azure and Google Cloud combined.

---

## ✅ Key Takeaways

- **Cloud economics** — Cloud shifts infrastructure from a capital expense (buy servers) to an operational expense (rent compute). This changes how businesses scale.
- **Pricing strategy matters** — Choosing the wrong pricing model can mean paying 3–10x more than necessary for the same workload.
- **Abstraction levels** — IaaS, PaaS, and SaaS represent increasing levels of managed abstraction. Where you operate depends on your team's expertise and control requirements.
- **AWS's dominance** — Built by solving Amazon's own scaling problems first. The internal necessity became the world's largest cloud platform.

---

## 🔗 Resources

- [AWS Pricing Calculator](https://calculator.aws/pricing/2/home)
- [AWS Free Tier](https://aws.amazon.com/free/)
- [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)
- [AWS Documentation](https://docs.aws.amazon.com/)

---

## 🏷️ Tags

`#7DaysOfAWS` `#AWSwithTWS` `#CloudComputing` `#AWS` `#DevOps` `#TrainWithShubham`

