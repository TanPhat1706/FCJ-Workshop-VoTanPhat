---
title: "Event 1"
date: 2026-05-23
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

<!-- {{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}} -->

# Bài thu hoạch “FCAJ Community Day (Tháng 5)”

<figure align="center">
  <img src="/images/4-EventParticipated/4.1-Event1/0.png" width="100%">
</figure>

### Mục Đích Của Sự Kiện

- Chia sẻ kiến thức chuyên sâu về cách ứng dụng AI và xây dựng hệ thống Multi-Agent trong thực tế.
- Khám phá các giải pháp tối ưu hóa hạ tầng với Amazon CloudFront và các công cụ dữ liệu thông minh.
- Truyền cảm hứng thông qua trải nghiệm thực tế từ cuộc thi Hackathon và quá trình biến ý tưởng thành sản phẩm.
- Giải mã các đặc tính kỹ thuật cốt lõi của LLM (Large Language Models) trong quá trình inference.

### Danh Sách Diễn Giả

- **Vy Lam** - Senior Business System Analyst VPBank
- **Thao Nguyen** - GenAI Engineer VIB
- **Mai Nguyen** - GenAI Engineer VIB
- **Uyen Le** - GenAI Engineer VIB
- **Anh Pham** - Cloud Consultant G-AsiaPacific VietNam
- **Thinh Nguyen** - Devops Engineer FCAJ
- **Tinh Truong** - Platform Engineer GoTymeX
- **Duc Dao** - Solutions Architect Cloud Kinetics

### Nội Dung Nổi Bật

#### Tầm quan trọng của Ngữ cảnh (Context) trong AI
- Tại sao AI thường thất bại khi thiếu ngữ cảnh và định nghĩa thực sự của "ngữ cảnh".
- Sự tiến hóa từ Prompts sang Memory (khái niệm Second AI Brain).
- Cách ngữ cảnh chất lượng dẫn đến kết quả chính xác hơn và lời khuyên xây dựng AI cho sinh viên.

#### Trợ lý AI Amazon Quick
- **Quick Chat Agent:** Trợ lý AI giúp khám phá và phân tích insight dữ liệu.
- **Quick Flows & Spaces:** Tạo luồng công việc thông minh bằng ngôn ngữ tự nhiên (no-code) và không gian cộng tác nhóm.
- **Quick Sight:** Xây dựng dashboard và báo cáo từ dữ liệu thô bằng ngôn ngữ tự nhiên.

#### Nền tảng Amazon CloudFront
- CloudFront đáp ứng cho mọi workload từ edge đến origin.
- Các chiến lược tối ưu hóa chi phí, tăng cường bảo mật và độ tin cậy.
- Cải thiện hiệu suất hệ thống toàn diện.

#### 36 Giờ với LotusHacks – Xây dựng UTMorpho
- Hành trình từ số 0 đến ý tưởng, định hình bài toán thực tế.
- Phát triển dưới áp lực: 36 giờ sprint liên tục.
- Những thách thức, thất bại, bước ngoặt và bài học rút ra sau sự kiện.

#### Tính không tất định của LLM (Non-Determinism)
- Phân tích cách LLM lựa chọn next token.
- Phá vỡ lầm tưởng: Cài đặt `Temperature=0` không đảm bảo tính tất định 100%.
- Tác động thực tế của quá trình tối ưu hóa inference và các chiến lược giảm thiểu rủi ro (mitigation strategies).

#### Hệ thống Multi-Agent cấp Doanh nghiệp
- Case study: Chấm điểm tín dụng cho startup và sự chênh lệch cấu trúc dữ liệu so với hệ thống ngân hàng truyền thống.
- Khi nào nên dùng Single Agent và sức mạnh của Multi-Agent Paradigm.
- Bản vẽ kỹ thuật của Virtual Credit Committee (Hội đồng tín dụng ảo).
- Quản trị tuân thủ (Guardrails & Compliance) và lộ trình triển khai tối ưu ROI.

