☁️ Day 1: AWS Fundamentals & Cloud Journey
🎯 Learning Objectives
Today, I explored the core principles of cloud computing and the evolution of AWS as a global leader. My goal was to understand how cloud architecture solves traditional infrastructure challenges.

🎯 Tasks for Day 1
1. Understand AWS Pricing Models
   AWS charges you based on what you use. That's the core idea. But how you pay depends on the model you choose.
Pay-as-you-go is the default. You spin up a server, you pay by the hour (or second). You shut it down, you stop paying. No upfront cost, no long-term commitment. This is what most beginners start with — and honestly, it's the most expensive per-hour rate AWS offers.
Reserved Instances (RIs) are a commitment deal. You say to AWS: "I'll use this specific server type for 1 or 3 years." In return, AWS gives you up to 72% off compared to pay-as-you-go. Catch? You're locked in. Useful if you know your workload won't change.
Spot Instances are AWS selling unused server capacity at up to 90% discount. The brutal catch: AWS can take them back with 2 minutes notice when demand rises. You should only run workloads that can be interrupted — batch jobs, data processing, rendering.
Savings Plans are like RIs but more flexible. You commit to spending a fixed dollar amount per hour (e.g. $10/hr) over 1-3 years, and AWS gives you discounted rates across a wider range of services.
Free Tier exists for new accounts — 12 months of limited free usage on services like EC2, S3, and Lambda. Great for learning.
  ::view-transition-group(*),
  ::view-transition-old(*),
  ::view-transition-new(*) {
    animation-duration: 0.25s;
    animation-timing-function: cubic-bezier(0.19, 1, 0.22, 1);
  }
VvisualizeVvisualize show_widgetFor your LinkedIn post — be honest with your take. For startups/learners: Pay-as-you-go wins at the start (no commitment risk), then Savings Plans once you have a predictable workload. Spot Instances are gold for cost-cutting if your app can handle interruptions.

Task 2 — On-premises vs Cloud vs Hybrid
On-premises (on-prem) means you own and run the hardware. Servers sit in your building or data center. You buy them, rack them, maintain them, replace them when they die. You have full control — and full responsibility for everything.
Cloud means someone else (AWS, Azure, GCP) owns the hardware. You rent compute, storage, databases over the internet. You pay only for what you use. No hardware to manage.
Hybrid is both. Some workloads run in your own data center, some in the cloud. They're connected, usually via a private network.
  ::view-transition-group(*),
  ::view-transition-old(*),
  ::view-transition-new(*) {
    animation-duration: 0.25s;
    animation-timing-function: cubic-bezier(0.19, 1, 0.22, 1);
  }
VvisualizeVvisualize show_widget
Task 3 — IaaS, PaaS, and SaaS
Think of it as a spectrum of how much AWS manages for you.
IaaS — Infrastructure as a Service: AWS gives you raw infrastructure. You get a virtual machine, storage, networking — and you manage everything above that (OS, runtime, your app, your data). Maximum control, maximum responsibility.

EC2 (virtual servers), S3 (raw storage), VPC (networking)

PaaS — Platform as a Service: AWS manages the infrastructure AND the platform (OS, runtime, scaling). You just deploy your code. You don't patch servers. You don't configure load balancers manually.

Elastic Beanstalk (deploy apps without managing servers), Lambda (serverless functions — just write the function, AWS runs it), RDS (managed database — no DBA required)

SaaS — Software as a Service: AWS (or anyone) gives you a finished application. You just log in and use it. Zero infrastructure or platform concern.

Amazon WorkMail (email service), Amazon Chime (video meetings), Amazon Connect (call center software)

  ::view-transition-group(*),
  ::view-transition-old(*),
  ::view-transition-new(*) {
    animation-duration: 0.25s;
    animation-timing-function: cubic-bezier(0.19, 1, 0.22, 1);
  }
VvisualizeVvisualize show_widgetThe key insight: the more you move right (toward SaaS), the less you manage — but the less flexibility you have. Most cloud engineers spend their time in IaaS and PaaS territory.

Task 4 — AWS History & Key Milestones
AWS didn't start as a cloud company. It started as an internal Amazon infrastructure project — they needed a reliable, scalable internal platform to build Amazon.com. Then they realized: other companies need this too. So they sold access to it.
Here's the honest timeline:
2002 — Amazon.com launches internal web services internally. They're solving their own chaos.
2006 — AWS goes public with two landmark services: S3 (Simple Storage Service — store files in the cloud) and EC2 (Elastic Compute Cloud — rent virtual servers). This is the actual birth of cloud computing as a commercial product.
2008 — Elastic Block Store (EBS) and more regions launch. AWS starts building global infrastructure.
2009 — RDS launches (managed relational databases). You no longer need a DBA to set up Postgres or MySQL.
2012 — AWS re:Invent conference launches. This is their annual product dump event — still a huge deal today. DynamoDB (managed NoSQL) goes generally available.
2014 — Lambda launches. This is massive. Serverless computing — you write a function, AWS runs it, you pay per execution. No servers to manage at all.
2016 — AWS hits $10 billion in annual revenue. It's now a dominant business unit inside Amazon, more profitable than Amazon's retail arm.
2017–2020 — Machine learning services flood in: SageMaker (2017), Rekognition, Comprehend. AWS becomes the default platform for AI/ML workloads.
2023–present — Bedrock launches (foundation models as a service), Amazon Q (enterprise AI assistant). AWS pivots hard into generative AI infrastructure.
Today AWS holds roughly 30-32% of the global cloud market — more than Azure and Google Cloud combined.
