---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu Tuần 5:

* Đào sâu chuyên môn về các dịch vụ bảo mật AWS, tập trung vào mã hóa dữ liệu, phát hiện mối đe dạo và quản lý credential.
* Nắm vững các cấu trúc mạng nâng cao để kết nối và quản lý nhiều VPCs một cách hiệu quả ở quy mô lớn.
* Hiểu rõ các kiến trúc tách rời và chuyển đổi quá trình triển khai ứng dụng sang các môi trường container sử dụng Docker, Amazon ECS và AWS CDK.
* Tính năng xem trang cá nhân và quên mật khẩu của dự án Mini Social Network được hoàn thiện.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Data Encryption & Credential Management:** <br> - Encryption với AWS Key Management Service (KMS): Tạo và quản lý các khóa mật mã để triển khai mã hóa dữ liệu khi lưu trữ cho nhiều dịch vụ của AWS. <br> - Data Protection với Amazon Macie: Sử dụng học máy để tự động phát hiện, phân loại và bảo vệ dữ liệu nhạy cảm (như PII) được lưu trữ trong Amazon S3. <br> - Credentials Management với AWS Secrets Manager: Lưu trữ, xoay vòng và truy xuất một cách an toàn các thông tin đăng nhập cơ sỡ dữ liệu và API keys mà không cần gắn cứng chúng vào ứng dụng. <br> **Project Mini Social Network:** <br> - Fix  lỗi "Coi trang cá nhân người khác hiện bản thân mình" <br> - Tính năng Quên mật khẩu (BE + FE). | 18/05/2026 | 18/05/2026 | https://000033.awsstudygroup.com/ <br> https://000090.awsstudygroup.com/ <br> https://000096.awsstudygroup.com/ <br> https://github.com/pht1412/Mini-Social-Network |
| 3 | **Threat Detection & Automated Patching:** <br> - Security Governance với AWS Firewall Manager: Cấu hình và quản lý tập trung các AWS WAF rules trên nhiều tài khoản và tài nguyên. <br> - Threat Detection với AWS GuardDuty: Bật tính năng phát hiện mối đe dọa thông minh và giám sát liên tục để phát hiện các hoạt động độc hại bên trong môi trường AWS. <br> - Systems Patching với EC2 Image Builder: Tự động hóa việc tạo, vá lỗi và triển khai các "Golden AMIs" (Amazon Machine Images) bảo mật và được tùy chỉnh. | 19/05/2026 | 19/05/2026 | https://000097.awsstudygroup.com/ <br> https://000098.awsstudygroup.com/ <br> https://000099.awsstudygroup.com/ |
| 4 | **Identity, Backup & Data Security:** <br> - Cross-Domain Authentication với Amazon Cognito: Triển khai xác thực người dùng, phân quyền và trải nghiệm đăng nhập liền mạch cho các ứng dụng web và mobile. <br> - S3 Security Best Practices (Advanced Review): Thực thi các bucket policies nghiêm ngặt, access points và mã hóa phía server để ngăn chặn rò rỉ thông tin. <br> - Data Protection với AWS Backup: Tập trung hóa và tự động hóa các chính sách sao lưu dữ liệu trên nhiều dịch vụ của AWS để đáp ứng các quy định. | 20/05/2026 | 20/05/2026 | https://000141.awsstudygroup.com/ <br> https://000069.awsstudygroup.com/ <br> https://000013.awsstudygroup.com/ |
| 5 | **Advanced Networking & Decoupling:** <br> - Network Integration với VPC Peering: Thiết lập các kết nối trực tiếp, kết nối không bắc cầu giữa hai VPCs để điều hướng traffic an toàn sử dụng địa chỉ IP riêng tư. <br> - Centralized Network Management với AWS Transit Gateway: Triển khai một cấu trúc mạng hình sao và trục để kết nối nhiều VPCs và mạng lưới on-premises một cách hiệu quả. <br> - Messaging Systems với SQS và SNS: Cấu hình các decoupled microservices sử dụng Amazon SQS (message queuing) và Amazon SNS (publish/subscribe notifications). | 21/05/2026 | 21/05/2026 | https://000019.awsstudygroup.com/ <br> https://000020.awsstudygroup.com/ <br> https://000077.awsstudygroup.com/ |
| 6 | **Containerization & Orchestration:** <br> - Containerization với Docker: Đóng gói mã nguồn của ứng dụng, runtime và các thư viện vào các Docker containers di động, gọn nhẹ. <br> - Container Orchestration với Amazon ECS: Định nghĩa các task definitions và triển khai các ứng dụng container một cách đáng tin cậy sử dụng Amazon Elastic Container Service. <br> - Infrastructure as Code cho ECS với CDK: Sử dụng AWS Cloud Development Kit (CDK) để cung cấp và quản lý các ECS clusters, dịch vụ và các thành phần mạng liên quan. | 22/05/2026 | 22/05/2026 | https://000015.awsstudygroup.com/ <br> https://000016.awsstudygroup.com/ <br> https://000118.awsstudygroup.com/ |

### Kết quả đạt được Tuần 5:

* Củng cố bảo mật hạ tầng bằng cách tích hợp AWS KMS cho khâu mã hóa, Secrets Manager cho credentials và GuardDuty cho phát hiện mối đe dọa liên tục.
* Đạt được kinh nghiệm thực hành trong việc xây dựng các kiến trúc mạng có thể mở rộng và có tính sẵn sàng cao sử dụng VPC Peering và AWS Transit Gateway.
* Thiết kế thành công một kiến trúc decoupled messaging sử dụng Amazon SQS và SNS để cải thiện khả năng phục hồi ứng dụng.
* Chuyển đổi sang các mô hình triển khai ứng dụng hiện đại bằng cách container hóa các ứng với Docker và tự động hóa việc triển khai Amazon ECS sử dụng AWS CDK.
* Tính năng xem trang cá nhân và quên mật khẩu của dự án Mini Social Network được hoàn thiện.


<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/7d168b611f6bef413547b9ad3f1345d29c6b3b3e">Hình 1: Commit code cho dự án Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/2.png"  width="100%">
  <figcaption><i>Hình 2: Tính năng xem trang cá nhân</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.5-Week5/3.png"  width="100%">
  <figcaption><i>Hình 3: Tính năng quên mật khẩu</i></figcaption>
</figure>