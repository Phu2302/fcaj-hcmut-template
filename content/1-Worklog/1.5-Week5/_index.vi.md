---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
reportTableColumns:
  - Thứ
  - Công việc
  - Ngày hoàn thành
reportType: worklog
---

### Mục tiêu tuần 5:

* Tích hợp trình biên soạn mã trực tuyến Monaco Code Editor cho các bài tập trắc nghiệm / lập trình.
* Hoàn thiện giao diện Diễn đàn (Forum), Bảng điểm, Đăng ký học phần và kết nối API với Backend.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tích hợp trình soạn thảo code **Monaco Code Editor** (`@monaco-editor/react`) cho giao diện làm bài tập lập trình (`QuizPage`).<br>- Hỗ trợ syntax highlighting và tùy chọn ngôn ngữ (C++, Python, JavaScript). | 13/07/2026 | 13/07/2026 | |
| 3 | - Phát triển giao diện Diễn đàn học tập (`Forum`).<br>- Xây dựng trang Đăng câu hỏi & Thảo luận (`ForumPostPage`) giữa sinh viên và giảng viên. | 14/07/2026 | 14/07/2026 | |
| 4 | - Thiết kế giao diện Trang Đăng ký học phần (`CourseRegistration`).<br>- Phát triển giao diện Bảng điểm (`Scoreboard`) và Hồ sơ cá nhân (`ProfilePage`). | 15/07/2026 | 15/07/2026 | |
| 5 | - Cấu hình `Axios Interceptor` kết nối Frontend với Backend API.<br>- Tự động đính kèm Bearer Token vào header và xử lý điều hướng tự động khi hết hạn phiên làm việc (401 Unauthorized). | 16/07/2026 | 16/07/2026 | |
| 6 | - Kiểm thử toàn bộ luồng người dùng (User Flow), sửa lỗi UI/UX và tối ưu hiệu năng trang web.<br>- Họp nhóm đánh giá hoàn thiện Frontend, chuẩn bị cho tuần triển khai lên Cloud AWS. | 17/07/2026 | 17/07/2026 | |


### Kết quả đạt được sau tuần 5:

* Tích hợp thành công Monaco Code Editor cho trải nghiệm thực hành lập trình trực tiếp trên trình duyệt.
* Hoàn thiện toàn bộ các trang giao diện Frontend chính: Quiz, Forum, Đăng ký học phần, Bảng điểm và Hồ sơ cá nhân.
* Tích hợp thành công API giữa Frontend và Backend, sẵn sàng cho đóng gói ứng dụng.
