---
title: "Event 2"
date: 2026-06-20
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

<!-- {{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}} -->

# Bài thu hoạch Cuộc thi “FCAJ AWS Cloud Architect”

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/0.png" width="100%">
</figure>

### Mục Đích Của Sự Kiện

- Ôn tập và củng cố toàn diện kiến thức về dịch vụ đám mây AWS thông qua hình thức "Gamification" (trò chơi hóa).
- Rèn luyện kỹ năng làm việc nhóm, quản trị rủi ro và tư duy ra quyết định chiến lược dưới áp lực thời gian.
- Tạo không gian kết nối (networking) và giải trí, giúp các thực tập sinh cân bằng giữa cường độ học tập cao và các hoạt động ngoại khóa.
- Đánh giá năng lực thiết kế hệ thống từ mức cơ bản đến chuyên sâu (Cloud Practitioner, Solutions Architect Associate - SAA, Solutions Architect Professional - SAP).

### Cấu Trúc & Thể Lệ Cuộc Thi

Cuộc thi diễn ra với sự tranh tài của **8 đội**, thi đấu trực tiếp qua các bộ câu hỏi. Mỗi vòng gồm 10 câu hỏi với điểm số tương ứng theo độ khó:
- **Cloud Practitioner:** 10 điểm/câu
- **SAA (Solutions Architect Associate):** 20 điểm/câu
- **SAP (Solutions Architect Professional):** 50 điểm/câu

#### Các Quyền Năng (Kỹ Năng Hỗ Trợ)
Mỗi đội được cung cấp 2 kỹ năng chiến thuật để thay đổi cục diện điểm số:
1. **Ngôi sao hy vọng (High Risk - High Reward):** Trả lời đúng được cộng gấp đôi số điểm, nhưng sai sẽ bị trừ gấp đôi số điểm của câu hỏi đó.
2. **Giảm thiểu rủi ro (Safe Play):** Trả lời đúng chỉ được cộng phân nửa (50%) số điểm, nhưng nếu sai sẽ không bị trừ điểm.

#### Lộ Trình Thi Đấu
- **Vòng loại (10 câu):** 7 câu Cloud Practitioner, 2 câu SAA, 1 câu SAP.
- **Vòng Bán kết (10 câu):** 5 câu Cloud Practitioner, 3 câu SAA, 2 câu SAP.
- **Vòng Chung kết (10 câu):** 3 câu Cloud Practitioner, 4 câu SAA, 3 câu SAP.

### Những Gì Học Được

#### Tư Duy Chiến Thuật và Quản Trị Rủi Ro
Việc sử dụng các quyền năng "Ngôi sao hy vọng" hay "Giảm thiểu rủi ro" rất giống với tư duy thiết kế kiến trúc phần mềm thực tế. Sẽ có những lúc cần chấp nhận rủi ro để tối ưu hóa hiệu suất (scale nhanh), nhưng cũng có những feature cốt lõi cần sự an toàn tuyệt đối (không bị trừ điểm/downtime) dù lợi ích mang lại thấp hơn. Điều này rèn luyện khả năng đánh giá Trade-off (Sự đánh đổi) – một kỹ năng sống còn của mọi Senior Developer/Solutions Architect.

#### Nền Tảng Kiến Trúc Đám Mây (Cloud Architecture)
Thông qua việc tiếp xúc với các câu hỏi chuẩn SAA và SAP, em nhận ra được các "blind spots" (điểm mù) trong kiến thức của mình về bảo mật, kết nối mạng và tối ưu chi phí trên AWS. Khối lượng kiến thức từ cuộc thi giúp củng cố bức tranh tổng thể khi thiết kế các ứng dụng phân tán.

### Ứng Dụng Vào Công Việc

- **Tư duy Fail-Fast & Safe Deployment:** Từ bài học "Giảm thiểu rủi ro" trong cuộc thi, em ứng dụng vào việc thiết lập các luồng CI/CD cho dự án hiện tại (NodeJS/Spring Boot). Triển khai theo từng phase nhỏ để hạn chế rủi ro ảnh hưởng đến PostgreSQL Database thay vì release toàn bộ.
- **Nâng cấp kiến trúc hệ thống:** Lấy cảm hứng từ các câu hỏi SAA/SAP để xem xét lại kiến trúc hiện tại của dự án: liệu hệ thống đã có tính sẵn sàng cao (High Availability) chưa, thiết kế cơ sở dữ liệu đã tối ưu I/O trên môi trường cloud chưa.

### Trải nghiệm trong sự kiện

Cuộc thi ngày 20/06 tại văn phòng AWS mang lại một làn gió rất mới trong suốt quá trình thực tập. Thay vì những buổi hội thảo thuần kỹ thuật, việc biến kiến thức thành một sàn đấu trực tiếp giúp mọi người hào hứng hơn rất nhiều.

Dù đội của chúng em đã phải dừng chân ngay từ vòng loại đầu tiên, nhưng đây lại là một trải nghiệm "thất bại" cực kỳ vui vẻ và bổ ích. 
- Thứ nhất, việc cọ xát với các câu hỏi SAA và SAP ngay từ vòng loại giúp em nhận ra biển kiến thức Cloud rộng lớn đến mức nào và bản thân cần phải nỗ lực trau dồi thêm.
- Thứ hai, sự kiện đã hoàn thành xuất sắc vai trò "vừa học vừa chơi". Được thi đấu cùng các anh em đồng nghiệp trong một không gian năng động, hiện đại của AWS giúp em giải tỏa căng thẳng và tăng tính gắn kết với mọi người.

Nhìn lại, việc "bị loại sớm" thực chất là một cơ hội để em ngồi dưới quan sát chiến thuật của các đội khác, học hỏi cách họ tư duy khi đưa ra lựa chọn và tiếp thu thêm được những kiến thức chuyên sâu trong các vòng Bán kết và Chung kết.

#### Một số hình ảnh khi tham gia sự kiện

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/1.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/2.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/3.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/4.png" width="100%">
</figure>

<figure align="center">
  <img src="/images/4-EventParticipated/4.2-Event2/5.png" width="100%">
</figure>

> Sự kiện khép lại với niềm vui và sự thoải mái. Thất bại trong một trò chơi là bước đệm tuyệt vời để thành công trong các dự án kiến trúc đám mây thực tế.