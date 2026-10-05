# Group Feedback Synthesis — Nhóm FinTech (sau đủ 3 notes)

> Mỗi thành viên test 1 tester ngoài nhóm với cả A/B/C (~20 phút/tester). Tổng hợp dựa trên hành vi và lời nói thực tế từ đủ 3 phiên độc lập (Cường, Thăng, Dũng), không tuyên bố validated, không tâng bốc giải pháp.

| Nội dung | Feedback 1 (Cường facilitate) | Feedback 2 (Thăng facilitate) | Feedback 3 (Dũng facilitate) | Pattern hoặc khác biệt |
|---|---|---|---|---|
| **First action** | Mở A bấm `[Xem gợi ý]`; mở B dừng lại trước chatbox; mở C liếc nút ngoại lệ. | Thử lần lượt A → B → C; đọc kỹ ví dụ lợp ngói ở A; mở khung chat ở B. | Thử lần lượt A → B → C; đọc kỹ chẩn đoán sai 2 lần ở A rồi chuyển sang thử các nút ở B. | **Pattern:** Cả 3 tester đều tập trung cao độ vào ví dụ trực quan (lợp ngói) và đều có phản xạ tìm kiếm sự tương tác hai chiều thay vì đọc văn bản tĩnh. |
| **Breakdown chính (Nguyên văn lời Tester)** | 1. *"Luồng hơi ép buộc người dùng vào một khuôn, chưa cho control được."*<br>2. *"Khi chưa hiểu bài thì vẫn chưa biết cần hỏi AI về vấn đề gì."*<br>3. *"Có giải thích tổng quát nhưng chưa cho phép hỏi lại khi chưa hiểu."* | - **Option A:** *"Chưa cho tự do gõ câu hỏi"* (Control: 5/5, Help: 5/5).<br>- **Option B:** *"Đôi khi chính tôi chưa hiểu rõ là tôi nên đặt câu hỏi gì, dẫn đến việc đặt câu hỏi không tối ưu"* (Control: 4/5, Help: 5/5).<br>- **Option C:** *"Trải nghiệm hơi bị động, lo ngại sẽ bị sót thông tin khi AI đã định hướng sẵn"* (Control: 2/5, Help: 4/5). | - **Option A:** *"Luồng gợi ý ban đầu khá định hướng; muốn hỏi một chi tiết riêng thì chưa tiện"* (Control: 4/5, Help: 5/5).<br>- **Option B:** *"Nhiều lựa chọn can thiệp khiến tôi phải tự quyết khá nhiều; lúc đang bí kiến thức có thể không biết nên chọn cách hỏi nào trước"* (Control: 5/5, Help: 5/5).<br>- **Option C:** *"AI tự kết luận 80% lỗi ở overlap khiến tôi lo nếu nguyên nhân là Top-k hoặc đọc nhầm đề thì phải vào báo ngoại lệ để sửa"* (Control: 3/5, Help: 4/5). | **Sự hội tụ bằng chứng tuyệt đối (Triangulation):**<br>1. **Ở A:** Cả 3 khen ví dụ lợp ngói nhưng đồng thuận là quá định hướng, thiếu tiện lợi khi muốn hỏi một chi tiết riêng.<br>2. **Ở B:** Cả 3 đều gặp hiện tượng *tê liệt nhận thức*: khi đang bí kiến thức thì không biết đặt câu hỏi gì / không biết chọn cách hỏi nào trước.<br>3. **Ở C:** Cả 3 đều lo ngại việc AI tự động áp đặt định hướng sẵn sẽ làm sót thông tin / chẩn đoán lệch (Control chỉ 2-3/5). |
| **Cách lấy lại control** | Dùng nút đổi góc độ ở B (Ví dụ đời thực); bấm nút `[Báo ngoại lệ]` ở C; bấm `Trang chủ`. | Chấm điểm Control ở C tụt xuống 2/5 để phản đối sự tự động áp đặt; tìm kiếm ô gõ câu hỏi tự do ở A. | Tích cực dùng các nút can thiệp ở B: yêu cầu đổi cách giải thích, so sánh overlap 0 và 50, chuyển sang Top-k và tự gõ sửa ô ghi chú cá nhân. | **Pattern:** Khi cảm thấy bị ép khuôn hoặc AI đoán mò, cả 3 tester đều chủ động kích hoạt các công cụ can thiệp hoặc đòi hỏi quyền được tự tay điều chỉnh. |
| **Option được chọn** | **Option B** (sau khi dùng nút đổi góc độ giải thích). | **Chưa chốt / Phân vân giữa A và B** (thích ví dụ ở A nhưng muốn tự do gõ ở B). | **Option B** (được đánh giá cao nhất về tính chủ động). | **Khác biệt & Xu hướng:** 2/3 tester chốt chọn B, 1 tester phân vân giữa A và B. Không có bất kỳ ai chọn Option C làm giải pháp học tập lâu dài. |
| **Trade-off nguyên văn** | *"Chọn B vì muốn tự làm chủ, chấp nhận tốn công gõ và lúc đầu hơi bối rối không biết hỏi gì."* | *"Option C rất nhanh nhưng đánh đổi bằng việc bị động và dễ sót ý; Option B tự do nhưng tốn công nghĩ câu hỏi tối ưu; Option A dễ hiểu nhất nhưng bị gò bó."* | *"B phù hợp nhất khi tôi muốn hiểu đúng lỗ hổng của bản thân và có thể thay đổi cách học ngay trong lúc trao đổi. Đánh đổi là cần thêm các câu hỏi gợi ý hoặc lộ trình ngắn để người học không bị bí khi chưa biết phải yêu cầu AI hỗ trợ thế nào."* | **Pattern cốt lõi:** Người học sẵn sàng đánh đổi sự rảnh tay (từ chối tự động hóa của C) để lấy quyền làm chủ (chọn B), nhưng tha thiết yêu cầu hệ thống cung cấp "giàn giáo gợi ý" (scaffolding) để không bị bơ vơ khi đang hổng kiến thức. |

