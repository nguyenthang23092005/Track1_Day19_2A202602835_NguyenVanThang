# AI Support Log — Option C

**MHV:** 2A202602835 · **Họ tên:** Nguyễn Văn Thăng · **Nhóm:** FinTech  
**Case:** A — AI Tutor: Diagnostic Refresher

Đây là bản ghi hỗ trợ AI và giới hạn sử dụng, không phải phần đóng góp cá nhân hoặc reflection do AI viết thay người nộp.

## 1. Hỗ trợ thuộc phạm vi được phép

| Nội dung AI đã hỗ trợ | Artifact / giới hạn |
|---|---|
| Triển khai cơ chế tương tác C từ design sheet: hai gợi ý, chọn/sửa/phủ quyết, preview và quay lại quiz | [Prototype HTML](prototype/index.html); người học quyết định phần ôn |
| Sinh fixture bài RAG, đáp án sai mẫu, lịch sử học mẫu và canned outputs cho phần ôn | Chỉ dùng làm nội dung trong prototype; không phải observation hoặc lịch sử của tester thật |
| Viết code giao diện, xử lý quiz, đổi lựa chọn, bỏ qua và reset | Toàn bộ CSS/JavaScript được nhúng trong một HTML theo yêu cầu bàn giao |
| Soạn kịch bản đối thoại mẫu: opening, task và câu compare | Dùng để chuẩn bị facilitation; không ghi thành lời tester đã nói |
| Chuẩn bị annotation ngoài giao diện | [Annotation](prototype/annotations.md); không hiện cho tester |
| Kiểm tra chức năng của prototype C trên Edge offline | [QA report](prototype/qa-report.md): 13 nhóm kiểm tra đạt; đây là QA kỹ thuật, không phải test người dùng |
| Đối chiếu nội dung ôn với tài liệu kỹ thuật | Nguồn tham khảo trong annotation; không dùng tài liệu này để bổ sung evidence về hành vi người học |

## 2. Điểm chưa phù hợp và giới hạn của output

- Bản đầu tách nhiều file JS/CSS. Người nộp yêu cầu chỉ một HTML; AI đã gộp và kiểm tra lại. Không ghi thay đổi do AI thực hiện thành việc người nộp tự sửa code bằng tay.
- Mức chắc 70%/40% là canned theo design sheet, không có phép đo độ chính xác mô hình. Các gợi ý không chứng minh người học thiếu khái niệm đó.
- QA chỉ xác nhận các luồng kỹ thuật đã kiểm tra. Nó không chứng minh tester ngoài nhóm hiểu giao diện, ôn đúng nền hoặc làm bài tốt hơn.


## 3. Cách xử lý evidence và hồ sơ trước khi nộp

- Loại quote/observation/feedback tự sinh khỏi phần kết quả test; chỉ điền bằng ghi chép từ phiên tester thật.
- Giữ lời nói và hành vi thực tế, kể cả mâu thuẫn hoặc chưa rõ. Tách chúng khỏi diễn giải của nhóm; không làm sạch evidence đến mức đổi nghĩa hoặc mất bối cảnh.
- Chỉ tổng hợp pattern và chốt Next Change sau khi có feedback thực tế. Nêu rõ Still Unproven, không suy ra validation từ canned output hoặc QA.
- Người nộp tự viết đóng góp cá nhân và reflection sau buổi học. AI không điền thay những phần này.


