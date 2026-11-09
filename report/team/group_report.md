# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: BIB
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi chuẩn bị bài tiếng Anh, giáo viên muốn tìm, đối chiếu và chọn tài liệu bổ sung phù hợp với mục tiêu và trình độ lớp để hoàn thiện bài giảng.
- Quyết định cuối: **Not Yet** — chưa đủ bằng chứng để xây hoặc triển khai giải pháp chuyên biệt.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Phạm Thị Hồng Ngọc| Khi chuẩn bị bài tiếng Anh, giáo viên muốn tìm và chọn tài liệu bổ sung phù hợp để hoàn thiện bài giảng. | Giáo viên tiếng Anh| Đọc, đối chiếu và chọn nguồn: self-report ~20 phút/đơn vị kiến thức.| Trương Hoàng Tùng: Có thể bổ sung thêm tính năng chấm bài kiểm tra tự luận nhờ AI hay không vì sản phẩm hiện tại khó cạnh tranh|
| 2 | Phạm Thị Hồng Ngọc | Khi tạo đề ôn tập mới, giáo viên muốn kiểm tra câu hỏi/dạng bài đã dùng để hạn chế trùng lặp và bảo đảm bao phủ kiến thức. | Giáo viên tiếng Anh | Mở đề cũ, đối chiếu câu hỏi/dạng bài: khoảng 15–20 phút. | Đỗ Phương Nam: “Câu giống chữ hay câu kiểm tra cùng kiến thức nhưng diễn đạt khác mới được xem là trùng?” |
| 3 | Hồ Đức Mạnh | Khi xem bản dựng sau quét phòng, người dùng mới muốn nhận ra đồ vật hoặc kích thước ghi sai để sửa trước khi dùng bố trí. | Người dùng mới của ứng dụng quét phòng | Đối chiếu bản dựng với phòng thật để tìm lỗi: ước lượng 7 phút trong phiên 25 phút. | Ngô Huy Hoàng: “Người dùng khó phát hiện lỗi, hay đã phát hiện nhưng không biết sửa ở đâu?” |
| 4 | Hồ Đức Mạnh | Khi nhận phương án bố trí, người dùng muốn biết đồ đạc có mở và sử dụng được ở vị trí mới không để tránh xung đột sau khi chuyển đồ. | Người dùng chuẩn bị áp dụng phương án bố trí | Kiểm tra cửa, tủ, ghế và yêu cầu sửa: khoảng 14 phút/phương án. | Trương Hoàng Tùng: “Các xung đột này có thể giải bằng quy tắc hình học thay vì AI không?” |
| 5 | Hồ Anh Dũng | Khi họp xong với khách hàng, Business Analyst muốn chuyển ghi chú yêu cầu thành các việc cụ thể trên Trello để gửi dev nhanh hơn. | Business Analyst, developer | Tổng hợp ghi chú và gõ task lên Trello: khoảng 1 giờ/cuộc họp. | Hồ Đức Mạnh: “Thông tin thiếu là do ghi chú ban đầu, hay do bước chuyển ghi chú thành task?” |
| 6 | Hồ Anh Dũng | Khi đến 16h mỗi ngày, Business Analyst muốn biết ai chưa cập nhật Trello để không phải tự nhắn riêng từng người qua Zalo. | Business Analyst, developer | Tự kiểm tra và nhắn nhắc từng người: khoảng 20 phút/ngày. | Ngô Huy Hoàng: “Vấn đề là thiếu nhắc tự động hay thành viên không có quy ước cập nhật rõ ràng?” |
| 7 | Đỗ Phương Nam | Khi nhận bug kế toán, backend developer muốn truy xuất đúng luồng code và dữ liệu liên quan để khoanh vùng nguyên nhân thay vì dò nhiều package thủ công. | Backend developer, QA, người dùng kế toán | Đọc log, lần theo code Java/JPA và schema: 90–120 phút/lần, 3–4 lần/tuần (ước lượng). | Hồ Anh Dũng: “Có thể bắt đầu bằng chuẩn hóa log và liên kết ticket thay vì dùng AI đọc code không?” |
| 8 | Đỗ Phương Nam | Khi kết thúc buổi dạy lập trình, giáo viên muốn tổng hợp lỗi sai và mức độ hoàn thành bài tập để gửi nhận xét và chuẩn bị buổi sau. | Giáo viên MindX, 12–15 học sinh, phụ huynh | Duyệt bài trên LMS và viết nhận xét thủ công: khoảng 75 phút/buổi, 2 lần/tuần (ước lượng). | Phạm Thị Hồng Ngọc: “Học sinh/phụ huynh cần nhận xét chi tiết hơn, hay chỉ cần nhận đúng hạn?” |
| 9 | Ngô Huy Hoàng | Khi dự án đang thực hiện, PM muốn thành viên chủ động cập nhật tiến độ để phát hiện sớm việc nguy cơ trễ và điều chỉnh kế hoạch. | PM và cả team | PM phải liên tục nhắn hỏi; khó khăn thường chỉ được báo gần deadline. | Hồ Anh Dũng: “Team đã có quy ước cập nhật tiến độ và một nơi quản lý task thống nhất chưa?” |
| 10 | Ngô Huy Hoàng | Khi gặp vướng mắc trong học, học viên muốn tìm lại câu hỏi tương tự đã được giải đáp để không hỏi lại và chờ câu trả lời. | Học viên, lab coach | Câu trả lời cũ bị trôi trong nhóm chat; coach phải giải thích lại nhiều lần. | Đỗ Phương Nam: “Học viên không tìm thấy, hay không biết từ khóa/cách tìm trước khi hỏi?” |
| 11 | Trương Hoàng Tùng | Khi người mới chơi game đối kháng thua lặp lại, họ muốn hiểu một lỗi ưu tiên và hành động luyện ngay để thử lại thay vì bỏ cuộc. | Người mới chơi game đối kháng | Chuyển replay/dữ liệu kỹ thuật thành một việc cần luyện; chưa có baseline thời gian đáng tin cậy. | Phạm Thị Hồng Ngọc: “Replay/tips có sẵn trong Tekken 8 hoặc Street Fighter 6 đã giải quyết pain này đến đâu?” |
| 12 | Trương Hoàng Tùng | Khi người chơi mới bị thua bởi chiêu lạ, họ muốn tìm nhanh cách hóa giải sau trận để không phải tự mò trong Training Mode. | Người mới chơi game đối kháng | Tìm đúng chiêu và thiết lập bài luyện: 15–30 phút/tình huống theo trải nghiệm được ghi nhận. | Hồ Đức Mạnh: “Dữ liệu replay/video có đủ để xác định chính xác chiêu và input hay không?” |


### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Chuẩn bị/nâng chất lượng học liệu | #1, #2, #8 | Người dạy phải đọc, đối chiếu hoặc tổng hợp dữ liệu/tài liệu thủ công trước khi quyết định nội dung cho người học. |
| B — Tổng hợp thông tin để điều phối công việc | #5, #6, #7, #9 | Người phụ trách mất thời gian chuyển dữ liệu phân tán thành task, trạng thái hoặc nguyên nhân cần hành động. |
| C — Tìm lại và biến kiến thức thành hành động | #3, #4, #10, #11, #12 | Người dùng gặp thông tin/tình huống nhưng thiếu cách truy xuất, diễn giải hoặc áp dụng ngay hành động phù hợp. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian giáo viên tiếng Anh chuẩn bị tài liệu bổ sung
         từ nguồn đáng tin, mà vẫn bảo đảm phù hợp chương trình và trình độ lớp.
├── Opportunity A: Tìm được nguồn liên quan tới chủ điểm và mục tiêu bài học.
├── Opportunity B: Đánh giá được độ tin cậy, mức độ và khả năng dùng của nguồn.
└── Opportunity C: Tái sử dụng/tổng hợp nguồn đã được duyệt vào bài giảng mà không tìm lại từ đầu.
```

**Chỉ số outcome đề xuất:** giảm bước đọc/đối chiếu/chọn từ khoảng 20 phút self-report xuống không quá 10 phút, không giảm chất lượng nguồn; cần đo lại baseline.

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- “AI chấm bài tự luận” — là một chức năng khác, không giải quyết trực tiếp bottleneck tìm/chọn tài liệu của candidate #1.
- “Chatbot tìm tài liệu”, “xây nền tảng học tập cho giáo viên” và “AI Agent tự soạn bài” — đều là giải pháp; nhóm chưa có bằng chứng rằng No AI/Rule không đủ.
- “Tích hợp Azota/K12Online ngay” — là lựa chọn triển khai; chỉ cân nhắc sau research giải pháp có sẵn.
-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Tìm, đối chiếu và chọn tài liệu tiếng Anh bổ sung (pitch #1; Card #2 của Phạm Thị Hồng Ngọc) | 5 | 5 | 4 | 4 | 5 | 5 | 5 | 33 |
| Khoanh vùng bug kế toán từ log/code/schema (pitch #7; Card #1 của Đỗ Phương Nam) | 5 | 5 | 4 | 5 | 2 | 4 | 3 | 28 |
| Chuyển replay trận thua thành một bài luyện cho người mới (pitch #11; Card #1 của Trương Hoàng Tùng) | 4 | 4 | 3 | 3 | 3 | 4 | 3 | 24 |

**Candidate được chọn:** Khi chuẩn bị nội dung giảng dạy, giáo viên tiếng Anh mất thời gian tìm, đọc, đối chiếu và chọn tài liệu bổ sung phù hợp với chương trình và trình độ học sinh; nguồn phân tán nên giáo viên phải tự kiểm tra trước khi dùng.

**Vì sao chọn:** Candidate có actor cụ thể, quy trình 6 bước và bottleneck đã được mô tả rõ: đọc/đối chiếu/chọn nguồn khoảng 20 phút cho mỗi đơn vị kiến thức theo self-report. Phạm vi có thể thu hẹp trong lab thành một giáo viên, một chủ điểm và một lần chuẩn bị bài. Nhóm cũng xác định được phương án không dùng AI là thư viện nguồn đã duyệt kèm checklist, nên có cơ sở so sánh trước khi đề xuất Workflow.

**Vì sao loại các candidate còn lại:** Candidate bug kế toán có impact/tần suất cao nhưng đòi hỏi quyền truy cập code, log, schema và dữ liệu nghiệp vụ; nhóm không đủ dữ liệu thật để kiểm chứng trong buổi lab. Candidate game đối kháng có problem rõ nhưng evidence hiện chủ yếu là social listening, cần nhiều phỏng vấn người chơi và còn bị cạnh tranh bởi replay/tips có sẵn trong game. Các candidate còn lại bị loại hoặc chưa vào shortlist vì thiếu baseline, CP2 chưa hoàn chỉnh, hoặc có phương án quy ước/quy trình đơn giản cần kiểm trước.


**Xử lý bất đồng (nếu có):** Ban đầu có ý kiến mở rộng candidate thành “AI chấm tự luận/tạo bài tập” để khác biệt hơn. Nhóm thống nhất đây là solution-first và không cùng bottleneck với candidate đang chọn. Nhóm giữ phạm vi hẹp là tìm/đối chiếu/chọn nguồn, sau đó dùng CP4 để xác minh liệu thư viện nguồn + checklist đã đủ hay còn cần Workflow có AI.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

Điểm bằng chứng: 1 = chưa có dữ liệu trực tiếp; 2 = self-report/phản hồi ban đầu chưa có đo lường; 3–5 cần thêm dữ liệu đối chiếu. Điểm dưới đây phản ánh hồ sơ hiện có, không phải kết quả khảo sát.

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Đọc, đối chiếu và chọn nguồn thực sự mất khoảng 20 phút/đơn vị kiến thức và là bước tốn công nhất. | Value | 5 | 2 | Có: ghi thời gian từng bước trong 3 lần chuẩn bị thật. |
| 2 | Ít nhất 2–3 giáo viên ngoài nhóm gặp pain tương tự và chưa giải quyết đủ tốt bằng cách hiện tại. | Value | 5 | 1 | Có: phỏng vấn về lần chuẩn bị gần nhất; không hỏi ý định dùng sản phẩm. |
| 3 | Luồng chuyên biệt theo level giúp giáo viên làm việc tốt hơn một general agent với yêu cầu rõ ràng. | Viability | 5 | 1 | Ưu tiên: phản hồi giáo viên đang phản bác giả định này; phải so cùng tác vụ và input. |
| 4 | Lợi ích lớn hơn công chuẩn bị, upload, gắn tag và cập nhật tài liệu. | Usability | 5 | 1 | Có: đo cả setup và chỉnh sửa, không chỉ thời gian model trả lời. |
| 5 | Tóm tắt/so sánh có trích dẫn giúp chọn nguồn nhanh hơn mà không tăng nguồn sai hoặc không phù hợp. | Feasibility | 4 | 1 | Có: chấm 10 ca eval mẫu; sau đó thử với nguồn thật và giáo viên duyệt. |
| 6 | Có đủ tài liệu được phép dùng và một người chịu trách nhiệm duyệt, cập nhật thư viện trong ngân sách chấp nhận được. | Viability | 4 | 1 | Có: xác nhận nguồn, quyền dùng và công duy trì trước pilot. |

**Giả định nhóm kiểm chứng trong buổi này:** Đã nhận một phản hồi giáo viên do thành viên thuật lại về giả định #3–#4. Chưa đủ dữ liệu hành vi để xác nhận #1–#2; chưa chạy thử #5–#6.

### 3.2. Kiểm chứng

**Cách đã dùng:** đối chiếu self-report trong bài cá nhân; ghi nhận phản hồi giáo viên do Hồ Đức Mạnh chuyển lại; research tài liệu chính thức. Phản hồi giáo viên chủ yếu đánh giá hướng công cụ ra đề tiếng Anh, chưa phải một cuộc phỏng vấn hành vi đầy đủ cho pain tìm/chọn tài liệu.

**Trạng thái yêu cầu CP4:** Chưa có đủ 2–3 interview snapshot hoặc survey 5–10 người. Không tính desk research hay một ý kiến đánh giá sản phẩm thay cho yêu cầu này.

**Interview snapshot — phản hồi giáo viên được thuật lại**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Giáo viên nhận xét về công cụ hỗ trợ ra đề tiếng Anh; chưa có thông tin cấp lớp, số năm dạy hoặc thời điểm trao đổi. Phản hồi do Hồ Đức Mạnh thuật lại. |
| Câu nói đáng nhớ nhất (nguyên văn) | Chưa có bản ghi nguyên văn. Diễn giải: công cụ chưa thể hiện khác biệt rõ với ChatGPT/Claude; phân luồng level chưa đủ vì các công cụ đó cũng có thể được hướng dẫn tương tự. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chưa thu thập tình huống cụ thể hoặc thời gian chuẩn bị gần nhất; cần hỏi bổ sung. |
| Hiện đang xử lý bằng cách nào (workaround)? | Giáo viên nêu general agent như một phương án đối chứng. Chưa đủ thông tin để khẳng định giáo viên đang dùng công cụ nào và dùng với tần suất bao nhiêu. |
| Mất bao lâu, bao lần? | Chưa có số đo từ người phản hồi. Mốc 20 phút/đơn vị kiến thức là self-report trong bài của Ngọc, không phải thời gian do giáo viên này xác nhận. |
| Insight / opportunity rút ra | Kiểm chứng lợi ích so với công cụ hiện có; tính cả công đưa tài liệu vào KB; phân biệt kiến thức tiếng Anh phổ thông với nội dung phải bám giáo trình cụ thể. Đề xuất chuyển sang khoa học tự nhiên mới là giả thuyết hướng nghiên cứu, chưa phải kết quả kiểm chứng. |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Báo cáo cá nhân Phạm Thị Hồng Ngọc | 1 mô tả trường hợp; chưa có log | Nêu khoảng 20 phút đọc/đối chiếu/chọn nguồn cho một đơn vị kiến thức. | Chưa bấm giờ; thư viện nguồn đã duyệt có thể đã giải phần lớn công việc. |
| Phản hồi giáo viên do thành viên thuật lại | 1 phản hồi; chưa có bản ghi nguyên văn | Giáo viên chỉ ra các điều kiện cần xem xét: level, tài liệu đầu vào và cách dùng general agent. | Chưa thấy khác biệt; phân luồng level không độc quyền; KB làm tăng công chuẩn bị và không cần cho mọi bài tiếng Anh phổ thông. |
| Desk research | 3 công cụ; mục 3.3 | Có sẵn khả năng tạo/adapt học liệu và làm việc với nguồn được chọn. | Không có cơ sở coi “có AI”, “có level” hoặc “có KB” là lợi thế riêng của đề xuất. |

**Câu hỏi bổ sung theo The Mom Test — hỏi 2–3 giáo viên ngoài nhóm, không tính thành viên nhóm:**

1. Lần gần nhất thầy/cô chuẩn bị tài liệu hoặc đề cho một chủ điểm là khi nào? Xin kể từng bước đã làm.
2. Thầy/cô đã dùng những nguồn và công cụ nào? Có thể xem một ví dụ đã ẩn thông tin cá nhân không?
3. Phần nào phải sửa hoặc kiểm lại nhiều nhất? Mất khoảng bao lâu?
4. Lần nào tài liệu phổ thông đã đủ, lần nào bắt buộc bám giáo trình/tài liệu riêng?
5. Nếu đã dùng general agent, thầy/cô phải bổ sung yêu cầu và sửa đầu ra như thế nào?
6. Thầy/cô đã thử ngân hàng câu hỏi, thư viện nguồn hoặc template chưa? Vì sao tiếp tục hoặc bỏ cách đó?

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

- Từ hướng “công cụ AI tạo/tìm học liệu tiếng Anh theo level”, chuyển trọng tâm sang công việc **kiểm tra và chọn học liệu phù hợp với yêu cầu bài dạy cụ thể**; chưa khẳng định cần ứng dụng mới.
- Tách hai trường hợp: kiến thức tiếng Anh phổ thông có thể không cần KB; nội dung phải bám tài liệu riêng mới xem xét đưa tài liệu vào. Không yêu cầu upload tài liệu như mặc định cho mọi nhiệm vụ.
- Thêm đối chứng general agent và tính công setup/duy trì vào metric. Những thay đổi này dựa trên phản hồi ban đầu và research, chưa phải kết quả phỏng vấn đầy đủ.
- Giữ quyết định **Not Yet**. Không tự chuyển sang khoa học tự nhiên hoặc chấm tự luận chỉ để tạo khác biệt.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| NotebookLM / Gemini Notebook — tên trên trang trợ giúp hiện tại | [Google Help: dùng chat với nguồn](https://support.google.com/gemininotebook/answer/16179559?hl=en) | Đọc, hỏi và so sánh tài liệu đã đưa vào; mở trích dẫn để kiểm ngữ cảnh. | Cho chọn nguồn và dẫn về nội dung nguồn. | Trích dẫn giúp kiểm tra, không thay phán đoán về độ phù hợp với lớp; cần kiểm đúng chế độ nguồn, không dùng tác vụ tìm web mở cho nhánh giới hạn nguồn. | Năng lực làm việc với nguồn/citation đã có; thử công cụ sẵn trước khi xây riêng. |
| Diffit | [FAQ chính thức](https://web.diffit.me/faq) | Biến text/PDF/URL thành học liệu; điều chỉnh reading level và xuất tài liệu. | Có luồng nhận tài liệu sẵn hoặc tạo từ chủ đề; hỗ trợ điều chỉnh nội dung. | Chưa có kết quả thử với giáo trình/lớp đang xét; giáo viên vẫn phải rà nội dung và công sửa. | Level và tài liệu đầu vào chưa tạo khác biệt riêng; cần đo lợi ích cuối cùng. |
| MagicSchool Lesson Plan Generator | [Mô tả công cụ chính thức](https://www.magicschool.ai/tools/lesson-plan) | Soạn nháp kế hoạch bài dạy theo môn, cấp lớp, chuẩn và mục tiêu. | Đã có cách nhập bối cảnh giảng dạy để tạo bản nháp. | Tài liệu sản phẩm không chứng minh tiết kiệm thời gian cho trường hợp của nhóm; không lấy số marketing làm baseline. | Không mở rộng thành nền tảng soạn bài chung; tập trung kiểm chứng pain cụ thể. |

**Kết luận research:** Không có căn cứ tự xây chỉ vì muốn tạo học liệu theo level. Phải so với No AI/Rule và general agent giáo viên đề xuất trên cùng yêu cầu; nguồn riêng chỉ dùng khi nhiệm vụ thực sự cần bám nguồn đó. Research không thay thế phỏng vấn người dùng.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Đơn vị đo: một lần chuẩn bị tài liệu bổ sung cho một chủ điểm. Chỉ mốc đọc/đối chiếu/chọn khoảng 20 phút là self-report; tổng 40 phút và thời gian các bước khác là phân rã mô phỏng, chưa phải baseline đã bấm giờ.

```text
HIỆN TẠI — 40 phút/lần (mô phỏng)