---

## Một Next Change nhóm chốt
> **Chốt 1 hướng đi duy nhất:** Thiết kế cơ chế **"Hybrid Scaffolded Drill-down"** (Khung chẩn đoán định hướng + Hỏi đáp đào sâu theo ngữ cảnh):

- **Next Change cụ thể:**
  1. **Khắc phục lỗi "tê liệt khi bí kiến thức / không biết hỏi gì trước" của Option B (xác nhận bởi cả 3/3 Tester):** 
     - Không để khung chat trắng bắt người học tự nghĩ. Sử dụng cơ chế phát hiện chủ động từ Option A để đưa ra chẩn đoán ban đầu và gợi ý sẵn 2–3 "nghi vấn cốt lõi" cụ thể (ví dụ: *"Tại sao cắt cụt câu lại làm mất ngữ cảnh?"* hoặc *"Vì sao k=1 không đủ thông tin đối chiếu?"*), đóng vai trò như lộ trình ngắn để người học không bị bối rối.
  2. **Khắc phục lỗi "quá định hướng / chưa tiện hỏi chi tiết riêng" của Option A & C (xác nhận bởi cả 3/3 Tester):** 
     - Xóa bỏ luồng 3 nút cứng nhắc. Trong đoạn văn giải thích của AI, cho phép người học **click trực tiếp vào bất kỳ câu hoặc từ khóa nào chưa hiểu (ví dụ click vào 'ranh giới cắt', 'top-k', 'đứt ngữ cảnh') để kích hoạt ô hỏi đáp đào sâu 2 chiều tại chỗ**, giúp người học tự do gõ hỏi vặn lại cho đến khi thực sự hiểu thấu đáo.
  3. **Khắc phục nỗi lo "bị động, sợ sót thông tin do AI tự kết luận" của Option C (Control chỉ 2-3/5 ở cả 3 Tester):** 
     - Loại bỏ việc AI tự động cập nhật bài làm ngầm; mọi gợi ý sửa đổi đều phải qua bước người học tự tay chọn lại sau khi đã hiểu bài qua cơ chế hỏi đào sâu.

