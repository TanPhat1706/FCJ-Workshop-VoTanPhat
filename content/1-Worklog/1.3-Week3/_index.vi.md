---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu Tuần 3:

* Đào sâu kiến thức thực tế về kiến trúc đám mây tiên tiến bao gồm caching, content delivery và serverless computing.
* Nắm vững tự động hóa hạ tầng và quản lý cấu hình sử dụng AWS Systems Manager, CloudFormation và AWS CDK.
* Tích hợp thành công ứng dụng local (với Java/Spring Boot) cùng các dịch vụ của AWS (Amazon S3, Amazon RDS).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Database, Caching & CDN:** <br> - NoSQL Database Essentials với Amazon DynamoDB: Cung cấp các bảng không quan hệ, quản lý phân vùng và thực thi các tác vụ CRUD. <br> - In-Memory Caching với Amazon ElastiCache: Cấu hình caching clusters để giảm độ trễ khi truy vấn cơ sở dữ liệu và cải thiện hiệu suất của ứng dụng. <br> - Content Delivery với Amazon CloudFront: Thiết lập một CDN distribution để tạo bộ nhớ đệm toàn cầu và cung cấp nội dung tĩnh/động an toàn tại các edge locations. | 04/05/2026 | 04/05/2026 | https://000060.awsstudygroup.com/ <br> https://000061.awsstudygroup.com/ <br> https://000061.awsstudygroup.com/ |
| 3 | **Directory Services, Migration & Serverless:** <br> - Directory Services với AWS Managed Microsoft AD: Triển khai và quản lý các dịch vụ directory trên cloud cho việc quản lý tài nguyên tập trung. <br> - VM Migration với AWS VM Import/Export: Thực hiện quá trình di chuyển các máy chủ on-premises sang các Amazon EC2 instances. <br> - Serverless Automation với AWS Lambda: Triển khai các event-driven, serverless functions để tự động hóa các tiến trình của backend mà không cần các máy chủ ảo. | 05/05/2026 | 05/05/2026 | https://000095.awsstudygroup.com/ <br> https://000014.awsstudygroup.com/ <br> https://000022.awsstudygroup.com/ |
| 4 | **Advanced Monitoring, Governance & Practical Integration:** <br> - Advanced Monitoring với CloudWatch và Grafana: Tích hợp các số liệu của CloudWatch với Grafana để trực quan hóa dữ liệu nâng cao. <br> - CloudWatch Advanced Workshop: Cấu hình các cảnh báo tổng hợp, số liệu tùy chỉnh và sử dụng CloudWatch Logs Insights. <br> - Resource Organization với Tags và Resource Groups: Triển khai các chiến lược gắn thẻ để nhóm và quản lý các tài nguyên AWS. <br> - Bài luyện tập số 1: Tích hợp AWS SDK cho Java vào một ứng dụng local Spring Boot để tải các tệp hình ảnh lên một Amazon S3 bucket. <br> - Bài luyện tập số 2: Cung cấp một Amazon RDS cho cơ sở dữ liệu SQL Server (Express Edition) và thiết lập thành công kết nối từ xa thông qua SSMS 20 cho quản trị viên. <br> **Meeting and study:** <br> - Lên văn phòng AWS để học tập, làm việc và họp nhóm. | 06/05/2026 | 06/05/2026 | https://000029.awsstudygroup.com/ <br> https://000036.awsstudygroup.com/ <br> https://000027.awsstudygroup.com/ |
| 5 | **Access Control & Systems Management:** <br> - Access Control với IAM và Resource Tags: Triển khai Attribute-Based Access Control (ABAC) sử dụng các thẻ tài nguyên cho các quyền hạn chi tiết. <br> - Systems Management với AWS Systems Manager: Tự động hóa các tiến trình vận hành, quản lý bản vá và cấu hình tài nguyên ở quy mô lớn. <br> - Remote Server Access với Systems Manager Session Manager: Thiết lập các phiên terminal an toàn, có thể kết nối được vào các EC2 instances mà không cần mở các cổng SSH (cổng 22) hay quản lý các bastion hosts. | 07/05/2026 | 07/05/2026 | https://000028.awsstudygroup.com/ <br> https://000031.awsstudygroup.com/ <br> https://000058.awsstudygroup.com/ |
| 6 | **Infrastructure as Code (IaC) & AWS CDK:** <br> - Infrastructure as Code với AWS CloudFormation: Cung cấp và quản lý hạ tầng của AWS sử dụng các declarative YAML/JSON templates. <br> - Cloud Development Kit (AWS CDK) Essentials: Định nghĩa cloud infrastructure as code sử dụng các ngôn ngữ lập trình quen thuộc thay vì declarative templates. <br> - AWS CDK Advanced: Xây dựng các cấu trúc tùy chỉnh có thể tái sử dụng và triển khai phức tạp, các kiến trúc đa tầng một cách có hệ thống. | 08/05/2026 | 08/05/2026 | https://000037.awsstudygroup.com/ <br> https://000038.awsstudygroup.com/ <br> https://000076.awsstudygroup.com/ |

### Kết quả đạt được Tuần 3:

* Nâng cấp các kỹ năng về kiến trúc thông qua việc triển khai thành công caching (ElastiCache), CDN (CloudFront), và serverless automation (Lambda).
* Tích hợp thành công các công cụ phát triển bên ngoài với AWS, thể hiện khả năng kết nối một ứng dụng local Spring Boot với Amazon S3 và quản lý các cơ sở dữ liệu đám mây từ xa thông qua SSMS 20.
* Tăng cường bảo mật và hiệu suất vận hành bằng cách sử dụng Systems Manager Session Manager và Attribute-Based Access Control (ABAC).
* Chuyển đổi từ thiết lập thủ công sang tự động hóa Infrastructure as Code (IaC) sử dụng cả hai hướng declarative (CloudFormation) và imperative (AWS CDK).

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/1.png"  width="100%">
  <figcaption><i>Hình 1: Tạo thành công dịch vụ Directory</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/2.png"  width="100%">
  <figcaption><i>Hình 2: Đăng tải thành công một tệp hình ảnh lên Amazon S3 từ ứng dụng local Spring Boot (Postman)</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/3.png"  width="100%">
  <figcaption><i>Hình 3: Đăng tải thành công một tệp hình ảnh lên Amazon S3 từ ứng dụng local Spring Boot (S3 Bucket)</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/4.png"  width="100%">
  <figcaption><i>Hình 4: Truy cập được tệp hình ảnh từ Amazon S3 thông qua một địa chỉ IP công khai</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/6.png"  width="100%">
  <figcaption><i>Hình 5: Tạo thành công cơ sở dữ liệu SQL Server trên RDS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/5.png"  width="100%">
  <figcaption><i>Hình 6: Kết nối thành công vào cơ sở dữ liệu SQL Server trên RDS thông qua SSMS 20</i></figcaption>
</figure>


<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/7.png"  width="100%">
  <figcaption><i>Hình 7: Thông tin các bảng trong cơ sở dữ liệu SQL Server trên RDS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/8.png"  width="100%">
  <figcaption><i>Hình 8: Học tập, làm việc và họp nhóm tại văn phòng AWS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/9.png"  width="100%">
  <figcaption><i>Hình 9: Học tập, làm việc và họp nhóm tại văn phòng AWS</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.3-Week3/10.png"  width="100%">
  <figcaption><i>Hình 10: Học tập, làm việc và họp nhóm tại văn phòng AWS</i></figcaption>
</figure>