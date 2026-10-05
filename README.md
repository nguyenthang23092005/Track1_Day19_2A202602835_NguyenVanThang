# Track 1 — Day 19 · Three prototypes, one next change

## 1. Thông tin cá nhân và nhóm

| Nội dung | Thông tin |
|---|---|
| MHV | **2A202602835** |
| Họ tên | **Nguyễn Văn Thăng** |
| Tên nhóm | **FinTech** |
| Case | **Case A — AI Tutor: Diagnostic Refresher** |
| Option cá nhân chịu trách nhiệm | **C — AI tự động xử lý ngầm, duyệt kết quả và báo ngoại lệ** |
| Tên repo | `Track1_Day19_2A202602835_NguyenVanThang` |

| Thành viên | Phân công thiết kế/build | Feedback trong synthesis |
|---|---|---|
| Nguyễn Anh Dũng | Option A — AI gợi ý dẫn dắt | Feedback 3 — test cả A/B/C với một tester ngoài nhóm |
| Tạ Việt Cường — 2A202602560 | Option B — Đối thoại hai chiều, người học điều phối | Feedback 1 — test cả A/B/C với một tester ngoài nhóm |
| Nguyễn Văn Thăng — 2A202602835 | Option C — AI xử lý ngầm, duyệt/báo ngoại lệ | Feedback 2 — test cả A/B/C với một tester ngoài nhóm |

Nhóm đã tổng hợp đủ ba phiên test độc lập trong [Group Feedback Synthesis](group-feedback-synthesis.md). Số thứ tự tại đó theo Cường → Thăng → Dũng; file notes sắp theo Dũng → Cường → Thăng.

## 2. Hypothesis Problem

**Giả thuyết nhóm tiếp tục dùng**, nối với [Three-Option Design Sheet](three-option-design-sheet.md):

> Khi đang học bài mới trên VLearn mà bị mắc kẹt ở đoạn không hiểu (ví dụ: làm sai quiz cuối bài), người học gặp khó khăn trong việc hiểu tiếp bài để làm được bài tập vì không xác định được mình đang thiếu khái niệm nền nào nên ôn lan man / sai chỗ, dẫn đến tốn 30–60 phút mà vẫn không hiểu, làm sai tiếp và dễ bỏ dở bài.

**Evidence từ Day 17:** Note 1 của Cường ghi học viên làm sai quiz RAG hai lần, xem slide 8–10, tìm Google/YouTube và hỏi bạn nhưng vẫn sai top-k, rồi bỏ dở. Note 2 do tôi facilitate ghi nhận người học quay lại bài trước nhưng không biết chính xác cần xem phần nào. Hai note hỗ trợ barrier “không biết thiếu nền nào”.

**Evidence phản biện:** Note 3 của Dũng ghi người học chỉ mất khoảng 1–2 phút khi dùng trợ lý AI. Hậu quả 30–60 phút chưa thể áp cho mọi người; phạm vi cần kiểm tra là ca tự tìm nguồn hoặc được AI giải thích chưa đúng chỗ.

**Still Unknown:** Chưa biết thiếu nền hay đứt mạch học là nguyên nhân chính, mức hậu quả có phổ biến hay không, và việc gợi ý đúng phần ôn có khiến người học hiểu rồi làm tiếp bài hay không. Ba phiên prototype test cung cấp learning về tương tác, chưa xác nhận toàn bộ giả thuyết này.

## 3. Three Solution Options và cách mở prototype

| Option | Cơ chế và cách chia việc người–AI | Prototype |
|---|---|---|
| **A — AI gợi ý dẫn dắt** | User kích hoạt từ banner; AI phân tích câu sai và gợi ý giải thích; user chấp nhận, yêu cầu đổi trọng tâm hoặc từ chối | [Option A](prototype/option-a.html) |
| **B — Đối thoại hai chiều, người học điều phối** | User đặt câu hỏi, đổi góc độ giải thích, chuyển sang Top-k và tự sửa ghi chú; AI phản hồi theo tương tác của user | [Option B](prototype/option-b.html) |
| **C — AI xử lý ngầm, duyệt/báo ngoại lệ** | AI tự chuẩn bị gói ôn sau khi sai quiz; user đọc kết quả, duyệt để áp dụng hoặc báo ngoại lệ khi AI suy luận sai | [Option C](prototype/option-c.html) |