- **Evidence dẫn tới quyết định này (Hội tụ bằng chứng từ cả 3 tester thật):**
  - **Từ Tester 1 (Cường facilitate):**
    * *"Luồng hơi ép buộc người dùng vào một khuôn, chưa cho người dùng control được."*
    * *"Khi người dùng chưa hiểu bài thì vẫn chưa biết cần hỏi AI về vấn đề gì."*
    * *"Có giải thích tổng quát nhưng chưa cho phép người dùng hỏi lại khi chưa hiểu."*
  - **Từ Tester 2 (Thăng facilitate):**
    * Nhận xét Option B: *"Đôi khi chính tôi chưa hiểu rõ là tôi nên đặt câu hỏi gì, dẫn đến việc đặt câu hỏi không tối ưu"* (Control 4/5, Help 5/5).
    * Nhận xét Option A: *"Chưa cho tự do gõ câu hỏi"* (dù khen gợi ý xuất hiện đúng lúc, ví dụ lợp ngói dễ hiểu).
    * Nhận xét Option C: *"Trải nghiệm hơi bị động, lo ngại sẽ bị sót thông tin trong một số trường hợp khi AI đã định hướng sẵn cho người dùng"* (Control chỉ 2/5).
  - **Từ Tester 3 (Dũng facilitate):**
    * Nhận xét Option A: *"Luồng gợi ý ban đầu khá định hướng; muốn hỏi một chi tiết riêng thì chưa tiện"* (Control 4/5, Help 5/5).
    * Nhận xét Option B: *"Nhiều lựa chọn can thiệp khiến tôi phải tự quyết khá nhiều; lúc đang bí kiến thức có thể không biết nên chọn cách hỏi nào trước"* (Control 5/5, Help 5/5).
    * Nhận xét Option C: *"AI tự kết luận 80% lỗi nằm ở overlap khiến tôi hơi lo: nếu nguyên nhân thật sự là Top-k hoặc đọc nhầm đề thì phải chủ động vào phần báo ngoại lệ để sửa"* (Control 3/5).
    * Trích dẫn trade-off: *"Đánh đổi là cần thêm các câu hỏi gợi ý hoặc lộ trình ngắn để người học không bị bí khi chưa biết phải yêu cầu AI hỗ trợ thế nào."*

---

## Still Unproven sau 3 feedback
1. **Nguy cơ sa đà / Chệch mục tiêu thời gian:** Cả 3 tester đều muốn đào sâu và tự do hỏi chi tiết, nhưng chưa kiểm chứng được liệu việc cho phép "click vào từ khóa để hỏi sâu vô tận" có khiến người học bị phân tâm, hỏi lan man sang các chủ đề khác và phá vỡ mục tiêu hoàn thành bài học trong <10 phút hay không.
2. **Hành vi thực tế dài hạn dưới áp lực thi cử:** Cả 3 tester đều từ chối Option C trong bài test (Control chỉ 2-3/5), nhưng chưa chứng minh được trong điều kiện áp lực thi cử cận kề hoặc bài tập dồn dập, liệu người học có vì lười mà quay lại chọn phương án "bấm Duyệt cho nhanh" như ở Option C hay không.
3. **Mức độ phụ thuộc vào trình độ người học (Novice vs Advanced):** Cả 3 tester đều là sinh viên kỹ thuật CNTT/AI/Data Science có tư duy phản biện cao. Chưa chứng minh được liệu người mới bắt đầu (novice) có cảm thấy "bị định hướng / ép khuôn" như 3 tester này hay họ thực sự lại cần một luồng cố định cầm tay chỉ việc.

---
> **ĐÁNH GIÁ GATE 5 (Learning, not praise):** Nhóm FinTech đã hoàn tất thu thập đủ 3 Feedback Notes độc lập ngoài nhóm với sự hội tụ bằng chứng hoàn hảo giữa cả 3 thành viên, ghi nhận đầy đủ hành vi thực tế, trade-off nguyên văn, bóc tách mâu thuẫn nhận thức và chốt đúng 1 Next Change cùng các câu hỏi còn bỏ ngỏ.
