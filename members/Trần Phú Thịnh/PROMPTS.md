# Prompt Log

## 1. Thông tin chung

| Thông tin | Nội dung |
|---|---|
| Môn học | Software Project (SWP391) |
| Mã môn học | SWP391 |
| Lớp | SE20A02 |
| Học kỳ | SU26 |
| Tên bài tập / Project | LuxeWay - Trusted E-commerce Platform for Vehicle Rental |
| Tên sinh viên / Nhóm | Trần Phú Thịnh - Nhóm 2 |
| MSSV / Danh sách MSSV | DE190371 |
| Giảng viên hướng dẫn | (Giảng viên môn SWP391) |
| Ngày bắt đầu | 2026-05-30 |
| Ngày cập nhật gần nhất | 2026-06-16 |

---

## 3. Công cụ AI đã sử dụng

- [x] ChatGPT
- [x] Gemini
- [ ] Claude
- [ ] GitHub Copilot
- [ ] Cursor
- [x] Antigravity
- [ ] Microsoft Copilot
- [ ] Perplexity

---

## 4. Bảng tổng hợp prompt đã sử dụng

| STT | Ngày | Công cụ AI | Mục đích | Prompt tóm tắt | Kết quả chính | Có sử dụng vào bài không? |
|---:|---|---|---|---|---|---|
| 1 | 2026-06-02 | Gemini | Hiểu RAG | Hỏi về kiến trúc RAG cho chatbot | Hiểu các khái niệm Ingestion, Retrieval | Có |
| 2 | 2026-06-05 | Antigravity | Dark mode | Hỏi code custom hook dark mode | Code cấu hình Tailwind và React | Có |
| 3 | 2026-06-10 | Antigravity | Gen code Chatbot | Xin code Spring AI SSE stream | Controller và Service cho Chatbot | Có |

---

## 5. Prompt chi tiết

---

### Prompt số 1

| Nội dung | Thông tin |
|---|---|
| Ngày sử dụng | 2026-06-05 |
| Công cụ AI | Antigravity |
| Mục đích | Tạo chức năng Dark/Light Mode bằng React + Tailwind |
| Phần việc liên quan | Frontend / Design |
| Mức độ sử dụng | Hỏi sinh code |

#### 5.1. Prompt nguyên văn

```text
Hãy giúp tôi viết một custom hook React tên là useTheme, và cấu hình TailwindCSS để làm chức năng chuyển đổi Dark/Light mode. Cần lưu trạng thái user chọn vào localStorage và tránh bị chớp màn hình trắng khi reload trang (FOUC).
```

#### 5.2. Bối cảnh khi viết prompt

```text
Dự án LuxeWay yêu cầu một giao diện hiện đại có hỗ trợ dark mode cho trải nghiệm mua sắm buổi đêm.
```

#### 5.3. Kết quả AI trả về

```text
Gợi ý file cấu hình tailwind.config.js với darkMode: 'class', một script inline đặt trong index.html để parse localStorage ngay lập tức, và một file useTheme.ts quản lý state.
```

#### 5.4. Kết quả đã áp dụng vào bài

```text
Đã áp dụng toàn bộ cấu trúc logic, từ script ở html đến hook.
```

#### 5.5. Phần sinh viên/nhóm đã chỉnh sửa hoặc cải tiến

```text
Tích hợp logic `useTheme` thẳng vào global state `uiStore.ts` bằng Zustand để các component khác có thể truy xuất dễ dàng hơn.
```

#### 5.6. Đánh giá chất lượng prompt

- [x] Prompt rõ ràng
- [x] Prompt có đủ bối cảnh
- [x] Prompt tạo ra kết quả tốt

---

### Prompt số 2

| Nội dung | Thông tin |
|---|---|
| Ngày sử dụng | 2026-06-10 |
| Công cụ AI | Antigravity |
| Mục đích | Code streaming response cho Chatbot AI |
| Phần việc liên quan | Backend / AI |
| Mức độ sử dụng | Hỏi sinh code |

#### 5.1. Prompt nguyên văn

```text
Tôi đang dùng Spring Boot 3. Hãy code cho tôi một ChatController có endpoint `/api/chat/stream`. Nó nhận đầu vào là câu hỏi của user, sau đó dùng ChatClient của Spring AI tích hợp Gemini để stream kết quả trả về liên tục bằng SSE (Server-Sent Events).
```

#### 5.2. Bối cảnh khi viết prompt

```text
Cần làm Chatbot cho trải nghiệm tốt như ChatGPT (hiển thị từng chữ) thay vì đợi hàng chục giây mới có kết quả hoàn chỉnh.
```

#### 5.3. Kết quả AI trả về

```text
Trả về class ChatController trả ra `Flux<String>`, sử dụng `chatClient.prompt().stream().content()`. Đi kèm cấu hình Maven.
```

#### 5.4. Kết quả đã áp dụng vào bài

```text
Sử dụng chính xác class Controller do AI cung cấp.
```

#### 5.5. Phần sinh viên/nhóm đã chỉnh sửa hoặc cải tiến

```text
Sửa lại cấu hình CORS, thêm annotation `@CrossOrigin` để frontend có thể nhận event.
```

#### 5.6. Đánh giá chất lượng prompt

- [x] Prompt rõ ràng
- [x] Prompt tạo ra kết quả tốt
- [x] Kết quả AI có lỗi nhỏ (thiếu CORS)

---

## 6. Prompt quan trọng nhất

### 6.1. Prompt được chọn

```text
Tôi đang xây dựng một ứng dụng thuê xe bằng Spring Boot và React. Tôi muốn làm một Chatbot thông minh có thể đọc hiểu chính sách thuê xe và thông tin xe của nền tảng để trả lời khách hàng. Hãy gợi ý cho tôi kiến trúc sử dụng RAG với Langchain và mô hình Gemini.
```

### 6.2. Vì sao prompt này quan trọng?

```text
Vì nó là nền tảng định hình toàn bộ giải pháp kỹ thuật cho module AI Chatbot, một tính năng cốt lõi của dự án.
```

### 6.3. Kết quả prompt này mang lại

```text
Giúp tôi hiểu khái niệm Vector Database, Data Chunking và cách RAG hoạt động.
```

### 6.4. Sinh viên/nhóm đã kiểm tra kết quả như thế nào?

```text
Xác minh lại các tài liệu từ Spring AI documentation xem có đúng như AI mô tả không.
```

### 6.5. Sinh viên/nhóm đã cải tiến gì từ kết quả AI?

```text
Chuyển đổi hoàn toàn sang kiến trúc Spring Boot thay vì dùng Python như AI gợi ý lúc đầu, sử dụng pgvector.
```

---

## 11. Cam kết sử dụng prompt minh bạch

Sinh viên/nhóm cam kết rằng:

- Các prompt quan trọng đã được ghi lại trung thực.
- Chịu trách nhiệm với sản phẩm cuối cùng.

| Đại diện sinh viên/nhóm | Ngày xác nhận |
|---|---|
| Trần Phú Thịnh - DE190371 | 2026-06-16 |
