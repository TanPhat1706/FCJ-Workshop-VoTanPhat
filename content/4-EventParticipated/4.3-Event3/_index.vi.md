---
title: "Event 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

<!-- {{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}} -->

# Bài thu hoạch “FCAJ Community Day (Tháng 6)”

<figure align="center">
  <img src="/images/4-EventParticipated/4.3-Event3/0.png" width="100%">
</figure>

### Mục Đích Của Sự Kiện

- Khám phá các bước tiến mới trong việc tự động hóa vận hành hệ thống Cloud (Autonomous Operations).
- Giới thiệu các giải pháp Voice Agent và cách xây dựng trải nghiệm giao tiếp AI tự nhiên ở quy mô lớn.
- Cung cấp kiến thức chuyên sâu về việc ứng dụng AI Agents vào các quy trình DevOps và HR.
- Hướng dẫn thiết lập bảo mật kết nối nội bộ cho các mô hình ngôn ngữ thông qua chuẩn MCP (Model Context Protocol).

### Danh Sách Diễn Giả

- **Truong Tran** - AI Solution Sales Noventiq
- **Steve Tran** - CTO/Founder CloudThinker
- **Trung Vu** - CEO Revve AI
- **Anh Dang** - Solution Sales Noventiq
- **Nghi Danh** - AI Engineer Renova Cloud
- **Kiet Tran** - AI Engineer AWS Student Builder Group
- **Bao Phan** - Cloud Engineer Cloud Kinetics
- **Nguyen Nguyen** - Cloud Engineer Cloud Kinetics
- **Toan Nguyen** - AWS Security Builder

### Nội Dung Nổi Bật

#### Deep Response Engine: Từ Phát Hiện đến Tự Động Giải Quyết
- Phân tích bức tường phức tạp (complexity wall) trong vận hành Cloud hiện đại.
- Sự chuyển dịch mang tính chiến lược từ hệ thống phản ứng theo cảnh báo (alert-driven) sang hệ thống định hướng hành động (action-driven).
- Tổng quan kiến trúc Deep Response Engine, giúp tự động hóa phản hồi sự cố, từ đó giảm thiểu chi phí và hướng tới mục tiêu zero-downtime.

#### Voice Agents: Xây dựng Hội thoại AI giống Con người
- Quá trình tiến hóa từ hệ thống tổng đài IVR truyền thống và Chatbots lên AI Voice Agents.
- Giải quyết các thách thức cốt lõi: Độ trễ (latency), độ chính xác và tính tự nhiên trong tương tác.
- Giới thiệu Amazon Nova Sonic và mô hình nền tảng speech-to-speech.
- Kiến trúc tích hợp giữa telephony, streaming, Amazon Bedrock và các công cụ MCP.

#### AWS DevOps Agent: Trợ thủ Vận hành Luôn Sẵn Sàng
- Giới thiệu AWS DevOps Agent nhằm giảm thiểu thời gian phát hiện (MTTD) và thời gian phục hồi (MTTR) thông qua AI.
- Hỗ trợ giám sát và vận hành trong môi trường multi-cloud và hybrid.
- Áp dụng phương pháp suy luận đa tác vụ (multi-agent reasoning) với Bedrock AgentCore.
- Phân tích case study thực tế và demo vận hành trên nền tảng Amazon ECS.

#### Ứng dụng AI trong Năng suất: Hoạch định Nguồn nhân lực
- Các thách thức chuyển đổi số trong nghiệp vụ HR tại các doanh nghiệp lớn.
- Tận dụng Amazon Quick để tự động hóa hoạt động nhân sự và phân tích dữ liệu (Workforce analytics).
- Ứng dụng dữ liệu (data-driven insights) vào việc ra quyết định chiến lược cho doanh nghiệp.

#### Xây dựng Kết nối MCP Riêng tư và An toàn với Amazon Quick
- Vai trò của MCP (Model Context Protocol) trong việc mở rộng khả năng của hệ thống AI.
- Đánh giá các rủi ro bảo mật khi tích hợp AI qua MCP.
- Cấu hình VPC private connectivity cho Amazon Quick để đảm bảo luồng dữ liệu nội bộ được bảo vệ nghiêm ngặt.

### Những Gì Học Được

