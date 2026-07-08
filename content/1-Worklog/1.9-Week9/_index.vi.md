---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu Tuần 9:

* Thiết kế và triển khai một hệ thống có khả năng mở rộng cao, hệ thống multi-type reaction có khả năng xử lý đồng thời cao.
* Tối ưu hóa render giao diện frontend, loại bỏ các nút nghẽn cổ chai của cơ sở dữ liệu trong backend và tăng cường bảo mật API chống lại spam.
* Tổng hợp các thành tựu kỹ thuật và kiến thức về kiến trúc hệ thống thành một cấu trúc bài đăng blog kỹ thuật hoàn chỉnh.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend - Architecture & Concurrency Control:** <br> - Di chuyển schema reaction sang một JSON-based Map linh hoạt để hỗ trợ multi-reaction types mà không cần thay đổi schema. <br> - Tối ưu hóa việc sử dụng bộ nhớ thông qua JPQL Constructor Expressions (`ReactionUserResponse`) cho DTO. <br> - Triển khai bộ nhớ đệm trong bộ nhớ (`ConcurrentHashMap` + `@Scheduled`) để ghi dữ liệu hàng loạt và giảm thiểu các nút nghẽn cổ chai khi xử lý đồng thời cao. <br> - Giải quyết các truy vấn N+1 sử dụng batch fetching và `HashMap` lookups, đồng thời triển khai cơ chế actionLock để ngăn chặn API spam. | 15/06/2026 | 15/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Frontend - UI/UX & Backend Debugging:** <br> - Giải quyết các lỗi không khớp dữ liệu Hibernate và vá các lỗi false-positive 403 Forbidden trong bộ lọc Spring Security. <br> - Triển khai giao diện "Hover to React" với trạng thái được quản lý tối ưu và tooltips thông minh (400ms) để ngăn chặn local DDoS từ các thao tác di chuột nhanh. <br> - Trích xuất `ReactionListDialog` cho mục đích lazy loading, giải quyết các vấn đề cắt xén giao diện avatar và cho phép điều hướng tới hồ sơ người dùng một cách dễ dàng. | 16/06/2026 | 16/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **Documentation & Knowledge Sharing:** <br> - Lên dàn ý (outline), bản nháp và cấu trúc nội dung kỹ thuật cho bài blog số 2, trình bày chi tiết về các kiến trúc được tối ưu hóa và kinh nghiệm phát triển gần đây. | 17/06/2026 | 17/06/2026 | [Tài liệu bài blog số 2](https://tinyurl.com/23f5rbm6) |
| 6 | **Team meeting:** <br> - Họp nhóm trực tiếp tại quán cà phê. | 19/06/2026 | 19/06/2026 | |


### Kết quả đạt được Tuần 9:

* Khả năng mở rộng và hiệu suất: Triển khai thành công một cơ chế tương tác có khả năng mở rộng cao. Cải thiện mạnh mẽ hiệu suất ứng dụng thông qua batching thao tác cơ sở dữ liệu, direct DTO projections và frontend debouncing.
* Tính ổn định và bảo mật của hệ thống: Tăng cường bảo mật hệ thống bằng cách giải quyết các các điểm bất thường trong Spring Security và triển khai các biện pháp bảo vệ giới hạn tốc độ ở cấp ứng dụng (thông qua cơ chế `actionLock`).
* Tài liệu kỹ thuật: Chuyển hóa các giải pháp kỹ thuật phức tạp thành tài liệu dễ tiếp cận thông qua việc khởi tạo bài blog kỹ thuật thứ hai.

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/2b1ba7a331b68933efd01d062c91cd82f5e9cc2a">Hình 1: Commit code cho dự án Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/2.png"  width="100%">
  <figcaption><i>Hình 2: Tính năng tương tác bài viết với nhiều lựa chọn cảm xúc</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/3.png"  width="100%">
  <figcaption><i>Hình 3: Danh sách người dùng đã tương tác với bài viết</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/4.png"  width="100%">
  <figcaption><i>Hình 4: Khu vực bình luận bài viết đã có tên và ảnh đại diện của người bình luận</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/5.png"  width="100%">
  <figcaption><i>Hình 5: Họp nhóm trực tiếp tại quán cà phê</i></figcaption>
</figure></i></figcaption>
</figure>