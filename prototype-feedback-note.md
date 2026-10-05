# Prototype Feedback Notes — Chặng 6 · Ghi chép và learning sau test

> **Trạng thái cập nhật:** Phần Nguyễn Văn Thăng bên dưới được hoàn thiện từ feedback thực tế trong [Group Feedback Synthesis](group-feedback-synthesis.md), cột “Feedback 2 (Thăng facilitate)”. Hai phần của Dũng và Cường vẫn là bản mô phỏng cũ, giữ nguyên để từng thành viên cập nhật; không dùng hai phần đó làm evidence thực tế. Số thứ tự note trong file này theo thành viên, khác thứ tự cột trong synthesis.

## Kịch bản dùng chung — 20 phút mỗi tester

| Thời gian | Hoạt động |
|---|---|
| 0–2 phút | Opening, hỏi lần gần nhất phải dừng học vì không hiểu |
| 2–14 phút | Tự dùng từng option, khoảng 4 phút/option; reset context giữa lượt |
| 14–18 phút | So sánh, hỏi lựa chọn, phân chia việc người–AI và điểm chưa thoải mái |
| 18–20 phút | Hoàn thành note, tách observed/interpreted/decided/still unproven |

**Opening:** “Chúng mình đang thử ba cách thiết kế, không kiểm tra bạn. Không có câu trả lời đúng hoặc sai. Bạn hãy tự thao tác và nói to điều mình đang nghĩ; mình sẽ cố gắng không hướng dẫn.”

**Task:** “Bạn đang học dở bài RAG này và vừa sai quiz 2 lần. Hãy dùng từng phương án để tìm chỗ đang thiếu và quay lại làm tiếp bài. Vừa làm vừa nói to suy nghĩ.” Giữ nguyên task/fixture/desired outcome, dành khoảng 4 phút cho mỗi lượt trong buổi so sánh.

**Compare:** “Trong tình huống này, bạn chọn A, B hay C? Vì sao?” / “Bạn muốn tự làm phần nào và giao cho AI phần nào?” / “Điều gì ở phương án đã chọn khiến bạn chưa thoải mái?”

Không narrate giao diện, không hướng dẫn chọn option, không trả lời hộ khi tester im lặng. Nếu cứu hộ, ghi đúng lúc và câu đã dùng. Không lộ annotation cho tester. Tất cả tester thật phải ngoài nhóm; ưu tiên có relevant context. Nếu thiếu người/thời gian, hoàn tất ngoài giờ trước khi nộp.

## Feedback 1 — Thành viên 1 / Nguyễn Anh Dũng 

**Tester/context giả lập:** T01, người mới học RAG. Trong 7 ngày gần nhất từng dừng một bài vì nhầm embedding và từ khóa; thường tìm AI giải thích nhưng khó đánh giá câu trả lời. Vai trò giả định: ngoài nhóm. Thứ tự A → B → C. Thời lượng lượt mô phỏng: A 3:35, B 3:10, C 3:50. Không có facilitator narrate trong kịch bản.

### OBSERVED 

| Observation | Note |
|---|---|
| First action | A: đọc mô tả rồi trả lời câu chẩn đoán đầu. B: mở map và chọn Embedding. C: chọn thẻ 70% trước khi đọc hết evidence. |
| Chỗ dừng, do dự hoặc hiểu sai | B: dừng khoảng 20 giây giữa Embedding và Top-k, đổi thẻ. C: hỏi “70% là chắc mình thiếu phần này à?” . |
| Evidence được đọc hay bỏ qua | A: đọc lý do sau chẩn đoán. B: nhìn highlight slide cũ. C: đọc evidence sau khi đã chọn; bỏ qua giới hạn ở thẻ Overlap. |
| Cách sửa/lấy lại control | B: đổi Embedding sang Top-k. C: từ preview bấm đổi lựa chọn rồi quay lại thẻ đầu; quay về quiz sau phần ôn. |
| Option được chọn | **A** |
| Lý do và trade-off | Lời nói giả lập: “Em chưa biết mình thiếu gì, trả lời mấy câu dễ hơn tự chọn.” Chấp nhận thêm bước hỏi để bớt phải tự đoán; không muốn luồng hỏi kéo dài. |
| Evidence chống lại kỳ vọng | C có evidence nhưng tester vẫn chọn theo % trước. B thao tác ít nhưng không giúp người mới tự quyết nhanh. |