#### Tư Duy Kỹ Thuật & Kiến Trúc
- **Chuyển đổi mô hình vận hành:** Sự thay đổi từ "Alert-driven" sang "Action-driven" là bước tiến tất yếu cho các hệ thống phần mềm quy mô lớn, giúp giảm tải đáng kể cho đội ngũ kỹ sư trực hệ thống.
- **Tiêu chuẩn tích hợp AI an toàn:** Hiểu rõ cách thức hoạt động của Model Context Protocol (MCP) kết hợp cùng AWS VPC để tạo ra các đường hầm giao tiếp an toàn giữa AI Agent và dữ liệu nội bộ mà không làm rò rỉ thông tin ra public internet.
- **Tối ưu hóa độ trễ hệ thống:** Xử lý hội thoại thời gian thực với mô hình speech-to-speech yêu cầu kiến trúc streaming tối ưu để đạt được độ trễ thấp nhất.

#### Chiến Lược Phát Triển Tích Hợp
- Khai thác sức mạnh của Bedrock AgentCore để phối hợp nhiều Agent, cho phép mỗi AI xử lý một miền nghiệp vụ độc lập (từ DevOps đến phân tích HR) thay vì xây dựng một hệ thống quá cồng kềnh.

### Ứng Dụng Vào Công Việc

- **Triển khai tự động hóa DevOps:** Đánh giá khả năng tích hợp AWS DevOps Agent vào quy trình CI/CD hiện hành cho các ứng dụng backend (như Spring Boot và NodeJS). Sử dụng Agent để theo dõi logs và tự động xử lý các lỗi cơ bản khi deploy trên Amazon ECS.
- **Bảo mật dữ liệu nội bộ:** Áp dụng kiến trúc VPC private connectivity và chuẩn MCP khi cần tích hợp trợ lý AI (Amazon Quick) với các cơ sở dữ liệu quan hệ nội bộ như PostgreSQL, đảm bảo dữ liệu ứng dụng không bị lộ lọt.
- **Xây dựng hệ thống tự phục hồi:** Nghiên cứu áp dụng tư tưởng của Deep Response Engine để viết thêm các kịch bản tự động xử lý (auto-remediation scripts) cho backend, giúp hệ thống chủ động phản ứng thay vì chỉ gửi cảnh báo (alert) mỗi khi có tải cao hoặc lỗi database.

### Trải nghiệm trong sự kiện

Tham gia **FCAJ Community Day** tháng 6 tại văn phòng AWS Việt Nam mang lại cho em cái nhìn thực tế và sâu sắc hơn về cách thức các doanh nghiệp đang vận hành hệ thống đám mây kết hợp cùng trí tuệ nhân tạo.

#### Tiếp cận kiến trúc vận hành hiện đại
- Buổi chia sẻ về AWS DevOps Agent và Deep Response Engine rất ấn tượng. Dưới góc độ của một người làm phát triển phần mềm và hệ thống, việc chuyển đổi từ tư duy "chờ cảnh báo rồi sửa" sang "hệ thống tự động chuẩn đoán và xử lý" mở ra nhiều định hướng tối ưu kiến trúc.

#### Trải nghiệm công nghệ AI mới nhất
- Việc chứng kiến demo Voice Agents với Amazon Nova Sonic cho thấy sự trưởng thành của AI trong việc xử lý hội thoại với độ trễ gần như bằng không. Đồng thời, kiến thức về Model Context Protocol (MCP) đặc biệt hữu ích để định hướng việc mở rộng các plugin/công cụ cho hệ thống một cách bảo mật.

#### Không gian học hỏi và kết nối chuyên nghiệp
- Trải qua kỳ thực tập tại môi trường chuyên nghiệp giúp em liên tục được cập nhật các xu hướng từ những chuyên gia hàng đầu, từ đó rèn luyện phong cách làm việc và tư duy giải quyết vấn đề dưới góc nhìn của một kỹ sư thực thụ.

#### Một số hình ảnh khi tham gia sự kiện

<figure align="center">
  <img src="/images/4-EventParticipated/4.3-Event3/1.png" width="100%">
</figure>

> Những kiến thức từ sự kiện không chỉ có giá trị tham khảo mà còn định hình rõ nét lộ trình em muốn áp dụng để xây dựng và bảo mật các hệ thống backend tích hợp AI trong thời gian tới.