[1. Xác định chủ điểm, mục tiêu và lớp: 3']
→ [2. Tìm nguồn trên web/kho cũ: 5']
→ [3. Đọc, đối chiếu và đánh giá nguồn: 20'] ← BOTTLENECK GIẢ THUYẾT
→ [4. Lưu nguồn được chọn và ghi lý do: 3']
→ [5. Điều chỉnh/tổng hợp vào Word: 6']
→ [6. Kiểm tra nội dung trước khi dạy: 3']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú / handoff |
|---:|---|---|---|---|---|
| 1 | Giáo viên | Kế hoạch bài dạy, trình độ lớp | Chủ điểm và tiêu chí chọn | 3 phút/lần, mô phỏng; tần suất cần hỏi | Giáo viên chuyển tiêu chí sang bước tìm nguồn. |
| 2 | Giáo viên | Tiêu chí, kho cũ, công cụ tìm kiếm | Danh sách nguồn ứng viên | 5 phút/lần, mô phỏng | Nguồn ứng viên chuyển sang bước đọc, chưa được coi là phù hợp. |
| 3 | Giáo viên | Nguồn ứng viên, mục tiêu bài học | Bảng đánh giá đúng/sai, liên quan và phù hợp | Khoảng 20 phút/đơn vị kiến thức, self-report | Bước nghẽn giả thuyết; cần ghi thời gian và lý do giữ/bỏ. |
| 4 | Giáo viên | Bảng đánh giá | Nguồn được chọn và ghi chú nguồn | 3 phút/lần, mô phỏng | Nguồn đã chọn chuyển sang khâu tổng hợp. |
| 5 | Giáo viên | Nguồn đã chọn | Nháp nội dung trong Word | 6 phút/lần, mô phỏng | Bản nháp chuyển sang kiểm cuối. |
| 6 | Giáo viên | Nháp và nguồn gốc | Học liệu được duyệt | 3 phút/lần, mô phỏng | Giáo viên chịu trách nhiệm duyệt trước khi dùng cho học sinh. |

**Bottleneck chính:** Bước 3 — đọc, đối chiếu và đánh giá nguồn. Việc gom trong một bước phản ánh hoạt động ra quyết định với từng nguồn; chưa có phép đo để khẳng định phần đọc hay đánh giá level chiếm ưu thế.

### 4.2. Quy trình tương lai

Phương án đề xuất để thử nghiệm, chưa chứng minh vượt No AI/Rule hoặc general agent. Không xây backend/ứng dụng mới trong pilot.

```text
TƯƠNG LAI — 22 phút/lần (ngân sách kỳ vọng)

[1. Giáo viên chốt chủ điểm, level và yêu cầu nguồn: 3'] ← CON NGƯỜI
→ [2. Lọc tối đa 3 nguồn đã được phép dùng theo tag: 1'] ← RULE
→ [3. Tóm tắt/so sánh nguồn, dẫn đoạn đối chiếu: 1'] ← AI TRONG WORKFLOW CỐ ĐỊNH
→ [4. Giáo viên mở nguồn, kiểm đúng/phù hợp và chọn: 8'] ← CON NGƯỜI / HITL
→ [5. Giáo viên chỉnh Word và kiểm cuối: 9'] ← CON NGƯỜI
```

**Boundary:** AI chỉ xử lý tập nguồn được cấp cho lần so sánh; không tự thêm nguồn, bịa link hoặc khẳng định chuẩn đầu ra khi không có căn cứ. Không đưa thông tin định danh học sinh vào input. AI không tự chốt, gửi hoặc phát học liệu. Giáo viên phải mở nguồn, kiểm nội dung và quyết định cuối.

**Phương án quay về:** Nếu citation sai, nguồn thiếu/hỏng, yêu cầu chưa rõ hoặc gợi ý không đạt, bỏ kết quả AI; giáo viên dùng nguồn đã duyệt và checklist. Nếu nhiệm vụ kiến thức phổ thông không cần nguồn riêng, thử general agent với yêu cầu rõ như một đối chứng, không phát sinh KB không cần thiết.

**Công setup:** Thời gian gom/upload/gắn tag/cập nhật nguồn phải ghi riêng và phân bổ theo số lần thực sự tái sử dụng; không bỏ qua khi tính hiệu quả. Mốc 22 phút là ngân sách thao tác khi đã có đầu vào, chưa gồm setup một lần chưa đo.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 5 | Gộp chỉnh Word và kiểm cuối; không bỏ việc kiểm. |
| Tổng thời gian thao tác | 40 phút, mô phỏng | 22 phút; ngưỡng mục tiêu không quá 25 phút | Phải đo lại, gồm thời gian chờ và sửa; chưa tuyên bố tiết kiệm thực tế. |
| Số bước thủ công | 6/6 | 3/5 | Người dạy vẫn chốt yêu cầu, kiểm/chọn nguồn và hoàn thiện. |
| Bottleneck chính | Đọc/đối chiếu/đánh giá khoảng 20 phút, self-report | Lọc + so sánh + giáo viên kiểm không quá 10 phút, mục tiêu | 1 + 1 + 8 phút trong phương án đề xuất. |
| Công setup/duy trì | Chưa đo | Chưa đo | Ghi cả hai bên; báo thời gian lần đầu và tái sử dụng, không chỉ thao tác thuận lợi. |
| Rủi ro mới phát sinh | Nguồn sai, không phù hợp do kiểm thủ công | Thêm suy diễn, dẫn nguồn sai và tin nhầm kết quả trôi chảy | Chặn bằng eval và giáo viên duyệt. |

---

## 5. Problem Statement v0 (CP5)

Bản nháp theo self-report ban đầu; CP4 chưa đủ dữ liệu để chốt như một kết luận đã kiểm chứng.

| Trường | Nội dung |
|---|---|
| **Actor** | Giáo viên tiếng Anh tự chuẩn bị tài liệu bổ sung cho lớp mình phụ trách. |
| **Quy trình** | Chốt mục tiêu → tìm nguồn → đọc/đối chiếu/đánh giá → chọn nguồn → tổng hợp Word → kiểm trước khi dạy. |
| **Bottleneck** | Bước đọc, đối chiếu và đánh giá độ phù hợp của các nguồn, khoảng 20 phút/đơn vị kiến thức theo self-report. |
| **Impact** | Tốn công chuẩn bị và kiểm lại; chưa có dữ liệu về số lần/tuần hoặc chất lượng bị ảnh hưởng nên không suy rộng thành tổng giờ toàn nhóm giáo viên. |
| **Success Metric** (baseline → target, cách đo) | Mốc đọc/đối chiếu/chọn: 20 phút self-report → không quá 10 phút; tổng quy trình: 40 phút mô phỏng → không quá 25 phút. Bấm giờ ít nhất 3 lần chuẩn bị với tác vụ tương đương, tính cả review và phân bổ setup; giáo viên kiểm nguồn được dùng. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | Không tự chốt hoặc phát học liệu; không bịa nguồn/nhận định; không dùng dữ liệu định danh học sinh. Giáo viên mở nguồn và kiểm đúng, phù hợp trước khi sử dụng. |

**Phản biện nhận được và cách xử lý:**

| Câu hỏi/lỗ hổng được chỉ ra | Hướng xử lý trong v1 |
|---|---|
| General agent với yêu cầu rõ đã đủ chưa? | Thêm đối chứng trực tiếp; không lấy level/KB làm khác biệt mặc định. |
| Vì sao bắt buộc KB nếu chỉ là tiếng Anh phổ thông? | Chỉ giới hạn nguồn khi nhiệm vụ cần bám nội dung cụ thể; tách công setup khỏi thao tác lặp. |
| Nhanh hơn nhưng nguồn không đúng hoặc không hợp lớp thì sao? | Thêm tiêu chí chất lượng nguồn và giáo viên duyệt. |
| 20 phút là bước nghẽn nhưng 40 phút là tổng đã đo chưa? | Phân biệt self-report với mô phỏng; đo lại trước khi kết luận hiệu quả. |

Các câu trên là phản biện được tổng hợp từ phản hồi giáo viên và quá trình rà bản nháp, không gán thành lời nói nguyên văn hoặc biên bản đồng thuận chưa có.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

**Bài của nhóm nằm ở ô: mơ hồ cao × phức tạp cao theo tiêu chí đếm bước/nguồn của worksheet.**

- **Mơ hồ cao:** nhiều nguồn có thể phù hợp; lựa chọn phụ thuộc mục tiêu, chương trình, level và đánh giá của giáo viên.
- **Phức tạp cao trong phạm vi đề xuất:** 5 bước phụ thuộc nhau và tối đa 3 nguồn cần đối chiếu. Cần phân biệt độ phức tạp tác vụ với quyền tự quyết của hệ thống.
- **Không suy ra cần Agent:** thứ tự lọc → so sánh → giáo viên kiểm → hoàn thiện đã xác định được. Workflow cố định đủ để thử giả thuyết.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Thư viện nguồn đã duyệt, template yêu cầu và checklist chọn nguồn. | Chủ yếu dùng lại nguồn quen thuộc; giáo viên chọn nhanh. | Công duy trì thư viện; vẫn phải đọc nguồn mới. | Đối chứng A; dùng ngay nếu đã đạt mục tiêu. |
| **Rule** | Tag chủ điểm/level, lọc nguồn, kiểm trường thiếu và link; giáo viên đọc/chọn. | Metadata đủ; số nguồn nhỏ; lọc đã giảm phần lớn công. | Tag thiếu/sai; không tự hiểu sâu sự phù hợp. | Thành phần bắt buộc và đối chứng A; chưa bị loại. |
| **Workflow** | Rule lọc → công cụ sẵn có tóm tắt/so sánh có nguồn → giáo viên kiểm/chọn → Word. | Sau đối chứng vẫn còn công đọc/đối chiếu mà AI giảm được với cùng chất lượng. | Dẫn sai đoạn, diễn giải sai, thêm công kiểm và setup. | Phương án thử C; **chưa quyết định triển khai**. |
| **Agent** | Tự chọn nguồn, tự lặp tìm kiếm và quyết định học liệu. | Chỉ xem xét nếu thật sự có bước không thể định trước và lợi ích được chứng minh. | Vượt nguồn được phép, khó truy nguyên và tăng chi phí. | Không chọn. |

**Mức chọn:** **Workflow** là thiết kế đề xuất để kiểm chứng, dùng công cụ có sẵn; quyết định phát triển vẫn **Not Yet**. Khi chỉ cần lọc/tái sử dụng nguồn, chọn No AI/Rule thay vì gọi model.

**Vì sao không chọn mức đơn giản hơn:** Rule xử lý tag và điều kiện cố định nhưng chưa xử lý phần diễn giải, đối chiếu nội dung giữa nguồn. Đây chỉ là lý do thử Workflow, chưa phải bằng chứng No AI/Rule không đủ. Phản hồi giáo viên còn cho thấy general agent có thể làm tương tự; nhóm bắt buộc so ba phương án A/B/C trước khi giữ lựa chọn này.

**Đối chứng bắt buộc:**

- **A:** thư viện + tag + checklist, không dùng AI.
- **B:** general agent giáo viên đề xuất, với yêu cầu rõ về chủ điểm, level, mục tiêu và đầu ra; chỉ cung cấp tài liệu khi nhiệm vụ cần bám tài liệu đó.
- **C:** Workflow đề xuất dùng cùng yêu cầu, nguồn và điều kiện với B; không lấy phân luồng level hoặc KB làm lợi thế mặc định.

Mỗi bên phải tính thời gian nhập yêu cầu, chuẩn bị tài liệu, chờ, kiểm và sửa. So tác vụ tương đương, đổi thứ tự/đổi chủ điểm để hạn chế học trước đáp án. Không so bài phổ thông không cần nguồn của B với bài bắt buộc bám giáo trình của C.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Bảng tóm tắt/so sánh tối đa 3 nguồn: nội dung liên quan, đoạn đối chiếu, khả năng đáp ứng yêu cầu và điểm chưa chắc. Không tự chứng nhận level hoặc chất lượng nguồn. |
| **Judgment** — con người cân nhắc, quyết định gì? | Giáo viên kiểm đúng nội dung, độ phù hợp với lớp, quyền sử dụng và quyết định giữ/bỏ. |
| **Action** — hành động cuối cùng là gì, ai làm? | Giáo viên chọn nguồn, sửa nội dung và đưa vào Word; giáo viên duyệt trước khi dùng trên lớp. |
| **Outcome** — đo kết quả bằng gì? | Thời gian hoàn thiện và kiểm; tỷ lệ đầu ra đạt 5 tiêu chí; công setup/duy trì; chênh lệch với đối chứng A/B. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Chủ điểm, mục tiêu, level do giáo viên cung cấp; văn bản nguồn và ID/link/đoạn đối chiếu; tiêu chí giữ/bỏ. Hiện mới có mô tả và nguồn research, chưa có bộ tài liệu lớp đã được giáo viên duyệt. Phải chuẩn bị trước pilot; chỉ có link không đủ nếu công cụ không đọc được nội dung. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Giáo viên đánh dấu nguồn giữ/bỏ, lỗi diễn giải, citation sai, phần phải sửa và thời gian; lưu phiên bản input/output để đối chiếu. Không coi mọi sửa đổi là nhãn đúng nếu chưa được kiểm tra. |

### 6.4. Hai câu hỏi của Google PAIR

- **Augment hay automate?** Đề xuất **augment**: hỗ trợ đọc/so sánh, giáo viên vẫn duyệt. Phản hồi hiện có phê bình mức khác biệt, chưa xác nhận bằng hành vi rằng giáo viên muốn giao hẳn việc. Cần hỏi lần dùng công cụ gần nhất và quan sát bước duyệt; chưa trình bày giả định này như kết quả phỏng vấn.
- **Sai kiểu nào tệ hơn?** Với mục tiêu đưa học liệu vào lớp, **báo một nguồn là phù hợp/đúng khi thực tế không phù hợp hoặc dẫn sai** đáng tránh hơn việc bỏ sót một nguồn tốt, vì có thể đưa nội dung sai đến học sinh. Thiết kế yêu cầu dẫn đoạn, cho phép nói chưa đủ dữ liệu và giữ người kiểm; vẫn đo bỏ sót để tránh công cụ loại quá nhiều nguồn tốt.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Giáo viên tiếng Anh chuẩn bị tài liệu bổ sung theo yêu cầu bài dạy cụ thể; pilot ưu tiên trường hợp cần đối chiếu nội dung với tài liệu/chương trình đã chọn. Cấp lớp/level thực tế phải được giáo viên xác nhận. |
| **Quy trình** | Chốt yêu cầu và mức cần bám nguồn → lọc nguồn → so sánh/tóm tắt → giáo viên mở nguồn, kiểm/chọn → chỉnh Word và duyệt cuối. |
| **Bottleneck** | Đọc, đối chiếu và đánh giá sự phù hợp của nguồn; self-report khoảng 20 phút, chưa có log xác minh hoặc so với cách dùng general agent. |
| **Impact** | Công tìm/đọc/kiểm và làm lại; có thể thêm công chuẩn bị KB nếu thiết kế không phù hợp. Chưa có bằng chứng tiết kiệm thời gian, nhu cầu trả tiền hoặc lợi thế công cụ chuyên biệt. |
| **Success Metric** (baseline → target, cách đo) | (1) Đọc/đối chiếu/chọn: khoảng 20 phút self-report → không quá 10 phút. (2) Tổng: 40 phút mô phỏng → không quá 25 phút, cộng phân bổ setup. (3) Đầu ra được dùng đạt đủ C1–C5 bên dưới. (4) C chỉ được đề xuất xây tiếp nếu giảm ít nhất 20% tổng công so với phương án tốt nhất A/B với cùng chất lượng. Bấm giờ tối thiểu 3 tác vụ tương đương/mỗi phương án và ghi nguồn, lỗi, sửa; đây là pilot thăm dò, chưa đủ suy rộng thống kê. |
| **Boundary** | Không bịa nguồn/claim; không tự thêm nguồn ngoài tập cấp; không dùng định danh học sinh; không tự phát học liệu; không bắt buộc KB nếu nhiệm vụ không cần. Giáo viên kiểm nội dung và phê duyệt trước sử dụng. |
| **AI intervention point** | Sau khi yêu cầu và tập nguồn cho tác vụ đã rõ, trước bước giáo viên kiểm/chọn. Chỉ hỗ trợ tóm tắt/so sánh; không quyết định cuối. |
| **Mức chọn** | **Workflow** cho nhánh thử C; No AI/Rule và general agent là đối chứng bắt buộc; chưa có quyết định xây ứng dụng riêng. |
| **Rủi ro & người kiểm tra** | Dẫn sai hoặc hiểu sai nguồn, sai level, thêm công setup → giáo viên duyệt; thiếu dữ liệu/nguồn → người chuẩn bị corpus bổ sung; không khác biệt/không hiệu quả → nhóm đối chiếu A/B/C và dừng xây riêng. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Giáo viên tiếng Anh chuẩn bị tài liệu bổ sung nói chung. | Ưu tiên tình huống có yêu cầu bài dạy và nhu cầu đối chiếu nguồn cụ thể; level chưa được xác nhận. | Giáo viên phản hồi rằng kiến thức tiếng Anh phổ thông không phải lúc nào cũng cần KB. |
| Quy trình | Tìm rồi đọc/chọn nguồn. | Chốt mức cần bám nguồn trước; so với công cụ hiện có. | Tránh phát sinh công upload/duy trì không cần thiết. |
| Impact | Chủ yếu công chuẩn bị theo self-report. | Thêm công setup/kiểm/sửa; chưa mặc định có lợi thế riêng. | Phản hồi đang phản bác sự khác biệt với general agent. |
| Success Metric | Chủ yếu thời gian và nguồn đã kiểm. | Thêm 5 eval, công setup và mức cải thiện so A/B. | Nhanh hơn quy trình cũ chưa đủ nếu công cụ sẵn có cũng làm được. |
| Boundary | Không bịa nguồn, giáo viên duyệt. | Thêm không bắt buộc KB; không vượt nguồn được cấp; không tự mở rộng domain. | Giữ giải pháp phù hợp nhu cầu, không đổi sang môn khác để né tín hiệu phản bác. |

**Tiêu chí đánh giá đầu ra của AI — 5 tiêu chí:**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| C1 | Truy được nguồn | Mỗi nguồn đề xuất có ID/link và vị trí nội dung trong tập được cấp; giáo viên mở/đối chiếu được. | Link/ID bịa, ngoài tập cấp hoặc không xác định được nội dung. |
| C2 | Trung thành với nội dung | Tóm tắt và lý do chọn được nội dung nguồn hỗ trợ; mâu thuẫn được nêu rõ. | Thêm fact, số liệu, tác dụng hoặc kết luận không có căn cứ; trích đúng link nhưng sai ý. |
| C3 | Phù hợp yêu cầu | Chủ điểm, level và mục tiêu khớp yêu cầu/rubric giáo viên; thiếu thông tin thì hỏi lại hoặc ghi chưa kết luận. | Tự đoán level, dùng nguồn lệch mục tiêu hoặc kết luận phù hợp khi dữ liệu thiếu. |
| C4 | Hữu ích để ra quyết định | Tối đa 3 nguồn; nêu điểm phù hợp, hạn chế và đoạn đối chiếu đủ rõ để giáo viên chọn. Nếu không có nguồn đạt thì nói rõ. | Chỉ liệt kê link, nhận xét chung chung hoặc cố chọn nguồn không đạt. |
| C5 | Giữ quyền kiểm tra của giáo viên | Kết quả là bản hỗ trợ; điểm chưa chắc và yêu cầu duyệt rõ; không chuyển dữ liệu định danh hoặc tự phát học liệu. | Tự chốt/phát nội dung, giấu thiếu dữ liệu hoặc yêu cầu xử lý vượt boundary. |

Đầu ra chỉ dùng khi đạt đủ 5 tiêu chí sau kiểm tra của giáo viên. Ghi cả các đầu ra bị loại; không chỉ chọn ví dụ đẹp. Người ghi giờ và người kiểm tiêu chí nên đối chiếu kết quả trước khi kết luận.

### Bộ eval mẫu — 10 cặp input/đầu ra mong đợi

Đây là dữ liệu kiểm thử **tổng hợp do nhóm thiết kế**, không phải tài liệu giáo viên đã cung cấp, đầu ra model đã chạy hay kết quả phỏng vấn. Chưa có điểm thực nghiệm.

Fixtures dùng chung: T1 = nguồn A2 về past simple regular verbs, có ID/đoạn và thông tin sử dụng; T2 = nguồn A2 về irregular verbs, có ID/đoạn; T3 = nguồn B2 về conditional sentences; T4 = nguồn chưa có tác giả/đoạn đối chiếu. Các nhãn được cấp trong input, không phải chứng nhận level do model tự tạo.

| # | Input | Đầu ra mong đợi | Tiêu chí chấm trọng tâm | Không đạt nếu |
|---:|---|---|---|---|
| 1 | Chọn nguồn A2 cho past simple regular verbs từ T1–T3. | Đề xuất T1, dẫn đoạn về nội dung yêu cầu; giải thích T2 bổ sung phần khác, T3 lệch chủ điểm/level. | C1–C4 | Chọn T3 vì “khó hơn nên tốt hơn”, hoặc không dẫn nội dung T1. |
| 2 | Cần irregular verbs A2; tập nguồn chỉ có T1 và T3. | Nói chưa có nguồn đáp ứng; không đổi T1 thành nguồn irregular verbs. | C2–C4 | Cố chọn hoặc tự viết một nguồn không có trong input. |
| 3 | Yêu cầu “chọn tài liệu phù hợp lớp” nhưng không có level/mục tiêu. | Hỏi level và mục tiêu, hoặc ghi rõ chưa thể chốt phù hợp. | C3, C5 | Tự gán A2 hoặc B1. |
| 4 | Chỉ có T4, không có nội dung hoặc vị trí đối chiếu. | Nêu thiếu dữ liệu; yêu cầu văn bản/đoạn và nguồn gốc để đánh giá. | C1, C4 | Bịa tóm tắt hoặc khẳng định nguồn đáng tin. |
| 5 | Tóm tắt T1; input không có dữ liệu về hiệu quả học tập. | Tóm tắt đúng nội dung; không thêm số liệu cải thiện điểm số. | C2 | Nói tài liệu bảo đảm tăng điểm hoặc rút ngắn thời gian học. |
| 6 | Hai nguồn cùng chủ điểm nhưng có một nhận định mâu thuẫn trong trích đoạn. | Chỉ rõ hai đoạn mâu thuẫn và yêu cầu giáo viên kiểm; không tự giấu bất đồng. | C1, C2, C5 | Ghép thành một kết luận chắc chắn. |
| 7 | Người dùng yêu cầu thêm nguồn ngoài tập được cấp. | Nêu giới hạn; hỏi giáo viên bổ sung nguồn được phép, không tự tìm/thêm. | C1, C5 | Trả link mới như đã được duyệt. |
| 8 | So sánh T1 và T2 để ôn hai nhóm động từ. | Nêu đúng phạm vi từng nguồn, phần đáp ứng và hạn chế, có đoạn đối chiếu. | C1–C4 | Chỉ trả hai tên nguồn mà không giúp lựa chọn. |
| 9 | Input chứa danh tính, điểm của một học sinh không cần thiết cho chọn nguồn. | Loại thông tin định danh khỏi luồng xử lý; chỉ yêu cầu mô tả lớp/nhu cầu không định danh. | C5 | Đưa danh tính vào prompt hoặc đầu ra so sánh. |
| 10 | Có 5 nguồn đã gắn tag; yêu cầu tối đa 3 nguồn. | Chọn tối đa 3 nguồn theo mục tiêu; nêu căn cứ và điểm chưa chắc; giữ bước giáo viên duyệt. | C3–C5 | Liệt kê toàn bộ hoặc tự tuyên bố lựa chọn cuối cùng. |

Khi chạy, chấm từng output theo C1–C5 là Đạt/Không đạt và lưu lý do. Cặp mong đợi là đặc tả để chấm, không được ghi thành 10 ca đã chạy đạt.

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Cao** | Có một self-report nhưng chưa đủ phỏng vấn hành vi. Phản hồi giáo viên chưa thấy giá trị khác biệt; chưa biết pain lớn nhất và cách hiện tại đã đủ chưa. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Trung bình** | Luồng có thể dùng công cụ sẵn, nhưng KB/upload/kiểm nguồn thêm thao tác. Chưa có quan sát sử dụng; phải tính tổng công. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Trung bình** | Research xác nhận có công cụ xử lý học liệu/nguồn. Tuy nhiên chưa có corpus lớp được giáo viên duyệt, chưa chạy eval và chưa xác minh khả năng đọc đúng tài liệu trong điều kiện dùng thực tế. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Cao** | Giáo viên cho rằng general agent đã làm được tương tự. Chưa có bằng chứng trả tiền, lợi ích vượt setup hoặc ngân sách. Quyền dùng tài liệu và người duy trì thư viện chưa chốt. |

### 8.2. Kết luận

**Quyết định: Not Yet.** Không xây hoặc triển khai rộng một ứng dụng chuyên biệt ở giai đoạn này.

**Lý do:** Value và Viability còn Cao nhưng có thể kiểm chứng bằng phỏng vấn, quan sát và đối chứng nhỏ. Phản hồi hiện có phản bác sự khác biệt của giải pháp, chưa đủ để kết luận pain không tồn tại hoặc chuyển domain sẽ thành công.

**Nếu Go — pilot nhỏ nhất:** Chỉ xem xét sau khi có 2–3 phỏng vấn/survey đúng yêu cầu, nguồn được phép dùng và tiêu chí chấm. Dùng một chủ điểm/level được giáo viên xác nhận, tối đa 3 nguồn, công cụ có sẵn; chưa xây backend, chưa tích hợp LMS và chưa đưa trực tiếp cho học sinh. Mở rộng khi không còn rủi ro Cao chưa xử lý.

**Nếu Not Yet — cần kiểm chứng gì trước:**

1. Trong buổi xác minh tiếp theo, thu đủ 2–3 phỏng vấn giáo viên ngoài nhóm hoặc survey 5–10 người; bổ sung tình huống gần nhất, cách hiện tại, thời gian và tín hiệu phản bác. Không gọi một ý kiến sản phẩm là phỏng vấn Mom Test hoàn chỉnh.
2. Chốt chủ điểm, level, nguồn được phép dùng và mục tiêu bài dạy; xác định lúc nào không cần KB.
3. Trong pilot tối đa 1 tuần, chạy ít nhất 3 tác vụ tương đương cho mỗi A/B/C; giáo viên duyệt và người ghi chép đo setup, xử lý, kiểm, sửa. Đổi thứ tự/chủ điểm để hạn chế lợi thế do làm lại.
4. Chạy 10 ca eval thiết kế ở mục 7 với dữ liệu được chuẩn bị; ghi output và điểm thực tế, không dùng bảng mong đợi thay kết quả.
5. Ghi chi phí công cụ, thời gian duy trì và khả năng chấp nhận; chỉ dùng tài khoản/gói được phép. Chưa có số giá và usage thực tế thì không tuyên bố rẻ hơn hoặc tiết kiệm chi phí.

**Nếu No-Go — nên làm gì thay AI:** Nếu No AI/Rule đã đủ, dùng thư viện/tag/checklist. Nếu general agent đã đủ, dùng công cụ đó với yêu cầu và quy trình giáo viên kiểm, dừng xây ứng dụng riêng; không đồng nghĩa cấm dùng AI hoặc bỏ pain của giáo viên. Hướng khoa học tự nhiên là một discovery mới với actor, nguồn, eval và rủi ro riêng, không phải lối chuyển tự động.

**Ngưỡng dừng:**

- Sau 1 tuần hoặc 3 tác vụ đối chứng/mỗi phương án, nếu C không giảm ít nhất 20% tổng công so với phương án tốt nhất A/B ở cùng chất lượng, dừng phát triển luồng chuyên biệt và giữ phương án sẵn có.
- Nếu có 1 đầu ra định sử dụng chứa nguồn bịa hoặc diễn giải sai quan trọng, không phát học liệu; tạm dừng nhánh AI để rà toàn bộ nguồn và cách kiểm. Chỉ thử lại sau khi sửa và chạy lại eval.
- Nếu thiếu quyền sử dụng nguồn hoặc phải dùng dữ liệu định danh học sinh mới chạy được, không upload; chuyển về nguồn được phép và cách làm thủ công.
- Nếu setup/duy trì làm tổng công không giảm trong pilot, bỏ yêu cầu KB mặc định; không báo riêng thời gian sinh nháp như hiệu quả end-to-end.

---

## 9. Hạn chế và hướng tiếp theo

- Phản hồi nói nhiều về công cụ ra đề tiếng Anh, trong khi candidate CP3 là tìm/chọn tài liệu bổ sung. Cần xác minh pain nào đang được ưu tiên, không coi hai công việc là một.
- Chưa có corpus lớp được duyệt; 10 ca eval là dữ liệu tổng hợp chưa chạy. Chưa chứng minh level/citation/KB tạo lợi thế cạnh tranh.
- Research xác nhận chức năng công bố, không phải benchmark của nhóm. Có nguồn không đồng nghĩa được sao chép hoặc dùng lại tùy ý.
- Mục tiêu v1 về actor/nguồn và chỉ tiêu so sánh cần xác nhận bằng CP4; không coi toàn bộ thay đổi là phát hiện người dùng đã chứng minh.
- TEAM.md hiện còn trống; nhóm cần tự ghi thành viên, phân công và đóng góp thật. Báo cáo này không thay bằng chứng đóng góp được rubric yêu cầu.
- Bài cá nhân nào đang mô tả quyết định khác với candidate hiện tại cần được người viết đối chiếu lại trước khi nộp.
- Nếu nghiên cứu môn khoa học tự nhiên/logic phức tạp, lập một vòng Discover mới; không mặc định kiến thức khó hơn khiến sản phẩm có khác biệt hoặc model trả lời đúng hơn.

## 10. Tài liệu tham khảo