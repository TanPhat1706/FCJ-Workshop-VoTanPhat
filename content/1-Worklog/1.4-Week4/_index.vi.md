---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu Tuần 4:

* Nắm vững các chiến lược tối ưu chi phí nâng cao và quản lý AWS billing toàn diện.
* Nâng cao bảo mật hạ tầng bằng cách triển khai các chính sách IAM nâng cao, compliance hubs và network firewalls.
* Tự động hóa khâu quản lý vòng đời dữ liệu và tích hợp trực tiếp các công cụ phát triển của AWS vào local IDE.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **IaC, Optimization & Network Monitoring:** <br> - Infrastructure as Code Workshop Series: Đi sâu vào các mô hình IaC nâng cao để cung cấp và cập nhật các kiến trúc đám mây mạnh mẽ. <br> - Right-Sizing với EC2 Resource Optimization: Phân tích các số liệu về hiệu suất để chọn các loại instance phù hợp, cân bằng giữa chi phí và yêu cầu về tính toán. <br> - Network Monitoring với VPC Flow Logs: Bắt và phân tích IP traffic ra vào các network interfaces để khắc phục các vấn đề về kết nối và bảo mật. | 11/05/2026 | 11/05/2026 | https://000102.awsstudygroup.com/ <br> https://000032.awsstudygroup.com/ <br> https://000074.awsstudygroup.com/ |
| 3 | **Billing, Quotas & Cost Management:** <br> - Billing Console Delegation: Cấu hình các quyền hạn IAM để cung cấp an toàn quyền truy cập billing và cost management cho các non-root users cụ thể. <br> - Managing Quotas với Service Quotas: Chủ động theo dõi và quản lý các giới hạn tài nguyên của AWS để ngăn chặn các nút nghẽn kiến trúc trong quá trình mở rộng. <br> - Cost and Usage Management: Sử dụng AWS Cost Explorer và các công cụ thanh toán để phân tích mô hình chi tiêu và dự báo chi phí sử dụng trong tương lai. | 12/05/2026 | 12/05/2026 | https://000075.awsstudygroup.com/ <br> https://000063.awsstudygroup.com/ <br> https://000064.awsstudygroup.com/ |
| 4 | **Data Lifecycle & Developer Tools:** <br> - Snapshot Automation với Amazon EBS Data Lifecycle Manager: Tự động hóa việc tạo, giữ lại và xóa các EBS volume snapshots cho mục đích khắc phục thảm họa. <br> - Anomaly Detection cho EBS Backups: Triển khai machine learning-powered monitoring để phát hiện các hoạt động sao lưu bất thường hoặc không được phép. <br> - Development Environment với AWS Toolkit for VS Code: Cài đặt và cấu hình AWS extension trong VS Code để tương tác với các dịch vụ của AWS và debug các ứng dụng serverless trực tiếp dưới local. | 13/05/2026 | 13/05/2026 | https://000088.awsstudygroup.com/ <br> https://000089.awsstudygroup.com/ <br> https://000087.awsstudygroup.com/ |
| 5 | **Advanced Identity & Data Security:** <br> - Identity Federation với AWS Single Sign-On: Quản lý truy cập đa tài khoản tập trung và liên kết các tài khoản doanh nghiệp hiện có. <br> - Permission Management với IAM Permission Boundaries: Triển khai các IAM guardrails nâng cao để xác định quyền tối đa mà các chính sách identity-based có thể cấp. <br> - S3 Security Best Practices: Thực thi các bucket policies nghiêm ngặt, cấu hình Block Public Access và triển khai mã hóa cấp đối tượng. | 14/05/2026 | 14/05/2026 | https://000012.awsstudygroup.com/ <br> https://000030.awsstudygroup.com/ <br> https://000069.awsstudygroup.com/ |
| 6 | **Compliance & Network Security:** <br> - Security Compliance với AWS Security Hub: Tập trung hóa các cảnh báo bảo mật và tự động hóa các bước kiểm tra compliance dựa trên AWS Foundational Security Best Practices. <br> - Private Access cho S3 với VPC Endpoints: Cấu hình Gateway VPC Endpoints để điều hướng S3 traffic một cách an toàn trong mạng nội bộ của AWS, tránh việc đi qua internet công khai. <br> - Application Protection với AWS WAF: Triển khai một Web Application Firewall để bảo vệ các ứng dụng web hoặc các API khỏi các các lỗ hổng bảo mật web phổ biến và bot phá hoại. <br> **Team meeting**: <br> - Họp nhóm trực tiếp tại quán cà phê | 15/05/2026 | 15/05/2026 | https://000018.awsstudygroup.com/ <br> https://000111.awsstudygroup.com/ <br> https://000026.awsstudygroup.com/ |

### Kết quả đạt được Tuần 4:

* Nâng cấp khả năng phục hồi hạ tầng bằng cách tự động hóa sao lưu các EBS thông qua Data Lifecycle Manager và tính năng phát hiện hành vi bất thường.
* Đạt được kinh nghiệm thực tế về bảo mật cấp độ doanh nghiệp thông qua việc triển khai VPC Endpoints, IAM Permission Boundaries và AWS WAF.
* Xây dựng một tư duy "FinOps" vững chắc thông qua việc nắm vững EC2 right-sizing, giám sát chi phí và quản lý quota tự động.
* Tối ưu hóa quy trình phát triển nhờ tích hợp thành công AWS Toolkit trực tiếp vào Visual Studio Code.

<figure align="center">
  <img src="/images/1-Worklog/1.4-Week4/1.png"  width="100%">
  <figcaption><i>Hình 1: Cấu hình thành công S3 bucket để chứa nhật ký truy cập vào website của dự án</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.4-Week4/2.png"  width="fit">
  <figcaption><i>Hình 2: Họp nhóm trực tiếp tại quán cà phê</i></figcaption>
</figure>