**Comparison contract:** Cùng người học VLearn, bài RAG, tình huống sai quiz hai lần, slide 8–10, lịch sử mẫu đã xem video embedding 18 phút; cùng task tìm phần chưa hiểu để quay lại quiz. Desired outcome là tự ôn đúng nền, làm tiếp bài trong dưới 10 phút và không bỏ dở. A/B/C khác cơ chế tương tác và cách phân chia quyền chủ động giữa người và AI.

**Cách chạy:** Tải toàn bộ repo, giữ nguyên cấu trúc thư mục, mở [Màn 0 chung](prototype/index.html) bằng Chrome/Edge và chọn A/B/C. Mỗi option có nút Trang chủ. Các trang HTML dùng chung `style.css`, JavaScript nằm trong từng trang; không cần server hay API AI. Nội dung và phản hồi AI là dữ liệu mẫu đã lập trình sẵn. Các nhãn độ chắc như 92% ở A hoặc 80% ở C là mô phỏng, chưa được đo độ chính xác.

**Bộ trải nghiệm dành cho tester:** Mở [test/index.html](test/index.html), thử A → B → C, điền Control/Help và nhận xét từng phương án, rồi so sánh. Bộ này có ô nhập câu hỏi ở B và lưu feedback bằng `localStorage` trong trình duyệt. Đây là thư mục giao diện thử nghiệm, không phải bộ test tự động.

Tài liệu thiết kế: [Design Sheet](three-option-design-sheet.md) · [Prototype Link](prototype-link.md). Một số mô tả trong Prototype Link còn thuộc thiết kế cũ (B sơ đồ nền, C hai giả thuyết); bảng trên phản ánh cơ chế trong bản build và synthesis hiện tại. Hướng thay đổi sau test ở mục 5 chưa được triển khai vào HTML.

## 4. Đóng góp của tôi trong nhóm

Tôi phụ trách **Option C**, với trọng tâm là cách người học kiểm soát kết quả AI đã chuẩn bị sẵn:

