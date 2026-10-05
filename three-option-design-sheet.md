# Three-Option Design Sheet — Nhóm FinTech | Case A AI Tutor: Diagnostic Refresher

> Phân công build: Option A — Nguyễn Anh Dũng · Option B — Tạ Việt Cường (2A202602560) · Option C — Nguyễn Văn Thăng

---

## CHẶNG 1 — Tổng hợp evidence (15 phút)

### 1.1. Evidence huddle — 3 Practice Notes đặt cạnh nhau

> Nguyên tắc: mỗi dòng là hành vi/lời nói đã ghi, tách khỏi diễn giải. Không bịa quote. Notes 2-3 do Thăng/Dũng điền nguyên văn trong lab.

| Practice Note | User đã thực sự làm/nói gì? (Observed) | Điều nhóm đang diễn giải (Interpreted — chưa kết luận) |
|---|---|---|
| 1 — Cường facilitate (01/10, bài RAG trên VLearn) | Học viên làm sai 2 lần câu quiz về chia đoạn văn bản (chunking) và chọn top-k ở bài trắc nghiệm cuối bài. Xem lại slide 8-10, Google "RAG chunk overlap bao nhiêu là đủ", xem video YouTube 18 phút về vector hoá văn bản (embedding), nhắn hỏi bạn cùng phòng. Nói "mất gần 1 tiếng mà vẫn sai câu top-k, thôi tắt máy đi ngủ". | Có workaround tốn công (slide cũ + Google + YouTube + hỏi bạn). Có hậu quả: mất ~60 phút, làm sai tiếp, bỏ dở buổi học. Gợi ý Pain A (không biết thiếu gì nên ôn lan man). |
| 2 — Thăng facilitate | Khi gặp một khái niệm không hiểu, học viên quay lại bài học trước để tìm nội dung liên quan nhưng không biết chính xác cần xem lại phần nào. | Học viên nhận ra mình đang thiếu kiến thức nhưng khó xác định chính xác kiến thức nền bị hổng. |
| 3 — Dũng facilitate | Khi được hỏi thời gian xử lý phần chưa hiểu bằng trợ lý AI, người học nói: "Thì nó mất khoảng tầm 1 đến 2 phút thôi." (02:29, bản chép lời Day 17). | Workaround bằng AI có thể đang đáp ứng khá nhanh nhiều câu hỏi của người học. Chi tiết này làm yếu giả định rằng việc tìm giải thích luôn tốn nhiều thời gian; chưa đủ để kết luận người học khó xác định kiến thức nền bị thiếu hoặc cần Diagnostic Refresher. |

