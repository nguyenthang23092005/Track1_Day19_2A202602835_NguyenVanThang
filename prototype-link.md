# Prototype Link — Nhóm FinTech (A/B/C chung)

> Cả 3 options bắt đầu từ cùng Trang chủ Màn 0 (`prototype/index.html`), cùng task, cùng dữ liệu mẫu (RAG Quiz & Slide 8-10). Tester tự mở và thao tác độc lập, không cần facilitator giải thích. Mỗi option đều có điểm phục hồi quyền kiểm soát (Control & Recovery) và nút Trang chủ.

## 1. Bản Micro-Prototype HTML Test-Ready trong Repo
Nhóm đã triển khai bộ Micro-Prototype tương tác hoàn chỉnh bằng HTML/CSS/JavaScript độc lập, không phụ thuộc server, mở trực tiếp bằng bất kỳ trình duyệt nào:

- **Màn 0 — Bối cảnh chung (Common Context) & Cửa vào A/B/C:**
  - File: [`prototype/index.html`]
  - Chức năng: Thể hiện tình huống bài học RAG, thông báo lỗi làm sai 2 lần quiz, tóm tắt slide 8–10 và cung cấp bảng điều hướng thử nghiệm 3 options.

- **Option A — AI chẩn đoán dẫn dắt (Nguyễn Anh Dũng phụ trách):**
  - File: [`prototype/option-a.html`]
  - Cơ chế: *AI Ask rồi Act* — 2 câu hỏi chẩn đoán nhanh → AI kết luận hổng Embedding (độ chắc 65%) → Thẻ giải thích 60 giây.

- **Option B — Sơ đồ kiến thức nền tảng tự chọn (Tạ Việt Cường phụ trách chính):**
  - File: [`prototype/option-b.html`]
  - Cơ chế: *AI Don't Act* — Sơ đồ 3 khái niệm nền do giảng viên tạo sẵn (Vector Embedding, Chunk Overlap, Top-k Retrieval) kèm nhãn gợi ý trung tính. Người học tự chọn và mở Thẻ ôn cấp tốc 60 giây (gồm Khái niệm, Ví dụ thực tế, Câu hỏi tự kiểm tra). Có nút đổi thẻ và đóng map 1 chạm.

- **Option C — Đồng chẩn đoán minh bạch có evidence (Nguyễn Văn Thăng phụ trách):**
  - File: [`prototype/option-c.html`]
  - Cơ chế: *AI Ask, User Chốt (Co-Create)* — AI đề xuất 2 giả thuyết có thanh đo độ chắc chắn (70% và 40%) kèm trích xuất căn cứ từ lịch sử học tập. Người dùng chọn 1 phương án hoặc nhấn quyền phủ quyết ("Cả hai đều không đúng") để chuyển sang Option B.

---

## 2. Đường link Online (nếu chạy qua GitHub Pages / Live Server)
- **Local file:** Mở trực tiếp file `prototype/index.html` trên trình duyệt Chrome / Edge / Firefox.
- **Quy trình chạy test:** Mở `index.html` → Bấm thử Option A (4 phút) → Trang chủ → Bấm thử Option B (4 phút) → Trang chủ → Bấm thử Option C (4 phút) → Phỏng vấn so sánh và trade-off (4 phút).

---

## 3. Tiêu chí nghiệm thu GATE 4 (Definition of Testable)
- [x] Tester tự mở và thao tác độc lập trên cả 3 option mà không cần hướng dẫn thao tác.
- [x] Cả 3 phương án chia sẻ ~70% bối cảnh chung (Bài 4 RAG, 2 câu quiz sai, tóm tắt slide 8-10, phong cách thiết kế).
- [x] Dữ liệu đủ thực tế để tester đọc và ra quyết định chuyên môn.
- [x] Thể hiện rõ ràng các nút lấy lại quyền kiểm soát (Bỏ qua câu hỏi, Đổi thẻ khác, Phủ quyết AI, Quay lại bài ngay, nút Trang chủ).
