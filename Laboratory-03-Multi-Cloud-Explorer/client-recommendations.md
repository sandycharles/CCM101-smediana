# Client Recommendations

## Client A – Startup Company

**Scenario:** Launching a new mobile application, limited budget, expects rapid growth.

**Recommended Platform:** AWS

**Justification:**

AWS is a good choice for a startup because its pay-as-you-go pricing model allows the company to use cloud resources without making a large upfront investment in hardware. AWS also provides services such as AWS Amplify and AWS Lambda that can help a small development team build and deploy applications quickly. Its auto-scaling capabilities allow the startup to increase resources as the number of users grows. In addition, AWS has a large ecosystem, extensive documentation, and many developer resources that can help the company solve technical problems efficiently.

**Services they could use:**
1. **AWS Amplify** – for quickly developing, hosting, and managing the backend of a mobile application.
2. **Amazon EC2 / AWS Lambda** – for scalable computing; Lambda is especially useful for serverless, event-driven workloads with pay-per-use pricing.
3. **Amazon DynamoDB** – for a scalable NoSQL database that can handle growing application traffic.
4. **Amazon S3** – for storing application assets, images, videos, backups, and other files at scalable storage capacity.

---

## Client B – University

**Scenario:** Already uses Windows Server, Microsoft 365, and Active Directory. Wants to migrate some services to the cloud.

**Recommended Platform:** Microsoft Azure

**Justification:**

Microsoft Azure is the best fit for the university because it integrates closely with the Microsoft technologies the institution already uses. Microsoft Entra ID can extend identity and access management to cloud applications while working with existing Microsoft environments. Azure also supports hybrid-cloud deployments, allowing the university to migrate workloads gradually instead of moving everything to the cloud at once. Services such as Azure Virtual Machines and Azure Virtual Desktop can also help the university move Windows-based applications and provide secure remote access to students and faculty.

**Services they could use:**
1. **Microsoft Entra ID** – for cloud-based identity and access management and integration with existing Microsoft environments.
2. **Azure Virtual Machines** – for migrating and running existing Windows Server workloads in the cloud.
3. **Azure Virtual Desktop** – for providing students, faculty, and staff with remote access to university applications and desktops.
4. **Azure Files** – for managed file shares that work well with Windows-based environments.

---

## Client C – AI Research Company

**Scenario:** Develops AI and Machine Learning applications requiring high-performance computing.

**Recommended Platform:** Google Cloud Platform (GCP)

**Justification:**

Google Cloud is a strong choice for an AI research company because it provides specialized infrastructure and services designed for artificial intelligence and machine learning workloads. Vertex AI provides tools for building, training, evaluating, and deploying machine learning models. Google Cloud also offers access to GPUs and Google's Tensor Processing Units (TPUs), which can provide high-performance acceleration for demanding AI workloads. In addition, Google Kubernetes Engine (GKE) is well suited for managing containerized research workloads at scale.

**Services they could use:**
1. **Vertex AI** – for building, training, evaluating, and deploying machine learning models.
2. **Compute Engine with GPUs/TPUs** – for high-performance computing and training large AI models.
3. **Google Kubernetes Engine (GKE)** – for orchestrating and scaling containerized AI and research workloads.
4. **BigQuery** – for analyzing large datasets that can be used in AI and machine learning pipelines.

---

## Client D – Global E-Commerce Company

**Scenario:** Multinational online shopping company, needs highly available infrastructure with automatic scaling.

**Recommended Platform:** AWS

**Justification:**

AWS is a strong choice for a global e-commerce company because it provides extensive worldwide infrastructure and services designed for highly available and scalable applications. Amazon EC2 Auto Scaling can automatically adjust computing resources according to changes in customer demand, which is especially useful during major sales and seasonal traffic spikes. Elastic Load Balancing can distribute incoming traffic across multiple resources, while Amazon CloudFront can deliver website content quickly to customers around the world. AWS also provides globally distributed database capabilities that can support reliable e-commerce applications and large-scale transactions.

**Services they could use:**
1. **Amazon EC2 Auto Scaling** – automatically adjusts computing capacity based on application demand.
2. **Elastic Load Balancing (ELB)** – distributes incoming application traffic across multiple servers and resources to improve availability.
3. **Amazon CloudFront** – provides fast global content delivery for websites, images, videos, and other e-commerce assets.
4. **Amazon Aurora Global Database** – provides a globally distributed relational database architecture suitable for applications requiring high availability and low-latency access.


## Checkpoint 6 – Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | AWS offers flexible pay-as-you-go pricing, introductory free-tier options, and a broad service catalog. These features allow a small team to control costs while having room to scale as the business grows. |
| Enterprise Organization | AWS | AWS provides a mature global infrastructure, extensive enterprise services, and a broad range of security and compliance capabilities. Its large ecosystem makes it suitable for organizations with complex and large-scale workloads. |
| Microsoft Environment | Azure | Azure provides strong native integration with Microsoft Entra ID, Microsoft 365, Windows Server, SQL Server, and other Microsoft technologies. This reduces migration complexity for organizations already using Microsoft's ecosystem. |
| AI / Machine Learning | GCP | Google Cloud provides specialized AI and ML infrastructure, including TPUs, along with Vertex AI for developing, training, and deploying machine learning models. Its strong background in AI research makes it a compelling choice for ML-heavy workloads. |
| Kubernetes Deployment | GCP | Google originally developed Kubernetes, and Google Kubernetes Engine (GKE) provides a mature managed Kubernetes platform. GKE offers integrated tools for deploying, managing, monitoring, and scaling containerized applications. |
| Global Web Application | AWS | AWS provides a large global infrastructure and services such as Amazon CloudFront, Elastic Load Balancing, and Amazon EC2 Auto Scaling. These services help deliver web applications with low latency, high availability, and the ability to handle traffic spikes. |

### Decision Summary

The decision matrix shows that there is no single cloud provider that is the best choice for every business requirement. **AWS** is a strong all-around option for startups, enterprises, and globally distributed applications because of its broad service selection and mature ecosystem. **Azure** is particularly suitable for organizations already invested in Microsoft technologies, while **GCP** stands out for artificial intelligence, machine learning, and Kubernetes workloads.

Organizations should select a cloud provider based on their specific requirements, existing technology environment, budget, technical expertise, security needs, and expected growth.

