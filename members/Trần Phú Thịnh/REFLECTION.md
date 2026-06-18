# AI Learning Reflection

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
| Ngày hoàn thành reflection | 2026-06-16 |

---

## 3. Tóm tắt quá trình sử dụng AI

```text
Trong dự án này, em (Trần Phú Thịnh) sử dụng AI chủ yếu để xây dựng tính năng AI Chatbot (hỗ trợ tư vấn thuê xe tự động) và cải thiện trải nghiệm giao diện người dùng với tính năng Dark/Light mode. AI đã đóng vai trò là một "mentor kỹ thuật", giúp em hiểu các khái niệm kiến trúc RAG, làm quen với Langchain/Spring AI và setup cấu trúc frontend mượt mà. Công cụ Antigravity và Gemini là trợ thủ đắc lực nhất trong suốt quá trình triển khai code thực tế.
```

---

## 4. Công cụ AI đã sử dụng

Đánh dấu các công cụ AI đã sử dụng.

- [x] ChatGPT
- [x] Gemini
- [ ] Claude
- [ ] GitHub Copilot
- [ ] Cursor
- [x] Antigravity
- [ ] Microsoft Copilot
- [ ] Perplexity

### Công cụ được sử dụng nhiều nhất

```text
Antigravity và Gemini.
```

### Lý do sử dụng công cụ đó

```text
Antigravity sinh code chính xác với ngữ cảnh dự án, trong khi Gemini có khả năng giải thích các lý thuyết về AI (LLM, Embeddings) rất trực quan và dễ hiểu.
```

---

## 5. AI đã hỗ trợ em/nhóm ở điểm nào?

- [x] Phân tích bài toán
- [x] Tìm ý tưởng giải pháp
- [x] Thiết kế giao diện
- [x] Thiết kế kiến trúc hệ thống
- [x] Viết code mẫu
- [x] Debug lỗi

### Mô tả chi tiết

```text
AI giúp thiết kế hệ thống RAG chatbot (VectorDB, Embeddings) và cấu hình TailwindCSS darkMode. Nó cũng hỗ trợ fix lỗi mất kết nối khi sử dụng SSE Streaming API.
```

---

## 6. AI có giúp em/nhóm học tốt hơn không?

### 6.1. Những điểm AI giúp em/nhóm học tốt hơn

```text
- Hiểu được công nghệ mới (RAG, Vector Search).
- Học được cách code SSE (Server Sent Events) trên Spring Boot và bắt event ở React.
- Cải thiện tư duy sử dụng TailwindCSS chuẩn chỉ.
```

### 6.2. Những điểm AI chưa giúp tốt hoặc gây khó khăn

```text
- AI hay cung cấp các phiên bản thư viện cũ (ví dụ Langchain4j bản cũ) khiến code copy vào bị báo lỗi ClassNotFound.
- Đôi khi AI (LLM) trả lời ảo giác (hallucination) khi test chatbot, đòi hỏi em phải học thêm kỹ năng Prompt Engineering để kiềm chế chatbot lại.
```

### 6.3. Em/nhóm có bị phụ thuộc vào AI không?

- [ ] Không phụ thuộc
- [x] Phụ thuộc ít
- [ ] Phụ thuộc trung bình
- [ ] Phụ thuộc nhiều

Giải thích:

```text
Chỉ dùng AI để định hình khung code ban đầu và giải quyết vấn đề chưa biết, sau đó tự điều chỉnh theo hệ thống dự án.
```

---

## 7. Em/nhóm đã kiểm tra kết quả AI như thế nào?

- [x] Chạy thử chương trình
- [x] Kiểm tra output
- [x] Đối chiếu với tài liệu môn học
- [x] Tra cứu tài liệu chính thống

### Ví dụ cụ thể về một lần kiểm chứng

| Nội dung | Mô tả |
|---|---|
| AI đã gợi ý gì? | Gọi API Gemini trả kết quả dạng stream. |
| Em/nhóm đã kiểm tra bằng cách nào? | Dùng Postman và Browser Devtools (Network -> EventStream) để kiểm tra luồng dữ liệu. |
| Kết quả kiểm tra | Bị block bởi chính sách CORS. |
| Em/nhóm đã xử lý tiếp như thế nào? | Bổ sung @CrossOrigin vào Controller và cấu hình proxy trên vite.config.ts. |

---

## 9. Phần đóng góp thật sự của sinh viên/nhóm

```text
Phần đóng góp cốt lõi của bản thân là:
- Cấu hình dữ liệu thực tế (dữ liệu các dòng xe cao cấp của dự án) vào cơ sở dữ liệu Vector (pgvector).
- Viết System Prompt chặt chẽ để bảo vệ chatbot khỏi các cuộc tấn công prompt injection hoặc bịa đặt thông tin.
- Custom màu sắc Dark mode bám sát hệ thống màu của LuxeWay (chứ không dùng màu xám đen chung chung của AI).
```

---

## 11. Bài học về môn học

```text
- Kiến thức về ứng dụng thực tế của Generative AI vào phần mềm, biến ứng dụng web truyền thống thành ứng dụng thông minh.
- Kỹ năng xử lý real-time streaming data.
- Kỹ năng styling frontend linh hoạt (Theming).
```

---

## 12. Bài học về sử dụng AI có trách nhiệm

```text
- Không dùng AI sinh code mà không đọc hiểu dòng code đó chạy thế nào, rủi ro về security là rất lớn.
- Biết cách quản lý rủi ro "ảo giác" của chatbot để bảo vệ thương hiệu của sản phẩm (hệ thống tư vấn phải chính xác).
```

---

## 17. Cam kết Reflection

Em/nhóm cam kết rằng nội dung reflection này phản ánh trung thực quá trình sử dụng AI và quá trình học tập trong bài tập/project.

| Đại diện sinh viên/nhóm | Ngày xác nhận |
|---|---|
| Trần Phú Thịnh - DE190371 | 2026-06-16 |