**Thảo luận nhanh (đủ 3 notes — chốt Chặng 1):**
- Situation/behavior/workaround lặp lại >1 lần: ✅ Note 1 (Cường) + Note 2 (Thăng) cùng pattern "quay lại bài cũ/slide cũ nhưng không biết xem lại phần nào" → ôn lan man. Note 1 chi tiết 4 bước (slide 8-10 + Google + YouTube 18' + hỏi bạn), Note 2 xác nhận hành vi quay lại bài trước nhưng mù chỗ cần xem.
- Evidence mâu thuẫn/gây bất ngờ: ⚠️ Note 3 (Dũng) làm yếu vế consequence "tốn 30-60 phút": khi dùng trợ lý AI, user chỉ mất 1-2 phút cho phần chưa hiểu. Nghĩa là hậu quả nặng chỉ đúng với workaround thủ công (tự tìm slide/Google/YouTube), chưa chắc đúng khi đã có AI. Note 3 chưa bác Pain A (vẫn chưa rõ user có tự xác định được chỗ hổng không), nhưng buộc nhóm thu hẹp phạm vi: problem đáng giải là ca tự xoay xở không AI / AI trả lời chung chung sai chỗ.
- Điều vẫn chỉ là suy đoán: (1) Pain A vs Pain B — nếu AI đã trả lời nhanh thì vấn đề còn lại có phải là ôn đúng nền + quay lại mạch học không? (2) Tần suất ≥2 lần/tháng có đúng cả 3 ca không? (3) User có tự ôn + quay lại làm tiếp nếu được chỉ đúng chỗ không?

### 1.2. Chốt Hypothesis Problem (giữ đúng cấu trúc Day 17)

> Khi [situation], [user] gặp khó khăn trong việc [job] vì [barrier], dẫn đến [consequence].

**Hypothesis Problem nhóm tiếp tục dùng trong Day 18:**

> Khi đang học bài mới trên VLearn mà bị mắc kẹt ở đoạn không hiểu (ví dụ: làm sai quiz cuối bài), người học gặp khó khăn trong việc hiểu tiếp bài để làm được bài tập vì không xác định được mình đang thiếu khái niệm nền nào nên ôn lan man / sai chỗ, dẫn đến tốn 30–60 phút mà vẫn không hiểu, làm sai tiếp và dễ bỏ dở bài.

**Evidence ban đầu hỗ trợ giả thuyết:**
- Note 1 (Cường): tình huống thật trong 7 ngày (tối 01/10, bài RAG, nhớ rõ môn/bài/câu sai), workaround 4 bước tốn công, hậu quả đo được (mất ~60 phút, sai tiếp câu top-k, tắt máy bỏ bài).
- Note 2 (Thăng): hội tụ với Note 1 ở barrier "không biết chính xác cần xem lại phần nào" dù đã chủ động quay lại bài trước. Củng cố Pain A: có nhận ra thiếu kiến thức nhưng không xác định được chỗ hổng.
- Note 3 (Dũng) — phản biện biên: quote nguyên văn "mất khoảng tầm 1 đến 2 phút thôi" (02:29) cho thấy workaround bằng AI hiện đã nhanh. Nhóm không dùng Note 3 để bác Pain A, mà để giới hạn phạm vi Day 18: test 3 options trong ca workaround thủ công / AI trả lời chưa đúng nền, nơi hậu quả tốn thời gian + bỏ bài vẫn còn.

**Điều vẫn chưa được chứng minh (Still Unknown sau Day 17):**
1. Pain A có phải nguyên nhân chính hay chỉ là Pain B (đứt mạch do phải rời bài)? Nếu B đúng thì không cần chẩn đoán lịch sử học.
2. Tần suất và mức độ hậu quả có đáng giải quyết (≥2 lần/tháng, >15 phút) với đa số người học hay chỉ 1 ca lẻ?
3. Người học có tự thay đổi hành vi (tự ôn + quay lại làm tiếp) nếu được chỉ đúng chỗ hay vẫn bỏ qua?

**GATE 1 — Evidence continuity:** ✅ Hypothesis có đủ user + situation + job + barrier + consequence; nối được với ít nhất 1 observation Day 17 (Note 1) và ghi rõ 3 điều chưa biết trên. Không coi Practice Notes là validation.

---

## CHẶNG 2 — Chọn ba Solution Options (20 phút)

### 2.1. Những thứ giữ nguyên cho A/B/C (Comparison Contract)

| Thành phần | Quyết định chung |
|---|---|
| Target user | Người học VLearn đang học bài mới |
| Situation | Giữa bài RAG, vừa sai quiz 2 lần về chunk overlap + top-k |
| Task | Hiểu tiếp để làm đúng quiz và quay lại bài cũ trong <10 phút |
| Desired outcome | Tự ôn đúng khái niệm nền và quay lại làm tiếp, không bỏ bài |
| Content/data fixture | Slide 8-10 tóm tắt, 2 câu quiz sai, lịch sử: đã xem embedding 18 phút, slide 8-10 đã mở 2 lần |

### 2.2. Những thứ được phép khác

| Thành phần | Option A — AI gợi ý dẫn dắt (Dũng) | Option B — Đối thoại 2 chiều & Quyền User (Cường) | Option C — Tự động ngầm & Duyệt ngoại lệ (Thăng) |
|---|---|---|---|
| Solution mechanism | 3 bước rõ ràng: Trước kích hoạt (Pre-activation banner) → AI chủ động phân tích & gợi ý giải pháp → Thao tác người dùng (Chấp nhận / Đổi / Từ chối). | Luồng đối thoại 2 chiều Người ↔ AI. Người dùng nắm quyền cao nhất, có bộ nút can thiệp/chỉnh sửa trực tiếp góc độ giải thích của AI và tự sửa ghi chú. | AI tự động xử lý ngầm (Background Pipeline) ngay khi sai quiz. Người dùng kiểm soát tại Điểm Duyệt kết quả (Approve) và Điểm Can thiệp qua ngoại lệ (Exception). |
| User làm gì? | Thấy mời gọi → Bấm kích hoạt → Đọc gợi ý của AI → Chọn thao tác phản hồi (chấp nhận/đổi/từ chối). | Chủ động đặt câu hỏi, bấm các nút chỉnh sửa (đổi sang ví dụ đời thực, bảng so sánh, tóm tắt siêu ngắn) và tự gõ sửa ghi chú. | Đọc kết quả soạn sẵn, bấm [Duyệt & Áp dụng] hoặc bấm [Báo ngoại lệ] chọn lý do AI đoán sai để thu hồi quyền tự động. |
| AI làm gì? | Quét câu sai + lịch sử → Chủ động gợi ý giải thích phần Chunk Overlap. | Đóng vai trò đối tác đối thoại 2 chiều, phản hồi tức thì và thích ứng theo mệnh lệnh chỉnh sửa của User. | Chạy ngầm phát hiện lỗi sai, quét lịch sử, tự soạn thảo sẵn gói giải pháp 60s và chờ phê duyệt. |
| Trigger | Xuất hiện banner mời kích hoạt sau lần sai thứ 2. | Người dùng chủ động mở luồng đối thoại và bấm nút điều phối. | Tự động kích hoạt ngầm ngay sau lần nộp quiz sai thứ 2. |
| Trade-off chính | Luồng rõ ràng, trực quan nhưng người học bị dẫn dắt theo khuôn. | Quyền kiểm soát tối đa, linh hoạt nhưng đòi hỏi người học phải chủ động tương tác. | Cực kỳ rảnh tay, nhanh chóng nhưng dễ chủ quan duyệt ẩu nếu không để ý ngoại lệ. |

### 2.3. Distance check (không nhắc màu/layout/wording)

- **A khác B vì:** A là luồng AI gợi ý sẵn và dẫn dắt 3 bước có sẵn; B là luồng đối thoại 2 chiều linh hoạt do User toàn quyền điều phối bằng các nút chỉnh sửa can thiệp.
- **B khác C vì:** B yêu cầu User chủ động đối thoại và trực tiếp nắn dòng suy nghĩ của AI; C là AI tự động xử lý ngầm từ trước, User chỉ đóng vai trò chốt duyệt hoặc báo ngoại lệ.
- **A khác C vì:** A yêu cầu người dùng kích hoạt và đi qua từng bước gợi ý; C đã hoàn tất xử lý ngầm từ trước mà không cần kích hoạt thủ công, đặt trọng tâm vào cơ chế can thiệp ngoại lệ.

Spectrum: B (USER-LED & TWO-WAY AGENCY) → A (AI-INITIATED & GUIDED) → C (AUTONOMOUS BACKGROUND & EXCEPTION/APPROVAL). Không làm option tệ cố ý.

**GATE 2 — Meaningful options:** ✅ Cùng user/situation/task/outcome/fixture, khác mechanism và chia việc user–AI rõ rệt.

---

## CHẶNG 3 — Human–AI Design pass (30 phút, chỉ critical interaction)

| Human–AI decision | Option A | Option B (Cường phụ trách) | Option C |
|---|---|---|---|
| User làm gì? AI làm gì? | User duyệt qua 3 bước: trước kích hoạt → nhận AI gợi ý → thao tác ra quyết định. AI chủ động gợi ý. | User đối thoại 2 chiều, bấm nút chỉnh sửa góc độ của AI và sửa ghi chú. AI thích ứng theo lệnh User. | User bấm Duyệt kết quả hoặc Can thiệp báo ngoại lệ. AI tự động chạy ngầm chuẩn bị sẵn giải pháp. |
| AI Act / Ask / Don't Act? Vì sao? | **Ask rồi Act (Guided Suggestion)** — Hỏi xác nhận kích hoạt trước khi đưa ra gợi ý, tránh làm phiền khi người học muốn tự suy nghĩ. | **User-Led / Don't Act độc quyền** — AI không tự phán xét mà lắng nghe và phục tùng các nút chỉnh sửa/kiểm soát của User. | **Autonomous Act with Human Exception** — AI tự động hành động ngầm vì chi phí thấp, nhưng bắt buộc dừng lại ở chốt chặn Duyệt & Báo ngoại lệ. |
| User hiểu capability/limit bằng gì? | Banner trước kích hoạt nói rõ: AI quét 2 câu sai để gợi ý, người học hoàn toàn có quyền từ chối. | Dòng cam kết quyền lực: "Bạn nắm quyền kiểm soát, AI là đối tác đối thoại; sử dụng các nút chỉnh sửa để điều phối". | Log ngầm minh bạch từng bước xử lý dữ liệu và thông báo: "Kết quả do AI chuẩn bị sẵn, cần bạn duyệt hoặc báo ngoại lệ". |
| Evidence/uncertainty thể hiện thế nào? | Hiển thị nhãn độ liên quan 92% kèm trích dẫn nguyên nhân vì sao AI chọn gợi ý Chunk Overlap. | Minh bạch qua phản hồi đối thoại; hiển thị bảng so sánh trực tiếp hậu quả giữa 0 từ và 50 từ khi User yêu cầu. | Hiển thị Background Event Logs chân thực, phân tích rõ câu sai và thời lượng xem video; cung cấp danh sách 3 lý do ngoại lệ khi AI đoán sai. |
| User kiểm soát và recovery thế nào? | Nút bỏ qua trước kích hoạt, nút yêu cầu AI đổi trọng tâm, nút từ chối gợi ý quay về bài học gốc, nút Trang chủ. | Bộ nút chỉnh sửa góc độ giải thích, nút khôi phục đối thoại, ô tự chỉnh sửa ghi chú, nút Trang chủ. | Nút [BÁO NGOẠI LỆ / CAN THIỆP] để hủy tự động hóa và chuyển sang Option B hoặc tự học, nút Trang chủ. |

Feedback/data check: fixture là canned, không dùng dữ liệu nhạy cảm thật. Nếu lưu lựa chọn: chỉ ảnh hưởng phiên hiện tại, có nút "Xoá lựa chọn của tôi".

**GATE 3 — Human control:** ✅ Mỗi option có expectation rõ, agency phù hợp hậu quả sai, và ≥1 đường kiểm soát/phục hồi về task gốc.

