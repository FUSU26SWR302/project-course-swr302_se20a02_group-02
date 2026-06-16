# Changelog

## 1. Quy định ghi Changelog

File này dùng để ghi lại các thay đổi quan trọng trong quá trình thực hiện bài tập, lab, assignment hoặc project.

---

## 2. Thông tin project

| Thông tin | Nội dung |
|---|---|
| Môn học | Software Project (SWP391) |
| Mã môn học | SWP391 |
| Lớp | SE20A02 |
| Học kỳ | SU26 |
| Tên bài tập / Project | LuxeWay - Trusted E-commerce Platform for Vehicle Rental |
| Tên sinh viên / Nhóm | Nhóm 2 (Lê Văn Hậu, Nguyễn Văn Dạng, Hồ Thành Trung, Trần Phú Thịnh, Nguyễn Bùi Quang Vinh) |
| MSSV / Danh sách MSSV | DE190968, DE190968, DE190928, DE190371, DE190264 |
| Giảng viên hướng dẫn | (Giảng viên môn SWP391) |
| Repository URL | https://github.com/fptu-se-su26/swp391-su26-ai-audit-project-swp391_se20a02_group-02 |
| Ngày bắt đầu | 2026-05-30 |
| Ngày hoàn thành | 2026-06-16 |

---

## 3. Tổng quan các phiên bản/giai đoạn

| Phiên bản/Giai đoạn | Thời gian | Nội dung chính | Trạng thái |
|---|---|---|---|
| Phase 01 | 2026-05-30 | Khởi tạo module Chatbot | Completed |
| Phase 02 | 2026-06-03 | Tích hợp RAG và Gemini | Completed |
| Phase 03 | 2026-06-07 | Xây dựng chức năng Dark/Light Mode | Completed |
| Phase 04 | 2026-06-12 | Testing và Tối ưu trải nghiệm | Completed |

---

# [Phase 01] Khởi tạo module Chatbot

## Ngày thực hiện

```text
2026-05-30
```

## Đã hoàn thành

- [x] Tạo service AI module bên trong Spring Boot
- [x] Cấu hình API Key của Google Gemini
- [x] Setup các thư viện Spring AI và pgvector
- [x] Tạo script khởi tạo bảng vector database

## Thay đổi chi tiết

| STT | Nội dung thay đổi | Người thực hiện | File/Module liên quan | Minh chứng |
|---:|---|---|---|---|
| 1 | Thêm dependency Spring AI | Trần Phú Thịnh | `pom.xml` | `commit abc1234` |
| 2 | Config Gemini API Key | Trần Phú Thịnh | `application.yml` | `commit def5678` |

## AI có hỗ trợ không?

- [x] Có
- [ ] Không

Nếu có, mô tả AI đã hỗ trợ phần nào:

```text
AI giúp tìm kiếm các dependency cần thiết để cấu hình Spring AI tương thích với Spring Boot 3.
```

---

# [Phase 02] Tích hợp RAG và Gemini

## Ngày thực hiện

```text
2026-06-03
```

## Đã hoàn thành

- [x] Xây dựng script crawl dữ liệu policy để làm knowledge base
- [x] Viết logic chia nhỏ văn bản (TokenTextSplitter)
- [x] Viết logic lưu embedding vào database
- [x] Viết `ChatbotService` để gọi retrieval và sinh câu trả lời
- [x] Triển khai API SSE stream dữ liệu

## Thay đổi chi tiết

| STT | Nội dung thay đổi | Người thực hiện | File/Module liên quan | Minh chứng |
|---:|---|---|---|---|
| 1 | Logic tạo Embeddings | Trần Phú Thịnh | `EmbeddingService.java` | `commit 123abcd` |
| 2 | RAG Retrieval Logic | Trần Phú Thịnh | `ChatbotService.java` | `commit 456efgh` |

## AI có hỗ trợ không?

- [x] Có
- [ ] Không

Nếu có, mô tả AI đã hỗ trợ phần nào:

```text
AI sinh code cho luồng Retrieval-Augmented Generation và code stream Server-Sent Events.
```

---

# [Phase 03] Xây dựng chức năng Dark/Light Mode

## Ngày thực hiện

```text
2026-06-07
```

## Đã hoàn thành

- [x] Custom hook xử lý logic đổi màu sáng/tối
- [x] Cấu hình Tailwind CSS để hỗ trợ class `dark`
- [x] Tạo UI component `ThemeToggle`
- [x] Tích hợp vào Header chung của hệ thống

## Thay đổi chi tiết

| STT | Nội dung thay đổi | Người thực hiện | File/Module liên quan | Minh chứng |
|---:|---|---|---|---|
| 1 | Component Toggle Theme | Trần Phú Thịnh | `ThemeToggle.tsx` | `commit 789ijkl` |
| 2 | Cấu hình Tailwind | Trần Phú Thịnh | `tailwind.config.js` | `commit 999mno` |

## AI có hỗ trợ không?

- [x] Có
- [ ] Không

Nếu có, mô tả AI đã hỗ trợ phần nào:

```text
AI sinh code script chèn vào head để ngăn chớp màn hình, và hỗ trợ logic quản lý state với Zustand.
```

---

# [Phase 04] Testing và Tối ưu trải nghiệm

## Ngày thực hiện

```text
2026-06-12
```

## Đã hoàn thành

- [x] Viết unit test cho logic RAG
- [x] Viết System Prompt chặn chatbot nói chuyện phiếm
- [x] Chỉnh chu màu sắc Dark mode ở các trang con
- [x] Debug lỗi đứt kết nối stream

## Thay đổi chi tiết

| STT | Nội dung thay đổi | Người thực hiện | File/Module liên quan | Minh chứng |
|---:|---|---|---|---|
| 1 | Update Prompt template | Trần Phú Thịnh | `ChatbotService.java` | `commit pqr123` |
| 2 | Fix CSS dark mode card | Trần Phú Thịnh | `VehicleCard.tsx` | `commit stu456` |

## AI có hỗ trợ không?

- [x] Có
- [ ] Không

Nếu có, mô tả AI đã hỗ trợ phần nào:

```text
AI cung cấp các câu lệnh để test prompt injection và cách để bảo vệ chatbot bằng kỹ thuật prompt engineering.
```

---

# 4. Tổng kết thay đổi cuối project

## 4.1. Các chức năng đã hoàn thành

| STT | Chức năng | Trạng thái | Minh chứng | Ghi chú |
|---:|---|---|---|---|
| 1 | AI Chatbot Tư vấn xe | Completed | Demo, Code | Hoạt động trơn tru |
| 2 | Dark / Light Theme Toggle | Completed | Demo, Code | Lưu cache browser |

---

## 4.2. Bài học rút ra

```text
Nắm được tư duy ứng dụng AI (GenAI) vào dự án phần mềm một cách chuyên nghiệp. Hiểu về các framework Frontend và cách styling.
```

---

# 5. Cam kết cập nhật Changelog

Sinh viên/nhóm cam kết rằng nội dung changelog phản ánh đúng các thay đổi đã thực hiện trong quá trình làm bài tập/project.

| Đại diện sinh viên/nhóm | Ngày xác nhận |
|---|---|
| Trần Phú Thịnh - DE190371 | 2026-06-16 |
