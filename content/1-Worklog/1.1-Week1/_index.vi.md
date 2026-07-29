---
title: "Worklog Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
reportTableColumns:
  - Thứ
  - Công việc
  - Ngày hoàn thành
reportType: worklog
---

### Mục tiêu tuần 1:

* Làm quen với văn hóa làm việc và các thành viên trong chương trình First Cloud AI Journey (FCAJ).
* Khám phá giao diện AWS Management Console và thực hành 5 bài lab cơ bản trên widget **Explore AWS** (Explore AWS Tasks).
* Nắm vững cách thiết lập ngân sách cảnh báo, khởi chạy máy chủ, xây dựng ứng dụng Serverless, tạo CSDL và thử nghiệm AI với Amazon Bedrock.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Làm quen với các thành viên FCAJ và tìm hiểu quy định làm việc.<br>- **Thực hành Lab 1 (AWS Budgets):** Vào AWS Budgets → Tạo `Monthly cost budget` đơn giản ($10/tháng) và đăng ký email nhận thông báo cảnh báo chi phí. | 15/06/2026 | 15/06/2026 | <https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html> |
| 3 | - Tìm hiểu dịch vụ Điện toán Đám mây Amazon EC2.<br>- **Thực hành Lab 2 (Amazon EC2):** Khởi chạy một EC2 instance nhỏ (t2.micro / Free Tier) từ widget Explore AWS, kiểm tra trạng thái kết nối và thực hiện xóa (`Terminate`) sau khi kết thúc. | 16/06/2026 | 16/06/2026 | <https://docs.aws.amazon.com/ec2/> |
| 4 | - Tìm hiểu mô hình kiến trúc Serverless trên AWS.<br>- **Thực hành Lab 3 (AWS Lambda):** Chọn bài thực hành xây dựng Serverless Web App qua Blueprint `Getting started with Lambda HTTP`, cấu hình HTTP API trigger và chạy thử ứng dụng. | 17/06/2026 | 17/06/2026 | <https://docs.aws.amazon.com/lambda/> |
| 5 | - Tìm hiểu dịch vụ Cơ sở dữ liệu quan hệ Amazon RDS.<br>- **Thực hành Lab 4 (Amazon RDS):** Khởi tạo một CSDL Amazon RDS nhỏ (gói Free Tier/Dev/Test), kiểm tra kết nối và xóa (`Delete database`) sau khi hoàn tất bài thực hành. | 18/06/2026 | 18/06/2026 | <https://docs.aws.amazon.com/rds/> |
| 6 | - Tìm hiểu tổng quan về Trí tuệ nhân tạo tạo sinh (Generative AI) trên AWS.<br>- **Thực hành Lab 5 (Amazon Bedrock):** Truy cập giao diện Bedrock Playground, lựa chọn các mô hình AI nền tảng (Foundation Models) và thực hiện thử nghiệm prompt cơ bản. | 19/06/2026 | 19/06/2026 | <https://docs.aws.amazon.com/bedrock/> |


### Kết quả đạt được tuần 1:

* **Hoàn thành 5 bài lab Explore AWS cơ bản ($20/bài):**
  1. **AWS Budgets:** Tạo thành công ngân sách cảnh báo chi phí $10/tháng, cấu hình email thông báo tự động khi ngân sách vượt ngưỡng để quản lý chi phí an toàn.
  2. **Amazon EC2:** Làm chủ quy trình khởi chạy một máy chủ ảo EC2, kiểm tra trạng thái hoạt động và biết cách dọn dẹp tài nguyên (Terminate) đúng quy trình.
  3. **AWS Lambda:** Hiểu tư duy Serverless, tạo thành công Web App đơn giản bằng AWS Lambda Blueprint tích hợp API Gateway HTTP API.
  4. **Amazon RDS:** Nắm rõ các bước khởi tạo Instance CSDL quan hệ RDS trên Cloud, cấu hình tham số cơ bản và chủ động xóa tài nguyên để tránh phát sinh chi phí.
  5. **Amazon Bedrock:** Trải nghiệm trực tiếp giao diện Bedrock Playground, thử nghiệm đưa câu lệnh (prompting) tương tác với các mô hình AI tiên tiến.

* **Hiểu và sử dụng thành thạo AWS Management Console Home:** Biết cách tận dụng widget *Explore AWS* để thực hành nhanh các dịch vụ AWS cốt lõi một cách trực quan và hiệu quả.