### INTERPRETED

Người mới có thể cần bước gợi mở trước khi tự chốt phần ôn. Nhãn số của C có thể tạo cảm giác AI đã chẩn đoán, dù giao diện có cảnh báo. Ít thao tác không đồng nghĩa ít tải nhận thức.

### DECIDED — NEXT CHANGE 

Test C với nhãn chắc bằng lời và evidence sát lựa chọn; quan sát người mới có chọn sau khi đọc lý do hay vẫn dựa vào độ chắc. Giữ quyền phủ quyết của C.

### STILL UNPROVEN

Chưa biết A có chẩn đoán đúng, giúp hiểu lâu dài hay phù hợp với người mới nói chung. Sự lựa chọn A trong một kịch bản không chứng minh A hiệu quả nhất.

## Feedback 2 — Thành viên 2 / Tạ Việt Cường 

**Tester/context giả lập:** T02, đã làm một bài tập RAG nhỏ. Trong 7 ngày gần nhất từng phải tra lại top-k; thường biết tên khái niệm mình đang nhầm. Vai trò giả định: ngoài nhóm. Thứ tự B → C → A để giảm việc option cuối luôn hưởng lợi từ lượt trước. Thời lượng lượt mô phỏng: B 2:15, C 3:20, A 3:40. Không có facilitator narrate trong kịch bản.

### OBSERVED — hành vi/lời nói giả lập

| Observation | Note |
|---|---|
| First action | B: chọn Top-k từ map. C: đối chiếu hai thẻ với đáp án sai về top-k. A: trả lời câu đầu, sau đó tìm đường bỏ qua câu tiếp. |
| Chỗ dừng, do dự hoặc hiểu sai | C: dừng khi không thấy Top-k trong hai gợi ý đầu. A: hỏi liệu có thể ôn thẳng phần đã biết mình cần hay không. |
| Evidence được đọc hay bỏ qua | B: đọc tên nền và nội dung ôn, không đọc highlight lịch sử. C: đọc evidence top-k, bỏ qua lịch sử video embedding. A: lướt lý do chẩn đoán. |
| Cách sửa/lấy lại control | C: chọn “Cả hai đều không đúng” → Top-k → preview → quiz. A: chọn quay lại bài ngay thay vì đi hết luồng. |
| Option được chọn | **B** |
| Lý do và trade-off | Lời nói giả lập: “Mình biết đang nhầm top-k; cho chọn thẳng là được.” Muốn tự chọn nền, giao công cụ việc trình bày ôn; chấp nhận rủi ro tự chọn sai. |
| Evidence chống lại kỳ vọng | Hai gợi ý AI của C không khớp nhu cầu tự nhận biết. A thêm chẩn đoán khiến người đã biết chỗ thiếu muốn bỏ qua. |

### INTERPRETED

Với người đã biết tên phần cần ôn, tự chọn có thể hữu ích hơn giải thích về suy luận AI. Recovery của C giữ được agency, nhưng phải đọc hai thẻ rồi phủ quyết vẫn tốn công hơn B.

### DECIDED — NEXT CHANGE

Trong C, làm quyền “không đúng / tự chọn phần khác” dễ nhận thấy ngay khi so sánh gợi ý. Không biến C thành luồng AI bắt buộc phải chấp nhận.

### STILL UNPROVEN

Chưa biết T02 tự xác định đúng chỗ hổng trong các bài khó hơn. Không suy ra B tốt nhất cho tất cả người học từ khả năng tự chọn trong tình huống này.

## Feedback 3 — Thành viên 3 / Nguyễn Văn Thăng

