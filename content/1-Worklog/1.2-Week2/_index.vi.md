---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo. Vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn, bao gồm cả warning này.
{{% /notice %}} -->

### Mục tiêu Tuần 2:

* Chuyển tiếp từ kiến thức lý thuyết sang thực hành bài lab trong môi trường AWS.
* Triển khai, cấu hình và quản lý thành công các dịch vụ cốt lõi của AWS thông qua AWS Management Console và CLI.
* Hiểu cách triển khai thực tế của cloud security, networking, compute và monitoring.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Account Setup & Cost Management:** <br> - Tạo tài khoản AWS đầu tiên: Thiết lập root user, kích hoạt xác thực đa yếu tố (MFA) và cấu hình các cảnh báo chi phí ban đầu. <br> - Quản lý chi phí với AWS Budgets: Tạo các ngân sách tùy chỉnh để theo dõi lượng tài nguyên sử dụng và thiết lập các cảnh báo tự động khi chi phí vượt ngưỡng cho phép để tránh chi tiêu quá mức. <br> - Nhận hỗ trợ với AWS Support: Làm quen với trung tâm hỗ trợ, thực hành tạo các trường hợp hỗ trợ và khám phá các khuyến nghị của AWS Trusted Advisor. | 27/04/2026 | 27/04/2026 | https://000001.awsstudygroup.com/ <br> https://000007.awsstudygroup.com/ <br> https://000009.awsstudygroup.com/ |
| 3 | **Security & Core Infrastructure:** <br> - Quản lý truy cập với AWS IAM: Tạo IAM users và groups, gắn các quyền hạn chi tiết (policies) và áp dụng nguyên tắc đặc quyền tối thiểu. <br> - Networking Essentials với Amazon VPC: Xây dựng một Virtual Private Cloud (VPC) tùy chỉnh, cấu hình public/private subnets, route tables và Internet Gateways. <br> - Compute Essentials với Amazon EC2: Chạy một máy chủ ảo, cấu hình Security Groups và kết nối thành công qua SSH. | 28/04/2026 | 28/04/2026 | https://000002.awsstudygroup.com/ <br> https://000003.awsstudygroup.com/ <br> https://000004.awsstudygroup.com/ |
| 4 | **Advanced Access, Storage & Databases:** <br> - Instance Profiling với IAM Roles cho EC2: Gắn một IAM Role vào EC2 instance để truy cập an toàn các AWS APIs (như S3) mà không cần gắn cứng access keys. <br> - Static Website Hosting với Amazon S3: Cung cấp một S3 bucket, chỉnh sửa chính sách của bucket cho phép truy cập công khai và host một trang web HTML tĩnh. <br> - Database Essentials với Amazon RDS: Cung cấp một phiên bản cơ sở dữ liệu quan hệ được quản lý, cấu hình connection endpoints và thiết lập network security phù hợp. | 29/04/2026 | 29/04/2026 | https://000048.awsstudygroup.com/ <br> https://000057.awsstudygroup.com/ <br> https://000005.awsstudygroup.com/ |
| 5 | **Simplified Compute & Scalability:** <br> - Simplified Computing với Amazon Lightsail: Triển khai nhanh một ứng dụng Virtual Private Server (VPS) đã được cấu hình sẵn (VD: WordPress) sử dụng Lightsail. <br> - Container Deployment với Amazon Lightsail Containers: Push các Docker images và quản lý dễ dàng các ứng dụng container sử dụng container service của Lightsail. <br> - Scaling Applications với EC2 Auto Scaling: Tạo launch templates và cấu hình Auto Scaling Groups để tự động thêm hoặc xóa các instances dựa trên lưu lượng truyền tải. | 30/04/2026 | 30/04/2026 | https://000045.awsstudygroup.com/ <br> https://000046.awsstudygroup.com/ <br> https://000006.awsstudygroup.com/ |
| 6 | **Monitoring, DNS & CLI Operations:** <br> - Giám sát với Amazon CloudWatch: Tạo các dashboard tùy chỉnh, theo dõi các thông số của tài nguyên (như CPU utilization) và thiết lập CloudWatch Alarms. <br> - Hybrid DNS Management với Amazon Route 53: Cấu hình hosted zones, quản lý các bản ghi DNS và điều hướng người dùng đến các tài nguyên AWS đã triển khai. <br> - Command Line Operations với AWS CLI: Cài đặt CLI, cấu hình programmatic credentials và quản lý các dịch vụ AWS trực tiếp từ terminal. <br> **Research:** <br> - Nghiên cứu về AWS SDK cho Java. | 01/05/2026 | 01/05/2026 | https://000008.awsstudygroup.com/ <br> https://000010.awsstudygroup.com/ <br> https://000011.awsstudygroup.com/ <br> [Bài nghiên cứu về AWS SDK cho Java](https://tinyurl.com/38vddpc9) |


### Kết quả đạt được Tuần 2:

* Đạt được kinh nghiệm thực hành thông qua việc hoàn thành 15 bài thực hành lab bao quát các dịch vụ AWS thiết yếu.
* Xây dựng thành công một cơ sở hạ tầng đám mây cơ bản bảo mật, bao gồm custom networks (VPC), computing resources (EC2, Lightsail) và storage/databases (S3, RDS).
* Thiết lập cơ chế bảo mật phù hợp sử dụng IAM roles, policies và Security Groups.
* Nắm vững khả năng quản lý các tài nguyên AWS thông qua cả giao diện trực quan (Management Console) và bằng dòng lệnh (programmatically) qua AWS CLI.

<figure align="center">
  <img src="/images/1-Worklog/1.2-Week2/1.png"  width="100%">
  <figcaption><i>Hình 1: Kết nối vào EC2 bằng SSH thông qua VS Code nhưng bị lỗi</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.2-Week2/2.png"  width="100%">
  <figcaption><i>Hình 2: Bị lỗi Network Interface</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.2-Week2/3.png"  width="100%">
  <figcaption><i>Hình 3: Tạo thành công một máy chủ ảo EC2 Windows</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.2-Week2/4.png"  width="100%">
  <figcaption><i>Hình 4: Sử dụng dịch vụ Cloud9 để làm bài lab nhưng không còn được hỗ trợ</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.2-Week2/5.png"  width="100%">
  <figcaption><i>Hình 5: Sử dụng dịch vụ Amazon CloudWatch để theo dõi các thông số của máy chủ ảo</i></figcaption>
</figure>