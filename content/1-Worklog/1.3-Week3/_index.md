---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 3 Objectives:

* Deepen practical knowledge in advanced cloud architectures including caching, content delivery and serverless computing.
* Master infrastructure automation and configuration management using AWS Systems Manager, CloudFormation and AWS CDK.
* Successfully integrate local application development (Java/Spring Boot) with cloud services (Amazon S3, Amazon RDS).

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Database, Caching & CDN:** <br> - NoSQL Database Essentials with Amazon DynamoDB: Provision NoSQL tables, manage partitions and execute CRUD operations. <br> - In-Memory Caching with Amazon ElastiCache: Configure caching clusters to reduce database query latency and improve application read performance. <br> - Content Delivery with Amazon CloudFront: Set up a CDN distribution to globally cache and deliver static/dynamic content securely at edge locations. | 05/04/2026 | 05/04/2026 | https://000060.awsstudygroup.com/ <br> https://000061.awsstudygroup.com/ <br> https://000061.awsstudygroup.com/
| 3 | **Directory Services, Migration & Serverless:** <br> - Directory Services with AWS Managed Microsoft AD: Deploy and manage directory services in the cloud for centralized resource administration. <br> - VM Migration with AWS VM Import/Export: Execute the migration process of on-premises virtual machine images into Amazon EC2 instances. <br> - Serverless Automation with AWS Lambda: Deploy event-driven, serverless functions to automate backend processes without provisioning servers. | 05/05/2026 | 05/05/2026 | https://000095.awsstudygroup.com/ <br> https://000014.awsstudygroup.com/ <br> https://000022.awsstudygroup.com/ |
| 4 | **Advanced Monitoring, Governance & Practical Integration:** <br> - Advanced Monitoring with CloudWatch and Grafana: Integrate CloudWatch metrics with Grafana for advanced data visualization and dashboarding. <br> - CloudWatch Advanced Workshop: Configure composite alarms, custom metrics and utilize CloudWatch Logs Insights. <br> - Resource Organization with Tags and Resource Groups: Implement tagging strategies to logically group and manage AWS resources. <br> - Practical Task 1: Integrated AWS SDK for Java within a local Spring Boot application to programmatically upload image assets to an Amazon S3 bucket. <br> - Practical Task 2: Provisioned an Amazon RDS for SQL Server (Express Edition) database and successfully established a remote connection via SSMS 20 for database administration. <br> **Meeting and study:** <br> -Study, work and team meeting at AWS office.| 05/06/2026 | 05/06/2026 | https://000029.awsstudygroup.com/ <br> https://000036.awsstudygroup.com/ <br> https://000027.awsstudygroup.com/ |
| 5 | **Access Control & Systems Management:** <br> - Access Control with IAM and Resource Tags: Implement Attribute-Based Access Control (ABAC) using resource tags for fine-grained permissions. <br> - Systems Management with AWS Systems Manager: Automate operational tasks, patch management and resource configuration at scale. <br> - Remote Server Access with Systems Manager Session Manager: Establish secure, auditable terminal sessions to EC2 instances without opening inbound SSH ports (port 22) or managing bastion hosts. | 05/07/2026 | 05/07/2026 | https://000028.awsstudygroup.com/ <br> https://000031.awsstudygroup.com/ <br> https://000058.awsstudygroup.com/ |
| 6 | **Infrastructure as Code (IaC) & AWS CDK:** <br> - Infrastructure as Code with AWS CloudFormation: Provision and manage AWS infrastructure using declarative YAML/JSON templates. <br> - Cloud Development Kit (AWS CDK) Essentials: Define cloud infrastructure as code using familiar programming languages rather than declarative templates. <br> - AWS CDK Advanced: Build custom reusable constructs and deploy complex, multi-stack architectures programmatically. | 05/08/2026 | 05/08/2026 | https://000037.awsstudygroup.com/ <br> https://000038.awsstudygroup.com/ <br> https://000076.awsstudygroup.com/ |


### Week 3 Achievements:

* Upgraded architectural skills by successfully implementing caching (ElastiCache), CDN (CloudFront), and serverless automation (Lambda).
* Successfully integrated external development tools with AWS, demonstrating the ability to connect a local Spring Boot application to Amazon S3 and manage cloud databases remotely via SSMS 20.
* Strengthened security and operational excellence by utilizing Systems Manager Session Manager and Attribute-Based Access Control (ABAC).
* Transitioned from manual console provisioning to automated Infrastructure as Code (IaC) using both declarative (CloudFormation) and imperative (AWS CDK) approaches.

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/1.png"  width="100%">
  <figcaption><i>Picture 1: Successfully created Directory service</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/2.png"  width="100%">
  <figcaption><i>Picture 2: Successfully uploaded an image asset to Amazon S3 from a local Spring Boot application (Postman)</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/3.png"  width="100%">
  <figcaption><i>Picture 3: Successfully uploaded an image asset to Amazon S3 from a local Spring Boot application (S3 Bucket)</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/4.png"  width="100%">
  <figcaption><i>Picture 4: Successfully accessed to S3 image asset from a public IP address</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/6.png"  width="100%">
  <figcaption><i>Picture 5: Successfully created a SQL Server database on RDS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/5.png"  width="100%">
  <figcaption><i>Picture 6: Successfully connected to a SQL Server database on RDS via SSMS 20</i></figcaption>
</figure>


<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/7.png"  width="100%">
  <figcaption><i>Picture 7: Tables in SQL Server database on RDS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/8.png"  width="100%">
  <figcaption><i>Picture 8: Study, work and team meeting at AWS office</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/9.png"  width="100%">
  <figcaption><i>Picture 9: Study, work and team meeting at AWS office</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/10.png"  width="100%">
  <figcaption><i>Picture 10: Study, work and team meeting at AWS office</i></figcaption>
</figure>