- **Thiết kế tương tác:** AI xử lý ngầm sau hai lần sai quiz; người học có điểm duyệt kết quả và điểm can thiệp báo ngoại lệ để đổi hướng hoặc thu hồi quyền tự động.
- **Bản build bàn giao:** [prototype/option-c.html](prototype/option-c.html) hiển thị log xử lý, gói ôn đề xuất và các lựa chọn can thiệp; [test/option-c.html](test/option-c.html) bổ sung phần ghi nhận feedback. Code triển khai có hỗ trợ AI.
- **Test và ghi nhận:** Tôi facilitate một tester ngoài nhóm thử A → B → C; ghi nhận việc đọc ví dụ ở A, mở chat ở B, nhu cầu gõ câu hỏi tự do và lo ngại bị động ở C. Điểm và lời nói được đối chiếu trong [note cá nhân](prototype-feedback-note.md#feedback-3--thành-viên-3--nguyễn-văn-thăng).
- **Learning cho nhóm:** Feedback của phiên tôi cho thấy tốc độ của C chưa bù được cảm giác thiếu kiểm soát. Tester phân vân A/B, muốn vừa có ví dụ/gợi mở vừa có quyền tự hỏi lại. Evidence này góp vào hướng thay đổi chung của nhóm.

Ở Day 17, Practice Note 2 do tôi facilitate cung cấp evidence về việc quay lại bài cũ nhưng không xác định được phần cần xem. Ở lần test prototype này, nguồn tổng hợp chưa ghi kết quả quiz sau test hoặc thời gian hoàn thành thực tế; tôi không dùng điểm hữu ích để suy ra hiệu quả học tập.

## 5. Prototype Feedback và một Next Change

**Feedback cá nhân:** [Feedback 3 — Nguyễn Văn Thăng](prototype-feedback-note.md#feedback-3--thành-viên-3--nguyễn-văn-thăng), tương ứng cột Feedback 2 trong synthesis.

| Option | Control | Help | Feedback chính từ tester của tôi |
|---|---|---|---|
| A | 5/5 | 5/5 | Đọc kỹ ví dụ lợp ngói, thấy dễ hiểu nhưng “Chưa cho tự do gõ câu hỏi” |
| B | 4/5 | 5/5 | Mở chat nhưng “Đôi khi chính tôi chưa hiểu rõ là tôi nên đặt câu hỏi gì, dẫn đến việc đặt câu hỏi không tối ưu” |
| C | 2/5 | 4/5 | “Trải nghiệm hơi bị động, lo ngại sẽ bị sót thông tin trong một số trường hợp khi AI đã định hướng sẵn cho người dùng” |

**Lựa chọn:** Tester của tôi **chưa chốt, phân vân giữa A và B**. Trade-off được ghi trong synthesis: “Option C rất nhanh nhưng đánh đổi bằng việc bị động và dễ sót ý; Option B tự do nhưng tốn công nghĩ câu hỏi tối ưu; Option A dễ hiểu nhất nhưng bị gò bó.”

**Tổng hợp ba phiên:** [Group Feedback Synthesis](group-feedback-synthesis.md) ghi hai tester chọn B, một tester phân vân A/B, không tester nào chọn C làm phương án học lâu dài. Các phản hồi gặp nhau ở ba điểm: A dễ hiểu nhưng thiếu tiện lợi khi hỏi riêng; B chủ động nhưng người đang bí chưa biết hỏi gì; C nhanh nhưng tạo lo ngại định hướng sai/sót thông tin. Đây là pattern trong ba phiên, chưa phải bằng chứng B hiệu quả hơn về kết quả học.

**Một Next Change nhóm chốt:** **Hybrid Scaffolded Drill-down — gợi ý ban đầu kết hợp hỏi đáp đào sâu theo ngữ cảnh**. Cơ chế gồm ba phần phục vụ cùng một hướng:

1. AI đưa gợi ý chẩn đoán ban đầu và 2–3 câu hỏi khởi đầu cụ thể, giúp người chưa biết hỏi gì bắt đầu.
2. Người học click câu hoặc từ khóa chưa hiểu để mở hỏi đáp tại chỗ, tự gõ hỏi lại và đổi trọng tâm.
3. Người học tự chọn mọi sửa đổi bài làm sau khi hiểu; bỏ cơ chế tự cập nhật ngầm.

Hướng này dùng evidence từ cả ba phiên: cần gợi mở ở B, cần hỏi lại ở A, cần giữ quyền kiểm soát ở C. Với phần C tôi phụ trách, lần sửa tiếp theo sẽ đưa quyền chất vấn/đổi hướng ngay tại nội dung đề xuất và giữ việc chọn đáp án ở người học. **Đây là quyết định thiết kế sau test, chưa phải tính năng đã triển khai hoặc đã test lại.**

**Still Unproven:** Chưa biết hỏi đào sâu có khiến người học lan man và vượt mục tiêu dưới 10 phút; hành vi có thay đổi dưới áp lực thi cử hay không; người mới có cần luồng cố định hơn nhóm tester kỹ thuật hay không. Chưa có đo kết quả quiz để kết luận hướng mới giúp hiểu đúng nền.

**Trạng thái notes:** Phần cá nhân của tôi đã cập nhật từ synthesis. Hai phần Dũng/Cường trong cùng file vẫn là bản mô phỏng cũ, cần từng thành viên cập nhật từ ghi chép thực tế. Kết quả chung ở README lấy từ synthesis đã hoàn thiện, không lấy từ hai note mô phỏng đó.

## 6. AI Support Log

Xem [AI Support Log](ai-support-log.md) để theo dõi hỗ trợ AI và giới hạn sử dụng. Log còn mô tả bản C cũ dạng hai giả thuyết/một HTML và dẫn tới annotation/QA report không có trong repo hiện tại; những mục đó cần đối chiếu lại trước khi nộp.

**AI hỗ trợ:** Tổ chức tài liệu theo Design Sheet, triển khai giao diện HTML/CSS/JavaScript và chuẩn bị protocol/mẫu note. Trong lần hoàn thiện này, AI đối chiếu feedback thực tế do tôi cung cấp qua synthesis để cập nhật note cá nhân và README.

**Output cần chỉnh:** Note và README cũ ghi feedback mô phỏng, lựa chọn C và đề xuất chỉ đổi nhãn độ chắc; các điểm này không khớp kết quả thực tế. Mô tả thiếu bản A/B và C đồng chẩn đoán hai giả thuyết cũng không khớp bản build hiện có. Bản cập nhật giữ nguyên lời tester, điểm đánh giá và lựa chọn phân vân A/B; phân biệt evidence, diễn giải và hướng sửa chưa triển khai.

**Phần tôi cung cấp:** Bản synthesis đã tổng hợp ý kiến sau ba phiên là nguồn cho kết quả test. AI không bổ sung danh tính tester, thời lượng từng lượt, thao tác cứu hộ hoặc kết quả quiz khi nguồn chưa ghi. Dữ liệu mẫu và phản hồi AI trong HTML không được dùng làm evidence hành vi người thật.

## Năm gate — đối chiếu hồ sơ hiện tại

| Gate | Evidence hiện có | Trạng thái và giới hạn |
|---|---|---|
| **1. Evidence Continuity** | Hypothesis nối Practice Notes 1/2, có Note 3 phản biện và Still Unknown | Có dấu vết evidence; chưa validation toàn bộ problem |
| **2. Meaningful Options** | A dẫn dắt, B đối thoại do user điều phối, C xử lý ngầm và duyệt/ngoại lệ | Ba cơ chế khác nhau, có build A/B/C trong repo |
| **3. Human Control** | A chấp nhận/đổi/từ chối; B đổi góc độ và sửa ghi chú; C duyệt/báo ngoại lệ | Có điểm kiểm soát; feedback C 2–3/5 cho thấy agency vẫn cần cải thiện |
| **4. Test-ready** | Có common context, bản A/B/C và synthesis từ ba phiên ngoài nhóm | Đã có bản dùng để test theo hồ sơ nhóm; chưa xác nhận link public hoặc QA trình duyệt trong lần cập nhật tài liệu này |
| **5. Learning** | Synthesis có pattern/khác biệt, trade-off, một Next Change và Still Unproven; note cá nhân đã cập nhật | Đã có learning từ test; hai note thành viên khác còn cần đồng bộ, hướng mới chưa test lại |

## Kiểm tra trước khi nộp

- [x] README ghi đúng Day 19, MHV/họ tên, Option C và sáu phần nội dung.
- [x] Có file A/B/C và đường mở common context/bộ trải nghiệm tester.
- [x] Synthesis ghi nhận đủ ba tester độc lập ngoài nhóm.
- [x] Note cá nhân và README khớp điểm Control/Help, lựa chọn phân vân A/B và trade-off thực tế.
- [x] Chốt một hướng thay đổi từ evidence, ghi rõ Still Unproven và trạng thái chưa triển khai.
- [x] Hai thành viên còn lại cập nhật note thực tế trong `prototype-feedback-note.md`.
- [x] Đồng bộ Prototype Link và AI Support Log với bản build hiện tại.
- [x] Kiểm quyền truy cập repo/link bàn giao từ tài khoản giảng viên/TA.
