---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu Tuần 10:

* Mở rộng các khả năng tương tác bằng cách triển khai một hệ thống multi-reaction toàn diện cho phần bình luận.
* Nâng cao trải nghiệm nhắn tin thời gian thực bằng cách tích hợp một công cụ chọn biểu tượng cảm xúc có khả năng thay đổi theme linh hoạt.
* Ổn định khâu hiển thị giao diện frontend bằng cách giải quyết các sự thay đổi về bố cục và tối ưu hóa thành phần của giao diện cho nhỏ gọn hơn.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend Architecture & Async Stability:** <br> - Di chuyển hệ thống tương tác bình luận từ một nút 'like' sang mô hình multi-reaction (LIKE, LOVE, HAHA, WOW, SAD, ANGRY). <br> - Tối ưu hóa các thao tác cơ sở dữ liệu sử dụng JPA Projections để truy xuất chính xác số lượt tương tác trong khi ngăn chặn các truy vấn N+1 thiếu hiệu quả. <br> - Chẩn đoán và giải quyết lỗi `LazyInitializationException` bên trong `NotificationService` bằng cách eagerly fetch các thực thể `User` cần thiết trước khi publish sự kiện. <br> - Tích hợp thư viện `react-reactions` để cung cấp các biểu tượng theo phong cách Facebook cho cả Post và Comment components. | 22/06/2026 | 22/06/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Frontend UX, Chatbox & UI Stabilization:** <br> - Tích hợp `emoji-picker-react` vào khung soạn tin nhắn, đảm bảo đồng bộ hóa động với global Dark/Light theme và văn bản dùng bảng mã Unicode. <br> - Loại bỏ thay đổi bố cục giao diện ("wobbly effect") trong các hover states bằng cách triển khai các wrapper có kích thước cố định và sử dụng MUI `<Popover>` với `disableScrollLock={true}` để ngăn chặn việc đóng băng khung hình và container clipping. <br> - Tái cấu trúc `CommentReactionButton` bằng cách thay thế các thành phần MUI bị phình to bằng các thành phần `Typography` nhẹ hơn để khôi phục tỷ lệ của bố cục. <br> - Triển khai một tiện ích `showDevelopmentAlert` sử dụng SweetAlert2 với conditional prop spreading để xử lý một cách khéo léo các tính năng "đang phát triển" trên website. | 23/06/2026 | 23/06/2026 | https://github.com/pht1412/Mini-Social-Network |

### Kết quả đạt được Tuần 10:

* Tính ổn định của hệ thống: Tăng cường quy trình thông báo bất đồng bộ bằng cách vượt qua thành công các giới hạn phiên Hibernate (`LazyInitializationException`).
* Tương tác được nâng cao: Triển khai thành công một hệ thống multi-reaction toàn diện cho phần bình luận và một công cụ chọn biểu tượng cảm xúc linh hoạt cho hộp thoại nhắn tin.
* Cải thiện UI/UX: Mang lại trải nghiệm giao diện người dùng liền mạch, không bị giật bằng cách giải quyết các thay đổi về bố cục, tối ưu hóa component rendering weights và triển khai thông báo thân thiện cho các tính năng sắp ra mắt.

<figure align="center">
  <img src="/images/1-Worklog/1.10-Week10/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/eefb219f23eda72d4004debeae9c65511771edfe">Hình 1: Commit code cho dự án Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.10-Week10/2.png"  width="100%">
  <figcaption><i>Hình 2: Bộ công cụ chọn emoji trong hộp thoại nhắn tin</i></figcaption>
</figure></i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.10-Week10/3.png"  width="100%">
  <figcaption><i>Hình 3: Các tính năng đang phát triển được thông báo qua pop-up thân thiện với người dùng hơn</i></figcaption>
</figure></i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.10-Week10/4.png"  width="100%">
  <figcaption><i>Hình 4: Các tương tác với bình luận đã có thông báo</i></figcaption>
</figure></i></figcaption>
</figure>