**Facilitator:** Nguyễn Văn Thăng — 2A202602835.  
**Tester/context:** Một tester ngoài nhóm, theo phiên do Thăng facilitate được ghi trong Group Feedback Synthesis. Synthesis mô tả cả ba tester thuộc nhóm sinh viên kỹ thuật CNTT/AI/Data Science; không ghi riêng tên, ngành cụ thể hoặc kinh nghiệm RAG của tester này.  
**Task:** Dùng cả A/B/C trong tình huống đang học bài RAG và vừa sai quiz hai lần, tìm phần chưa hiểu để quay lại làm tiếp.  
**Thứ tự thực tế:** A → B → C.  
**Thời lượng:** Protocol chung khoảng 20 phút/tester; nguồn tổng hợp không ghi thời lượng thực tế từng lượt.  
**Nguồn ghi chép:** [Group Feedback Synthesis](group-feedback-synthesis.md), cột “Feedback 2 (Thăng facilitate)” và phần evidence từ Tester 2. Nguồn chưa ghi thời điểm/câu cứu hộ hoặc kết quả quiz sau test.

### OBSERVED — hành vi, lời nói và điểm đánh giá thực tế

| Observation | Note |
|---|---|
| First action | Tester thử lần lượt A → B → C; đọc kỹ ví dụ lợp ngói ở A và mở khung chat ở B. |
| Chỗ dừng, do dự hoặc chưa hài lòng | **A:** “Chưa cho tự do gõ câu hỏi”. **B:** “Đôi khi chính tôi chưa hiểu rõ là tôi nên đặt câu hỏi gì, dẫn đến việc đặt câu hỏi không tối ưu”. **C:** “Trải nghiệm hơi bị động, lo ngại sẽ bị sót thông tin trong một số trường hợp khi AI đã định hướng sẵn cho người dùng”. |
| Evidence được đọc hay bỏ qua | Ghi nhận tester đọc kỹ ví dụ lợp ngói ở A; feedback khen gợi ý xuất hiện đúng lúc và ví dụ dễ hiểu. Chưa có ghi chép cụ thể về việc đọc/bỏ qua evidence hoặc log ở B/C. |
| Cách sửa/lấy lại control | Tester tìm kiếm ô gõ câu hỏi tự do ở A; đánh giá Control của C chỉ 2/5 và nêu lo ngại về định hướng sẵn. Đây là phản hồi về quyền kiểm soát; nguồn chưa ghi tester đã bấm Báo ngoại lệ ở C. |
| Option được chọn | **Chưa chốt; phân vân giữa A và B.** Thích ví dụ ở A nhưng muốn tự do gõ câu hỏi ở B. Không ghi nhận lựa chọn C. |
| Lý do và trade-off | “Option C rất nhanh nhưng đánh đổi bằng việc bị động và dễ sót ý; Option B tự do nhưng tốn công nghĩ câu hỏi tối ưu; Option A dễ hiểu nhất nhưng bị gò bó.” |
| Evidence chống lại kỳ vọng | A được chấm Control 5/5 và Help 5/5 nhưng tester vẫn yêu cầu quyền gõ hỏi tự do. B có Help 5/5 nhưng người học chưa biết nên hỏi gì. C nhanh nhưng Control chỉ 2/5; tốc độ không đủ để tester chọn C. |

**Điểm tester tự đánh giá** (giữ nguyên theo synthesis):

| Tiêu chí | Option A | Option B | Option C |
|---|---|---|---|
| Control — Quyền kiểm soát | 5/5 | 4/5 | 2/5 |
| Help — Độ hữu ích | 5/5 | 5/5 | 4/5 |

### INTERPRETED — diễn giải từ evidence

- Ví dụ trực quan và gợi ý đúng lúc của A có ích với tester, nhưng lời yêu cầu “tự do gõ câu hỏi” cho thấy người học vẫn muốn hỏi lại một chi tiết cụ thể. Điểm Control cao không xóa đi hạn chế này.
- B cho phép chủ động tương tác, nhưng quyền tự đặt câu hỏi cũng làm người đang bí kiến thức phải tự xác định điểm cần hỏi. Tester có thể cần một vài câu hỏi khởi đầu theo ngữ cảnh thay vì bắt đầu từ khung chat trống.
- C được nhìn nhận là nhanh nhưng bị động. Lo ngại sót ý cùng Control 2/5 gợi ý rằng người học muốn kiểm tra và điều chỉnh hướng ôn trước khi áp dụng.
- Việc phân vân A/B gợi ý nhu cầu kết hợp gợi mở dễ hiểu với đối thoại tự do. Đây là diễn giải cho phiên này; chưa chứng minh cơ chế kết hợp sẽ cải thiện kết quả học.

