---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---
### Mục tiêu Tuần 7:

* Cập nhật cấu hình React frontend để thiết lập giao tiếp liền mạch với hạ tầng backend thông qua Application Load Balancer (ALB).
* Xây dựng và triển khai một ứng dụng web frontend lên AWS S3 cho public static website hosting.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Frontend API Endpoint Configuration:** <br> - Chỉnh sửa các tệp cấu hình môi trường bên trong mã nguồn React+Vite. <br> - Thay thế các local API endpoints bằng AWS Application Load Balancer (ALB) URL (production-ready) của dự án để thống nhất giao tiếp giữa Client-Server. | 01/06/2026 | 01/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Production Build & AWS S3 Static Website Hosting:** <br> - Biên dịch mã nguồn thành một production bundle được tối ưu hóa sử dụng công cụ xây dựng của Vite. <br> - Cung cấp và cấu hình một AWS S3 bucket cho Static Website Hosting. <br> - Tải lên các build artifacts và cấu hình các bucket policies cần thiết để xuất ra thành công đường dẫn web công khai. | 02/06/2026 | 02/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 5 | **Meeting and study:** <br> - Lên văn phòng AWS để học tập, làm việc và họp nhóm. | 04/06/2026 | 04/06/2026 |

### Kết quả đạt được Tuần 7:

* Tách rời thành công frontend và backend hosting bằng cách điều hướng an toàn các API requests thông qua AWS Application Load Balancer (ALB).
* Sinh ra thành công một production bundle tối ưu hóa và sẵn sàng triển khai của ứng dụng React+Vite.
* Triển khai web thành công sử dụng AWS S3 Static Website Hosting, đảm bảo đáng tin cậy và có thể truy cập công khai cho người dùng của ứng dụng.

<figure align="center">
  <img src="/images/1-Worklog/1.7-Week7/1.png"  width="100%">
  <figcaption><i>Hình 1: Triển khai thành công S3 bucket chứa ứng dụng frontend React+Vite</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.7-Week7/2.png"  width="100%">
  <figcaption><i>Hình 2: Truy cập thành công website dự án một cách công khai</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.7-Week7/3.png"  width="100%">
  <figcaption><i>Hình 3: Học tập, làm việc và họp nhóm tại văn phòng AWS</i></figcaption>
</figure>