# AI Audit Log

## 1. Thông tin chung

| Thông tin | Nội dung |
|---|---|
| Môn học | SWR302 |
| Mã môn học | SWR302 |
| Lớp | SE20A02 |
| Học kỳ | SU26 |
| Tên bài tập / Project | LuxeWay - Trusted E-commerce Platform for Vehicle Rental |
| Tên sinh viên | Nguyễn Bùi Quang Vinh |
| MSSV | DE190264 |
| Vai trò | Member |
| Ngày cập nhật | 2026-06-16 |

---

## 2. Công cụ AI đã sử dụng

- [x] ChatGPT / Codex
- [ ] Gemini
- [ ] Claude
- [ ] GitHub Copilot
- [ ] Cursor
- [ ] Antigravity
- [ ] Microsoft Copilot
- [ ] Perplexity

---

## 3. Mục tiêu sử dụng AI

```text
Em sử dụng AI để hỗ trợ rà soát cấu trúc dự án LuxeWay, đọc hiểu các phần frontend/backend
đã có, gợi ý cách sửa lỗi, cải thiện giao diện, kiểm tra luồng chạy project và hoàn thiện
tài liệu cá nhân trong thư mục members.

AI được dùng như công cụ hỗ trợ phân tích, review và đề xuất. Em vẫn kiểm tra lại code,
đọc nội dung thay đổi, chạy các lệnh build/test khi cần và chịu trách nhiệm với kết quả cuối.
```

---

## 4. Nhật ký sử dụng AI chi tiết

### Lần sử dụng AI số 1

| Nội dung | Thông tin |
|---|---|
| Ngày sử dụng | 2026-06-16 |
| Công cụ AI | ChatGPT / Codex |
| Mục đích sử dụng | Rà soát và cập nhật tài liệu cá nhân |
| Phần việc liên quan | Report / Documentation |
| Mức độ sử dụng | Hỗ trợ một phần |

#### Prompt đã sử dụng

```text
Ở phần member tôi có cập nhật 1 folder của tôi hãy sửa lại 4 file có trong đó dựa trên những gì chúng ta đã làm từ trước đến giờ. Tôi sẽ cung cấp cho bạn họ tên, mssv, tên lớp, tên môn:
- họ và tên: Nguyễn Bùi Quang Vinh.
- MSSV: DE190264
- Môn: SWR302
- Lớp: SE20A02
```

#### Kết quả AI gợi ý

```text
AI đọc thư mục members/Nguyễn Bùi Quang Vinh, kiểm tra 4 file AI_AUDIT_LOG.md,
CHANGELOG.md, PROMPTS.md, REFLECTION.md và thay nội dung template bằng nội dung
đã điền thông tin sinh viên, môn học, lớp, project LuxeWay và quá trình sử dụng AI.
```

#### Phần sinh viên đã sử dụng từ AI

```text
Em sử dụng cấu trúc trình bày, bảng thông tin, phần mô tả quá trình dùng AI,
phần kiểm chứng kết quả AI và phần cam kết học thuật.
```

#### Phần sinh viên tự chỉnh sửa hoặc cải tiến

```text
Em cung cấp thông tin cá nhân chính xác gồm họ tên, MSSV, lớp và môn học.
Em kiểm tra lại nội dung để đảm bảo phản ánh đúng quá trình làm việc với project LuxeWay.
```

#### Minh chứng

| Loại minh chứng | Nội dung |
|---|---|
| File liên quan | members/Nguyễn Bùi Quang Vinh/AI_AUDIT_LOG.md |
| File liên quan | members/Nguyễn Bùi Quang Vinh/CHANGELOG.md |
| File liên quan | members/Nguyễn Bùi Quang Vinh/PROMPTS.md |
| File liên quan | members/Nguyễn Bùi Quang Vinh/REFLECTION.md |
| Kết quả chạy/test | Đã rà soát bằng lệnh đọc file và tìm kiếm trong repository |

---

## 5. Bảng tổng hợp mức độ sử dụng AI

| Hạng mục | Không dùng AI | AI hỗ trợ ít | AI hỗ trợ nhiều | AI sinh chính | Ghi chú |
|---|:---:|:---:|:---:|:---:|---|
| Phân tích yêu cầu |  | x |  |  | Dùng để làm rõ cách ghi tài liệu |
| Thiết kế giao diện |  | x |  |  | Gợi ý cải thiện nếu cần |
| Code frontend/backend |  | x |  |  | AI hỗ trợ review và sửa lỗi nhỏ |
| Debug lỗi |  |  | x |  | Hỗ trợ đọc lỗi, đề xuất hướng xử lý |
| Kiểm thử sản phẩm |  | x |  |  | Gợi ý lệnh build/test và checklist |
| Viết báo cáo |  |  | x |  | Hỗ trợ cấu trúc nội dung |

---

## 6. Các lỗi hoặc hạn chế từ AI

| STT | Lỗi/hạn chế từ AI | Cách phát hiện | Cách xử lý/cải tiến |
|---:|---|---|---|
| 1 | AI có thể suy đoán sai thông tin môn học/project nếu không có dữ liệu | So sánh với thông tin do sinh viên cung cấp | Ưu tiên dùng thông tin người dùng cung cấp: SWR302, SE20A02, DE190264 |
| 2 | AI có thể đề xuất nội dung quá chung chung | Đọc lại reflection và prompt log | Chỉnh nội dung theo đúng project LuxeWay |
| 3 | AI không thay thế việc kiểm tra file thật | Kiểm tra trực tiếp repository | Đọc file, tìm kiếm bằng `rg`, xác nhận đường dẫn trước khi sửa |

---

## 7. Kiểm chứng kết quả AI

```text
Em kiểm chứng bằng cách đọc lại các file Markdown sau khi cập nhật, đối chiếu với thông tin
cá nhân đã cung cấp và đảm bảo nội dung không mâu thuẫn với project LuxeWay. Khi AI đề xuất
code hoặc tài liệu, em không nộp nguyên văn nếu chưa đọc lại và hiểu nội dung.
```

---

## 8. Đóng góp cá nhân

```text
Nguyễn Bùi Quang Vinh - DE190264 chịu trách nhiệm cập nhật thư mục member cá nhân,
ghi nhận minh bạch quá trình sử dụng AI, rà soát nội dung tài liệu và đảm bảo các phần
đã nộp có thể giải thích lại được.
```

---

## 9. Reflection cuối bài

```text
AI hỗ trợ tốt ở việc gợi ý cấu trúc tài liệu, đọc hiểu project nhanh hơn và đưa ra checklist
kiểm tra. Tuy nhiên, phần quyết định cuối cùng vẫn do em thực hiện: xác nhận thông tin cá nhân,
kiểm tra nội dung, đánh giá tính phù hợp và chịu trách nhiệm với sản phẩm nộp.
```

---

## 10. Cam kết học thuật

Em cam kết rằng nội dung AI hỗ trợ đã được ghi nhận trung thực, không nộp kết quả AI khi chưa
kiểm tra, có khả năng giải thích các phần đã nộp và chịu trách nhiệm với sản phẩm cuối cùng.

| Đại diện sinh viên | Ngày xác nhận |
|---|---|
| Nguyễn Bùi Quang Vinh - DE190264 | 2026-06-16 |