### DECIDED — NEXT CHANGE

**Theo quyết định chung của nhóm:** thử một hướng **“Hybrid Scaffolded Drill-down” — gợi ý ban đầu kết hợp hỏi đáp đào sâu theo ngữ cảnh**.

Cơ chế thử tiếp: AI đưa chẩn đoán ban đầu dưới dạng gợi ý kèm 2–3 câu hỏi khởi đầu; người học click câu/từ khóa chưa hiểu để mở hỏi đáp tại chỗ và tự gõ hỏi lại; mọi sửa đổi bài làm đều cần người học tự chọn, không tự cập nhật ngầm. Đây là một hướng thiết kế thống nhất, chưa được áp dụng vào bản prototype hiện tại.

**Evidence cá nhân dẫn tới hướng này:** B khiến tester chưa biết đặt câu hỏi gì → cần gợi ý khởi đầu; A chưa cho gõ hỏi tự do → cần đối thoại tại phần chưa hiểu; C bị đánh giá bị động, Control 2/5 → giữ quyền quyết định việc áp dụng ở người học. Không dùng feedback này để chốt B là lựa chọn cuối của tester hoặc giữ C chỉ bằng việc đổi nhãn độ chắc.

**Phần cần sửa ở Option C tôi phụ trách:** trình bày kết luận như gợi ý có thể chất vấn; mở đường hỏi lại/đổi trọng tâm ngay tại nội dung giải thích; để người học tự chọn sửa đáp án sau khi hiểu. Kiểm tra lại với cùng task RAG xem tester có bắt đầu hỏi dễ hơn và chủ động xác nhận/sửa hướng ôn hay không.

### STILL UNPROVEN

1. Chưa có kết quả quiz sau test hoặc đo thời gian hoàn thành; chưa biết hướng mới giúp hiểu đúng nền và quay lại bài trong dưới 10 phút hay không.
2. Chưa biết câu hỏi khởi đầu có giảm khó khăn khi chưa biết hỏi gì, hay tiếp tục định hướng sai và làm sót ý.
3. Chưa biết hỏi đào sâu có khiến người học đi lan man, kéo dài thời gian hoặc bỏ mục tiêu ban đầu.
4. Chưa biết lựa chọn và mức độ chủ động có thay đổi khi chịu áp lực thi cử; kết quả từ nhóm tester kỹ thuật chưa đại diện cho người mới bắt đầu.

## Trạng thái hồ sơ sau cập nhật

- [x] Có protocol chung và nhiệm vụ mỗi thành viên test cả A/B/C.
- [x] Có bản build A/B/C trong thư mục `prototype/` và bộ trải nghiệm trong `test/`.
- [x] Synthesis ghi nhận ba phiên độc lập ngoài nhóm, pattern/khác biệt, một Next Change và Still Unproven.
- [x] Phần Nguyễn Văn Thăng đã thay dữ liệu mô phỏng bằng evidence trong synthesis, tách Observed / Interpreted / Decided / Still Unproven.
- [ ] Hai phần note của Dũng/Cường trong file này cần được từng thành viên cập nhật từ ghi chép thực tế.
- [ ] Triển khai và test lại hướng Hybrid Scaffolded Drill-down.

**GATE 5 — Learning:** Bản synthesis đã ghi learning sau ba phiên test theo dữ liệu nhóm cung cấp. Phần cá nhân của Thăng đã đối chiếu theo nguồn đó; file notes này vẫn còn hai phần mô phỏng của thành viên khác. Việc chốt Next Change chưa chứng minh giải pháp đã được validated.

