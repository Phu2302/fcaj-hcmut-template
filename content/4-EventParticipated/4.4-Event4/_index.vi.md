---
title: "Sự kiện 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---
# Bài thu hoạch "Agentic AI Build Week & One Team Community Day: Hành trình sáng tạo và làm chủ giải pháp AI trên AWS"

### Mục đích của sự kiện

- **Tiếp cận bài toán thực tế của AI Agent:** Tìm hiểu cách xây dựng các trợ lý AI có khả năng tự động hành động (Agentic AI) giải quyết các bài toán phức tạp trong doanh nghiệp và đời sống.
- **Học hỏi tư duy thiết kế kiến trúc Đa kênh (Multi-channel):** Tích hợp AI Agent vào các nền tảng chat phổ biến như Zalo, Messenger, WhatsApp.
- **Trải nghiệm thực chiến 24h Hackathon:** Lắng nghe chia sẻ kinh nghiệm, áp lực thời gian và bài học rút ra từ các đội thi xuất sắc tại Agentic AI Build Week (AABW).
- **Ứng dụng AI vào quy trình kỹ thuật chuyên sâu:** Tìm hiểu các ứng dụng AI Native hỗ trợ Kiến trúc sư giải pháp (Solutions Architect) tự động hóa sơ đồ kiến trúc, mã IaC và ước tính chi phí AWS.
- **Phân tích dữ liệu & Tín hiệu doanh nghiệp:** Khám phá cách kết hợp mô hình Multi-Agent Architecture với Web Crawler để phân tích và cảnh báo tái cấu trúc doanh nghiệp.

### Danh sách diễn giả & Các đội ngũ chia sẻ

- **Dự án KFC Bot Agent (Đội One Team):** Anh Duy, Trần Đông, Đoàn Trung, Minh Việt, Anshul Roy.
- **Dự án S.H.E.P.H.E.R.D (Đội 3KA):** Huỳnh An Khương, Nguyễn Quốc Huy, Ngô Quang Khôi, Hoàng Lê Thành Đức, Đặng Nguyễn Phước Lộc.
- **Dự án SA Professional AI Native App (Đội Plan V):** Phạm Tiến Thuận, Phát Huỳnh, Hoàng Long, Lê Minh Nghĩa, Trần Đại Vĩ, Nguyễn An.
- **Dự án Signal Scout (Đội Dream AI Team):** Lê Tấn Lực, Đỗ Hoàng Hiếu, Triệu Quốc Hào, Nguyễn Văn Duy Khiêm, Nguyễn Công Minh, Nguyễn Trần Minh Quân.

---

### Nội dung nổi bật

#### 1. KFC Bot Agent – Trợ lý AI đặt hàng đa kênh (Đội One Team)

- **Bối cảnh & Vấn đề thực tế:** Đặt hàng bằng giọng nói/chat là một bài toán hệ thống cực kỳ phức tạp. Dẫn chứng từ việc McDonald's từng phải hủy thử nghiệm AI tại 100 cửa hàng Drive-thru cho thấy: ngôn ngữ tự nhiên thì lộn xộn nhưng quy tắc kinh doanh (khuyến mãi, biến thể món ăn, trạng thái giỏ hàng) lại rất nghiêm ngặt. Việc bắt khách hàng thoát ứng dụng nhắn tin (Zalo, Messenger) để chuyển sang app đặt đồ ăn khiến tỷ lệ rơi rụng đơn hàng (Lost Order) rất cao.
- **Giải pháp & Giá trị cốt lõi:** KFC Bot Agent cho phép người dùng **"Đặt hàng mà không cần rời khỏi cuộc trò chuyện"**. Khách hàng không cần tạo tài khoản mới, không phải chuyển app, giảm sự phụ thuộc vào tổng đài viên.
- **Cơ chế 5 bước hành động của Agent:**
  1. *Mục tiêu (Goal):* Hiểu ý định đặt hàng.
  2. *Kế hoạch (Plan):* Quyết định các bước xử lý.
  3. *Công cụ (Tools):* Tra cứu dữ liệu kinh doanh đáng tin cậy.
  4. *Hành động (Act):* Cập nhật giỏ hàng & áp mã giảm giá.
  5. *Xác thực (Verify):* Kiểm tra lại giỏ hàng thực tế.
