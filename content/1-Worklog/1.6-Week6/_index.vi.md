---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu Tuần 6:

* Tối ưu hóa cơ sở dữ liệu và giải quyết các điểm quan trọng gây nghẽn hiệu suất bên trong ứng dụng Spring Boot (Data JPA).
* Triển khai toàn bộ vòng đời cho tính năng social Friend Request.
* Cải thiện hiệu suất ứng dụng React frontend, đặc biệt tập trung vào truy xuất dữ liệu, quản lý state và các thành phần rendering cycles của giao diện Admin.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend Optimization (JPA & Caching):** <br> - Phân tích các nhật ký thực thi truy vấn để xác định các thút thắt cổ chai về hiệu suất trong FeedService. <br> - Loại bỏ những truy vấn N+1 bằng cách triển khai Pre-warm L1 Cache và batch fetching cho original posts/media thông qua `findByIdInWithMedia`. <br> **Project Mini Social Network:** <br> - Cải thiện hệ thống: <br> &emsp; + Vào profile : nút kết bạn, nếu là bạn bè hiển thị "bạn bè", nếu không là bạn bè hiển thị và thực thi được nút "kết bạn" <br> &emsp; + Rà soát lại toàn bộ query để giảm số lượng câu query gọi xuống SQL Server.| 25/05/2026 | 25/05/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Backend Stability & Refactoring:** <br> - Giải quyết cảnh báo Hibernate in-memory pagination (HHH000104) trong `PostRepository` sử dụng `@EntityGraph`. <br> - Tái cấu trúc `PostService.mapToPostResponse` để ngăn chặn tình trạng đệ quy vô hạn (rủi ro StackOverflow). <br> - Áp dụng `@Transactional(readOnly = true)` cho các thao tác đọc và tái cấu trúc `toggleLike` để có cơ chế xử lý lỗi khéo léo. | 26/05/2026 | 26/05/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **Frontend - Social Features & Data Mapping:** <br> - Phát triển nút Friend Request trên trang cá nhân người dùng. <br> - Quản lý toàn bộ trạng thái vòng đời của friend request: Add Friend, Request Sent và Friends. <br> - Tái cấu trúc `PostManager.tsx` để ánh xạ và sử dụng chính xác cấu trúc JSON của `Page<T>` từ Spring Boot. | 27/05/2026 | 27/05/2026 | https://github.com/pht1412/Mini-Social-Network |
| 5 | **Frontend - Admin UI & Performance Optimization:** <br> - Triển khai phân trang mạnh mẽ phía server cho giao diện Admin sử dụng MUI TablePagination. <br> - Nâng cấp Admin Dashboard để hiển thị động (dynamically display) thống kê tương tác và xem trước các tệp hình ảnh/video từ bài viết. <br> - Tối ưu hóa chu kỳ tìm nạp dữ liệu trong React sử dụng `useCallback` hook để ngăn chặn render các thành phần vô hạn. | 28/05/2026 | 28/05/2026 | https://github.com/pht1412/Mini-Social-Network |
| 6 | **Team meeting:** <br> - Họp nhóm trực tiếp tại quán cà phê.| 29/05/2026 | 29/05/2026 | |

### Kết quả đạt được Tuần 6:

**Backend Performance & Stability:**
* Cải thiện đáng kể hiệu quả truy vấn bằng cách loại bỏ bài toán N+1 sử dụng L1 Cache pre-warming và batch fetching.
* Giải quyết thành công cảnh báo Hibernate in-memory pagination (HHH000104) bằng cách thay thế `JOIN FETCH` bằng `@EntityGraph`.
* Tăng cường sự ổn định của backend bằng cách giảm thiểu rủi ro StackOverflow trong quá trình ánh xạ DTO và giảm tranh chấp khóa cơ sở dữ liệu sử dụng `@Transactional(readOnly = true)`.

**Frontend UI/UX Enhancements:**
* Xây dựng thành công nút Friend Request (vòng đời các trạng thái Add, Sent, Friends) trang cá nhân.
* Nâng cấp Admin Dashboard thông qua việc triển khai phân trang phía server (handle cấu trúc `Page<T>` của Spring Boot qua MUI TablePagination) và thêm các khả năng xem trước các file hình ảnh/video từ bài viết.
* Tối ưu hóa vòng đời của thành phần React và loại bỏ triệt để render vô hạn thông qua việc triển khai chiến lược `useCallback` hook cho truy xuất dữ liệu.

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/b62e54e24524d1e2b0ed904ddf4e16408e3a0567">Hình 1: Commit code cho dự án Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/3.png"  width="100%">
  <figcaption><i>Hình 2: Giao diện Admin có phân trang và xem trước hình ảnh/video từ bài viết</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/4.png"  width="100%">
  <figcaption><i>Hình 3: Trạng thái bạn bè trên trang cá nhân</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/2.png"  width="100%">
  <figcaption><i>Hình 4: Họp nhóm trực tiếp tại quán cà phê</i></figcaption>
</figure>