---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 5 Objectives:

* Deepen expertise in AWS security services, focusing on data encryption, threat detection, and credential management.
* Master advanced networking topologies to connect and manage multiple VPCs efficiently at scale.
* Understand decoupled architectures and transition application deployment to containerized environments using Docker, Amazon ECS, and AWS CDK.
* Feature view profile and forgot password of project Mini Social Network will be completed.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Data Encryption & Credential Management:** <br> - Encryption with AWS Key Management Service (KMS): Create and manage cryptographic keys to implement encryption at rest for various AWS services. <br> - Data Protection with Amazon Macie: Utilize machine learning to automatically discover, classify, and protect sensitive data (like PII) stored in Amazon S3. <br> - Credentials Management with AWS Secrets Manager: Securely store, rotate, and retrieve database credentials and API keys without hardcoding them in applications. <br> **Project Mini Social Network:** <br> - Fix bug view profile. <br> - Feature forgot password (FE + BE). | 05/18/2026 | 05/18/2026 | https://000033.awsstudygroup.com/ <br> https://000090.awsstudygroup.com/ <br> https://000096.awsstudygroup.com/ <br> https://github.com/pht1412/Mini-Social-Network <br>
| 3 | **Threat Detection & Automated Patching:** <br> - Security Governance with AWS Firewall Manager: Centrally configure and manage AWS WAF rules across multiple accounts and resources. <br> - Threat Detection with AWS GuardDuty: Enable intelligent threat detection and continuous monitoring to identify malicious activities within the AWS environment. <br> - Systems Patching with EC2 Image Builder: Automate the creation, patching and deployment of secure, customized "Golden AMIs" (Amazon Machine Images). | 05/19/2026 | 05/19/2026 | https://000097.awsstudygroup.com/ <br> https://000098.awsstudygroup.com/ <br> https://000099.awsstudygroup.com/ |
| 4 | **Identity, Backup & Data Security:** <br> - Cross-Domain Authentication with Amazon Cognito: Implement user authentication, authorization and seamless sign-in experiences for web and mobile applications. <br> - S3 Security Best Practices (Advanced Review): Audit and enforce strict bucket policies, access points and server-side encryption to prevent data leaks. <br> - Data Protection with AWS Backup: Centralize and automate data backup policies across multiple AWS services to meet regulatory compliance. | 05/20/2026 | 05/20/2026 | https://000141.awsstudygroup.com/ <br> https://000069.awsstudygroup.com/ <br> https://000013.awsstudygroup.com/ |
| 5 | **Advanced Networking & Decoupling:** <br> - Network Integration with VPC Peering: Establish direct, non-transitive network connections between two VPCs to route traffic securely using private IP addresses. <br> - Centralized Network Management with AWS Transit Gateway: Implement a hub-and-spoke network topology to connect multiple VPCs and on-premises networks efficiently. <br> - Messaging Systems with SQS and SNS: Architect decoupled microservices using Amazon SQS (message queuing) and Amazon SNS (publish/subscribe notifications). | 05/21/2026 | 05/21/2026 | https://000019.awsstudygroup.com/ <br> https://000020.awsstudygroup.com/ <br> https://000077.awsstudygroup.com/ |
| 6 | **Containerization & Orchestration:** <br> - Containerization with Docker: Package application code, runtime and dependencies into portable, lightweight Docker containers. <br> - Container Orchestration with Amazon ECS: Define task definitions and deploy containerized applications reliably using Amazon Elastic Container Service. <br> - Infrastructure as Code for ECS with CDK: Use AWS Cloud Development Kit (CDK) to programmatically provision ECS clusters, services and associated networking components. | 05/22/2026 | 05/22/2026 | https://000015.awsstudygroup.com/ <br> https://000016.awsstudygroup.com/ <br> https://000118.awsstudygroup.com/ |


### Week 5 Achievements:

* Fortified infrastructure security by integrating AWS KMS for encryption, Secrets Manager for credentials and GuardDuty for continuous threat detection.
* Gained hands-on experience in building scalable and highly available network architectures using VPC Peering and AWS Transit Gateway.
* Successfully designed a decoupled messaging architecture utilizing Amazon SQS and SNS to improve application resilience.
* Transitioned to modern application deployment paradigms by containerizing applications with Docker and automating Amazon ECS deployments using AWS CDK.
* Feature view profile and forgot password of project Mini Social Network are completed.

<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/7d168b611f6bef413547b9ad3f1345d29c6b3b3e">Picture 1: Commit code for project Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/2.png"  width="100%">
  <figcaption><i>Picture 2: Feature view profile</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/3.png"  width="100%">
  <figcaption><i>Picture 3: Feature forgot password</i></figcaption>
</figure>