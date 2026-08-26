# Client Recommendations

## Client A – Startup Company
**Scenario:** Launching a new mobile application, limited budget, expects rapid growth.

**Recommended Platform:** AWS

**Justification:**
[Write 3–5 sentences. Talking points: AWS offers a generous free tier and pay-as-you-go pricing that suits limited startup budgets. Its broad service catalog and auto-scaling capabilities mean the startup won't need to migrate providers as it grows. AWS also has the largest developer community and documentation base, which helps small teams move fast without heavy vendor support.]

**Services they could use:**
1. **AWS Amplify** – for fast mobile app backend development
2. **Amazon EC2 / AWS Lambda** – for scalable compute (Lambda especially for pay-per-use, budget-friendly serverless)
3. **Amazon DynamoDB** – for a scalable NoSQL database that grows with user base
4. **Amazon S3** – for storing app assets/media at low cost

---

## Client B – University
**Scenario:** Already uses Windows Server, Microsoft 365, and Active Directory. Wants to migrate some services to the cloud.

**Recommended Platform:** Microsoft Azure

**Justification:**
[Write 3–5 sentences. Talking points: Azure offers native, seamless integration with Microsoft 365 and Active Directory (via Microsoft Entra ID), meaning the university can extend its existing identity and access setup to the cloud with minimal rework. Azure also supports hybrid cloud scenarios well through Azure Arc and Azure AD Connect, letting the university migrate gradually instead of all at once. Educational institutions also often qualify for Microsoft's academic licensing discounts.]

**Services they could use:**
1. **Microsoft Entra ID (Azure AD)** – extends existing on-prem Active Directory to the cloud
2. **Azure Virtual Machines** – to migrate Windows Server workloads directly
3. **Azure Virtual Desktop** – for remote student/faculty access to university applications
4. **Azure Files** – for shared file storage compatible with existing Windows environments

---

## Client C – AI Research Company
**Scenario:** Develops AI and Machine Learning applications requiring high-performance computing.

**Recommended Platform:** Google Cloud Platform (GCP)

**Justification:**
[Write 3–5 sentences. Talking points: GCP is widely regarded as the strongest platform for AI/ML workloads, offering purpose-built infrastructure like TPUs (Tensor Processing Units) that AWS and Azure don't have equivalents for. Its Vertex AI platform streamlines the ML lifecycle from training to deployment. GCP also originated Kubernetes, making GKE the most mature option for orchestrating containerized, high-performance research workloads.]

**Services they could use:**
1. **Vertex AI** – end-to-end platform for building, training, and deploying ML models
2. **Compute Engine with TPUs/GPUs** – high-performance computing for training large models
3. **Google Kubernetes Engine (GKE)** – for orchestrating containerized research workloads at scale
4. **BigQuery** – for large-scale data analysis feeding into ML pipelines

---

## Client D – Global E-Commerce Company
**Scenario:** Multinational online shopping company, needs highly available infrastructure with automatic scaling.

**Recommended Platform:** AWS

**Justification:**
[Write 3–5 sentences. Talking points: AWS has the largest global infrastructure footprint of the three providers, which matters directly for a multinational company needing low latency worldwide. Its auto-scaling and load-balancing services are mature and battle-tested at massive scale (Amazon's own retail business runs on it). AWS also offers strong CDN (CloudFront) and global database replication options suited to e-commerce traffic spikes during sales events.]

**Services they could use:**
1. **Amazon EC2 Auto Scaling** – automatically adjusts compute capacity based on demand
2. **Elastic Load Balancing (ELB)** – distributes traffic across regions for high availability
3. **Amazon CloudFront** – CDN for fast global content delivery
4. **Amazon Aurora (Global Database)** – highly available, globally distributed relational database

