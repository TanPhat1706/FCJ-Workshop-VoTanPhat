---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu Tuần 8:

* Đại tu (overhaul) các chức năng hệ thống cốt lõi và làm ổn định các AWS S3 media.
* Truy tìm và giải quyết các lỗi quản lý state nghiêm trọng trong hệ thống thông báo và các chức năng social.
* Đạt được sự đồng bộ tính năng giữa môi trường phát triển và môi trường production cho các chức năng quản lý bài đăng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Cloud Storage Integration (Media Fix):** <br> - Truy tìm và debug lỗi đăng tải video thất bại lên AWS S3. <br> - Sửa các cấu hình multipart tải lên và đảm bảo xử lý kiểu MIME chính xác để khôi phục thành công khả năng tải video lên. | 08/06/2026 | 08/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **State Management & Data Mapping:** <br> - Notification System: Tái cấu trúc vòng đời của thông báo để giải quyết lỗi trạng thái "stuck unread", đảm bảo các trạng thái đã đọc/chưa đọc hoạt động chuẩn xác. <br> - Social Features: Debug và sửa lỗi API response/state management gây ra tình trạng số lượng bạn bè của người dùng hiển thị sai (bằng 0). | 09/06/2026 | 09/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **UI/UX Bug Scrub (Mini Game Module):** <br> - Kiểm tra mô đun Mini Game module để xác định các lỗi trên giao diện. <br> - Vá các lỗi giao diện bằng cách hồi phục các image assets bị thiếu và giải quyết các vấn đề về kiểu chữ/hiển thị phông chữ trên các trình duyệt khác nhau. | 10/06/2026 | 10/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 5 | **Feature Migration & Environment Parity:** <br> - Đồng bộ các tính năng quản lý bài đăng từ môi trường phát triển sang môi trường production. <br> - Tích hợp, cấu hình và kiểm thử thành công các "Edit Post" và "Delete Post" API endpoints cũng như thành phần giao diện trên môi trường production. | 11/06/2026 | 11/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 6 | **Meeting and study:** <br> - Lên văn phòng AWS để học tập, làm việc và họp nhóm. | 12/06/2026 | 12/06/2026 |


### Kết quả đạt được Tuần 8:

* Tính ổn định của hệ thống: Khôi phục toàn bộ multimedia capabilities bằng cách giải quyết dứt điểm các vấn đề về quy trình tải video lên AWS S3.
* Trải nghiệm người dùng (UX): Loại bỏ các lỗi trạng thái nghiêm trọng trong hệ thống thông báo và các lỗi hiển thị giao diện người dùng bên trong mô đun Mini Game, cải thiện đáng kể sự hài lòng của người dùng.
* Sự tương đồng về triển khai: Di chuyển thành công các thao tác CRUD thiết yếu (Edit/Delete posts) lên cloud, đảm bảo tính nhất quán khi vận hành giữa môi trường phát triển và môi trường production.

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/51d501ed9195d001235a081be0397c355852ca82">Hình 1: Commit code cho dự án Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/2.png"  width="100%">
  <figcaption><i>Hình 2: Trạng thái đã đọc/chưa đọc của thông báo hoạt động chuẩn xác</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/3.png"  width="100%">
  <figcaption><i>Hình 3: Số lượng bạn bè hiển thị chính xác</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/4.png"  width="100%">
  <figcaption><i>Hình 4: Giao diện Mini Game đã có hình ảnh và phông chữ không còn lỗi</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/5.png"  width="100%">
  <figcaption><i>Hình 5: Giao diện chỉnh sửa bài viết</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/6.png"  width="100%">
  <figcaption><i>Hình 6: Giao diện xóa bài viết</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/7.png"  width="100%">
  <figcaption><i>Hình 7: Lên văn phòng AWS để học tập, làm việc và họp nhóm</i></figcaption>
</figure>