- **Kiến trúc "Design Once | Deploy Everywhere":**
  * *Luồng đa kênh:* Tin nhắn từ Zalo, WhatsApp, Telegram... đi qua các Channel Adapters để chuẩn hóa thành `Normalized Message`, sau đó đưa vào nền tảng **One Agent Platform** (suy luận, tools, guardrails, memory).
  * *Hạ tầng AWS:* Kết hợp WAF, API Gateway, Lambda, SQS, AgentCore Gateway, Amazon Bedrock AgentCore, DynamoDB (State/Session), OpenSearch, ElastiCache, S3 và các cổng thanh toán/giao hàng.
- **Bốn con số hiệu suất ấn tượng:**
  * **$0.006 / đơn hàng:** Chi phí vận hành cực rẻ (tính trên 500 đơn/ngày).
  * **$88 / tháng:** Tổng chi phí hạ tầng (Amazon Bedrock chiếm 75%).
  * **3 - 5 giây:** Độ trễ phản hồi tin nhắn hoàn chỉnh.
  * **Giảm 60% Infra Code:** Nhờ sử dụng nền tảng AgentCore thay thế hạ tầng truyền thống.
- **Thông điệp dự án:** *"Khách hàng của KFC Việt Nam đã có mặt sẵn trên Zalo. KFC AI giúp họ không bao giờ phải đi đâu khác nữa."*

---

#### 2. Dự án S.H.E.P.H.E.RD – Giám sát & Điều phối An ninh/Lưu lượng Thông minh (Đội 3KA)

- **Hành trình 24h Hackathon:** Đội ngũ trải qua các giai đoạn cảm xúc từ *Hoài nghi* (quá tải ban đầu) → *Cuốn vào công việc* → *Tự hào*. Những kỷ niệm thực chiến 3h sáng: uống 5 lon Redbull, lỡ đẩy file `.env` lên GitHub, cãi nhau phân chia công việc nhưng vẫn cùng nhau hoàn thiện sản phẩm.
- **Bài toán & Giải pháp:** Giám sát thủ công lối vào/hàng đợi tại sự kiện rất dễ bỏ sót ùn tắc. S.H.E.P.H.E.R.D sử dụng phân tích Camera trực tiếp để đo mật độ người, ước tính thời gian xếp hàng và cảnh báo sớm nguy cơ ùn tắc.
- **2 tính năng AI Agentic cốt lõi:**
  * *Autonomous Monitor:* Giám sát tự động 24/7.
  * *Operator Copilot:* Trợ lý hỏi đáp bằng ngôn ngữ tự nhiên giúp nhân viên nhận gợi ý xử lý sự cố.
- **Công nghệ & Hạ tầng AWS:** YOLO + ByteTrack, Amazon SageMaker, Amazon Bedrock AgentCore + Strands Agent, React Dashboard. Hạ tầng AWS bao gồm Kinesis Video Streams, ECS Fargate, Lambda, API Gateway và DynamoDB.

---

#### 3. SA Professional AI Native App – Trợ lý tự động hóa cho Kiến trúc sư Giải pháp (Đội Plan V)