### Những Gì Học Được

#### Tư Duy Kỹ Thuật & Kiến Trúc
- **Tư duy hướng Context:** Trong phát triển ứng dụng AI, việc xây dựng hệ thống lưu trữ và truy xuất ngữ cảnh (Memory/Second Brain) quan trọng hơn việc chỉ tinh chỉnh prompt.
- **Kiến trúc Cloud-Native:** Tận dụng CDN (CloudFront) không chỉ để caching mà còn làm nền tảng bảo mật và tối ưu chi phí hạ tầng.
- **Multi-Agent Design:** Phân tách các tác vụ phức tạp (như chấm điểm tín dụng) thành nhiều Agent hoạt động độc lập sẽ an toàn và hiệu quả hơn một Single Agent ôm đồm mọi việc.

#### Kinh Nghiệm Thực Tế
- Hiểu rõ bản chất hoạt động của LLM dưới tầng suy luận (inference), từ đó thiết kế hệ thống có khả năng chịu lỗi (fault-tolerant) đối với các kết quả không tất định.
- Tư duy làm việc agile và xử lý khủng hoảng qua case study 36 giờ hackathon.

### Ứng Dụng Vào Công Việc

- **Tối ưu hóa các hệ thống AI đang phát triển:** Tích hợp quản lý context tốt hơn cho các tính năng trò chuyện/xử lý nghiệp vụ.
- **Áp dụng Amazon CloudFront:** Cấu hình CloudFront phân phối nội dung và API để giảm tải cho backend (như Spring Boot/NodeJS) và tăng cường bảo mật.
- **Nghiên cứu mô hình Multi-Agent:** Thử nghiệm thiết kế luồng xử lý dữ liệu phức tạp (như tổng hợp, đánh giá) bằng việc phối hợp nhiều AI Agents thay vì một model duy nhất.
- **Áp dụng chiến lược kiểm soát LLM:** Xây dựng các cơ chế xác thực kết quả (guardrails) khi gọi API LLM cho các dự án hệ thống, đặc biệt với những nghiệp vụ yêu cầu tính chính xác cao.

### Trải nghiệm trong sự kiện

Tham gia **FCAJ Community Day** tại tòa nhà Bitexco là một cơ hội tuyệt vời để em cập nhật những xu hướng công nghệ mới nhất về Cloud và AI. Một số trải nghiệm đáng nhớ:

#### Góc nhìn sâu sắc về AI và Cloud
- Các bài trình bày không chỉ dừng lại ở lý thuyết mà đi sâu vào các bài toán kỹ thuật hóc búa, điển hình như vấn đề "Non-Determinism" của LLM dù đã set temperature bằng 0.
- Nắm bắt được cách các dịch vụ như Amazon Quick và CloudFront giải quyết bài toán lớn về phân tích dữ liệu và tối ưu hiệu suất ở quy mô doanh nghiệp.

#### Bài học thực chiến và truyền cảm hứng
- Câu chuyện 36 giờ của Team VIB mang lại nguồn năng lượng rất lớn, giúp em học hỏi được cách quản lý thời gian, định hình scope dự án trong môi trường áp lực cao.
- Trải nghiệm không gian sự kiện chuyên nghiệp tại tầng 26 Bitexco cùng cộng đồng công nghệ chất lượng giúp em mở rộng tầm nhìn về lộ trình phát triển kiến trúc hệ thống hiện đại.

#### Một số hình ảnh khi tham gia sự kiện

<figure align="center">
  <img src="/images/4-EventParticipated/4.1-Event1/1.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.1-Event1/5.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.1-Event1/8.png" width="100%">
</figure>

> Sự kiện đã mang lại cho em những kiến thức thực tế quý giá, từ việc triển khai hệ thống phân tán trên AWS đến việc ứng dụng AI một cách thông minh và có kiểm soát vào các dự án phần mềm.