- **Vấn đề của Solution Architect (SA):** Khách hàng luôn muốn có thiết kế hệ thống, sơ đồ kiến trúc và bảng tính chi phí "ngay lập tức". Việc bóc tách yêu cầu và vẽ sơ đồ thủ công ngốn rất nhiều thời gian.
- **Giải pháp & Tính năng:** Ứng dụng AI Native phân tích tài liệu/yêu cầu ngôn ngữ tự nhiên → Tự động phác thảo phương án kiến trúc → Tự sinh sơ đồ Draw.io & sơ đồ AWS có thể chỉnh sửa → Ước tính chi phí AWS định hướng (tại region `ap-southeast-1`) → Tự động phát hiện lỗ hổng và giả định trong yêu cầu.
- **Kiến trúc hệ thống:** Giao diện Chat → App Server → Knowledge Base (giá AWS), Amazon Bedrock, Draw.io MCP, AWS Pricing MCP. Triển khai bằng Terraform trên AWS (CloudFront, Cognito, ALB, ECS Fargate, PostgreSQL, S3, EFS).
- **Tác động đột phá:** Giúp SA đi từ tài liệu thô đến bản nháp kiến trúc, mã IaC và bảng dự toán chi phí AWS chỉ trong vài phút thay vì phải làm từ số 0.

---

#### 4. Signal Scout – Nền tảng Phân tích & Cảnh báo Tín hiệu Tái cấu trúc Doanh nghiệp (Đội Dream AI Team)

- **Mô hình Value Creation:** Xâu chuỗi các tín hiệu rời rạc (tin tức, biến động tài chính, tái cấu trúc) thành một câu chuyện phân tích hoàn chỉnh có bằng chứng hỗ trợ, giúp doanh nghiệp ra quyết định chiến lược kịp thời.
- **Kiến trúc AgentCore & AWS:** Sử dụng Route53, Amplify, Cognito, API Gateway, Lambda, DynamoDB. Hệ thống gồm *Crawler Subagent* (Apify, TinyFish) và *Analysis Subagent* (Bedrock Guardrails, Strands Agent, Langfuse).
- **Trải nghiệm demo:** Nền tảng web cho phép nhập URL/tên công ty để tự động điều tra các thay đổi cấu trúc, tài chính và hiển thị biểu đồ thời gian xu hướng.

---

### Những gì học được

- **Agentic AI Architecture:** Một Agent hoàn chỉnh không chỉ dừng lại ở Chatbot mà phải có đủ 5 bước: Goal → Plan → Tools → Act → Verify.
- **Triết lý "Design Once | Deploy Everywhere":** Việc thiết kế kiến trúc chuẩn hóa qua các lớp Adapter/Connector giúp dễ dàng mở rộng sản phẩm lên bất kỳ kênh giao tiếp nào mà không cần viết lại mã nguồn.
- **Tối ưu hóa chi phí Cloud với Bedrock & AgentCore:** Việc ứng dụng AgentCore giúp giảm 60% Infra code và tối ưu chi phí vận hành xuống chỉ vài cent/đơn hàng.
- **Bài học thực chiến Hackathon:** *"Có mặt đã là chiến thắng một nửa"*, *"Sản phẩm nhỏ chạy được còn hơn ý tưởng lớn mà hỏng"*, và *"Những đồng đội bạn gặp quan trọng hơn cả giải thưởng"*.

---

### Ứng dụng vào công việc

- **Áp dụng mô hình Đa tác nhân (Multi-Agent):** Phân chia nhiệm vụ cho các Agent nhỏ chuyên biệt (Crawler, Analysis, Guardrails) kết hợp với Agent chính để tránh loãng ngữ cảnh và tăng độ chính xác.
- **Ứng dụng MCP (Model Context Protocol):** Tích hợp MCP (như AWS Pricing MCP hay Draw.io MCP) để cho phép AI Agent trực tiếp tương tác và sinh ra tài liệu/sơ đồ kỹ thuật tự động.
- **Tối ưu hóa quy trình thiết kế Cloud:** Áp dụng tư duy AI Native vào việc phác thảo kiến trúc hệ thống và dự toán ngân sách AWS nhanh chóng cho các dự án thực tế.

### Hình ảnh minh chứng

![Event 4](/images/4-EventParticipated/4.4-Event4/Event4.png?v=2)
