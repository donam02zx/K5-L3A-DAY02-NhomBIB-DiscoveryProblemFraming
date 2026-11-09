# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: BIB
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi chuẩn bị bài tiếng Anh, giáo viên muốn tìm và chọn tài liệu bổ sung phù hợp để hoàn thiện bài giảng. | Giáo viên tiếng Anh | Đọc, đối chiếu và chọn nguồn: self-report ~20 phút/đơn vị kiến thức. 
- Quyết định cuối: Go / Not Yet / No-Go: Not Yet

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

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Giáo viên thực sự mất khoảng 20 phút/đơn vị kiến thức ở bước đọc/đối chiếu/chọn nguồn.| Value| 5| 2| Có: Thống kê những lần soạn đề trước đó|
| 2 | Giáo viên khác Huyền cũng gặp pain này, không chỉ là thói quen cá nhân.| Value| 5| 1| Có: Phỏng vấn 2–3 giáo viên khác |
| 3 | Kiểm chứng độ phù hợp của tài liệu, không chỉ là tìm link.| Usability| 5| 1| Có: Các nguồn cuối có phù hợp với năng lực của nhóm học sinh được hướng tới không|
| 4 | AI có thể gợi ý tài liệu có dẫn nguồn mà không bịa hoặc sai trình độ.| Feasibility| 4| 1| Chấm thử 3–5 truy vấn bằng rubric nguồn/phù hợp, có giáo viên duyệt.|

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Rà soát self-report trong Problem Card #2 của Phạm Thị Hồng Ngọc và research desk về công cụ hiện có. 

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Từ “AI tìm kiếm và tổng hợp tài liệu cho giáo viên” thu hẹp thành “giáo viên cần giảm thời gian đọc, đối chiếu và chọn nguồn **có thể kiểm chứng** theo chủ điểm/trình độ”. Tạm thời không kết luận AI cần thiết; CP4 chính thức phải phỏng vấn thêm 2–3 giáo viên và ghi cả trường hợp thư viện nguồn/checklist hoặc công cụ có sẵn đã đủ.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| MagicSchool AI | https://www.magicschool.ai/ | Hỗ trợ tạo lesson plan, assessment, differentiation và tài liệu lớp học. | Có nhiều công cụ cho giáo viên, giúp soạn nháp nhanh. | Chưa có bằng chứng công khai rằng công cụ chỉ làm việc trong whitelist nguồn của Huyền hoặc luôn giải thích độ phù hợp theo giáo trình/lớp. | Không cạnh tranh bằng thông điệp chung “AI tạo lesson plan”; cần kiểm chứng pain về nguồn đã duyệt/citation. |
| Diffit | https://app.diffit.me/ | Tạo và điều chỉnh study guide, bài tập, hoạt động theo nhiều mức. | Mạnh ở biến đổi/tạo học liệu phù hợp nhiều mức độ. | Chưa chứng minh được giải quyết bước xác minh nguồn gốc, bản quyền và độ phù hợp với chương trình cụ thể. | Tách rõ “tạo/adapt học liệu” khỏi “tìm và kiểm nguồn”. |
| Thư viện nguồn đã duyệt + checklist (No AI/Rule) | `[CẦN KIỂM chứng bằng Word/Drive hiện có của giáo viên]` | Lọc/tái sử dụng nguồn theo chủ điểm; giáo viên kiểm bằng checklist trước khi đưa vào Word. | Dễ triển khai, không bịa nguồn, giữ người dạy quyết định cuối. | Chưa biết thư viện có đủ nguồn mới hay có giảm thời gian xuống target hay không. | Đây là baseline bắt buộc; chỉ lên Workflow nếu Rule/checklist không đủ. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
[1 Xác định chủ điểm + mục tiêu bài học: ~3']
→ [2 Tìm nguồn trên web/kho cũ: ~5']
→ [3 Đọc và đối chiếu nguồn: ~12']
→ [4 Chọn/loại theo chương trình + trình độ: ~8'] ← BOTTLENECK GỘP (bước 3+4: ~20')
→ [5 Điều chỉnh/tổng hợp vào Word: ~7']
→ [6 Giáo viên tự kiểm trước khi dạy: ~5']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Giáo viên tiếng Anh | Kế hoạch bài dạy, lớp, chủ điểm | Mục tiêu/từ khóa tìm nguồn | ~3 phút/lần chuẩn bị — **mô phỏng, cần đo** | Xác định phần kiến thức cần bổ sung. |
| 2 | Giáo viên tiếng Anh | Từ khóa, Word/Drive cũ, công cụ tìm kiếm | Danh sách link/tài liệu ứng viên | ~5 phút/lần — **mô phỏng, cần đo** | Nguồn có thể đến từ Internet hoặc học liệu đã lưu. |
| 3 | Giáo viên tiếng Anh | Nhiều nguồn ứng viên | Nhận định sơ bộ về tính đúng/chất lượng | ~12 phút/lần — **phân rã mô phỏng** | Cùng bước 4 tạo thành self-report ~20 phút/đơn vị kiến thức. |
| 4 | Giáo viên tiếng Anh | Nguồn đã đọc, chương trình, trình độ lớp | Nguồn được chọn/bỏ | ~8 phút/lần — **phân rã mô phỏng** | **Bottleneck chính:** đối chiếu và ra quyết định; cần ghi tiêu chí giữ/bỏ qua phỏng vấn. |
| 5 | Giáo viên tiếng Anh | Nguồn được chọn | Nội dung/bài tập được tổng hợp vào Word | ~7 phút/lần — **mô phỏng, cần đo** | Có thể phát sinh việc điều chỉnh độ khó/ngôn ngữ. |
| 6 | Giáo viên tiếng Anh | Bản nháp Word | Nội dung sẵn sàng dùng trên lớp | ~5 phút/lần — **mô phỏng, cần đo** | Giáo viên chịu trách nhiệm chuyên môn cuối cùng. |

**Bottleneck chính:** Đọc, đối chiếu và chọn nguồn theo chương trình/trình độ (bước 3–4). Mốc ~20 phút là self-report trong Problem Card #2; tổng ~40 phút trong sơ đồ là mô phỏng để nhóm kiểm tra

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
[1 Giáo viên nhập chủ điểm, mục tiêu, lớp: ~3' — CON NGƯỜI]
→ [2 Lọc thư viện nguồn đã duyệt theo tag: ~1' — RULE]
→ [3 Tóm tắt/so sánh tối đa 3 nguồn, luôn kèm link: ~1' — AI WORKFLOW]
→ [4 Giáo viên mở link, kiểm và chọn/bỏ: ~8' — CON NGƯỜI / HITL]
→ [5 Điều chỉnh/tổng hợp vào Word + kiểm cuối: ~9' — CON NGƯỜI]
```

**Boundary:** AI chỉ tóm tắt/so sánh nguồn từ whitelist đã được giáo viên duyệt; phải hiển thị link; không tự tìm web ngoài whitelist, không tự tạo claim không có trong nguồn, không tự chọn hoặc gửi nội dung cho học sinh.

**Phương án quay về:** Nếu link hỏng, nguồn ngoài whitelist, thông tin sai hoặc giáo viên không chấp nhận gợi ý, bỏ hoàn toàn kết quả AI; giáo viên dùng thư viện nguồn đã duyệt + checklist 4 tiêu chí (nguồn/tác giả truy được, đúng chủ điểm, phù hợp trình độ, quyền sử dụng/tham khảo rõ ràng).

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 | 5 | Quy trình sau gộp “điều chỉnh” và “kiểm cuối” vào một bước có người chịu trách nhiệm. |
| Tổng thời gian | ~40 phút/lần — **mô phỏng, chưa đo** | ~22 phút/lần — **kỳ vọng, cần pilot** | Chỉ mốc bước 3–4 ~20 phút có self-report; cần bấm giờ ít nhất 3 lần trước/sau. |
| Số bước thủ công | 6/6 | 3/5 | Bước 2 là Rule, bước 3 là AI; giáo viên vẫn nhập yêu cầu, kiểm/chọn và hoàn thiện. |
| Bottleneck chính | Đọc + đối chiếu + chọn nguồn: ~20 phút self-report | Giáo viên kiểm nguồn/gợi ý: ~8 phút kỳ vọng | Giảm thời gian không được làm mất bước kiểm chuyên môn. |
| Rủi ro mới phát sinh | — | AI dẫn sai/thiếu link; tóm tắt sai; nguồn đúng nhưng không phù hợp lớp | Xử lý bằng whitelist, citation bắt buộc, HITL và phương án quay về. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Giáo viên tiếng Anh tự chuẩn bị tài liệu bổ sung cho lớp `[cấp/lớp cần chốt]`. |
| **Quy trình** | Xác định chủ điểm → tìm nguồn → đọc/đối chiếu → chọn/loại → điều chỉnh vào Word → tự kiểm trước khi dạy. |
| **Bottleneck** | Đọc, đối chiếu và xác minh nhiều nguồn trước khi quyết định nguồn nào phù hợp với chương trình và trình độ. |
| **Impact** | Self-report ban đầu là ~20 phút/đơn vị kiến thức; cần xác minh tác động lên chất lượng và khả năng tái sử dụng. |
| **Success Metric** | `[baseline đã bấm giờ]` → `[target]`, đo trong 3 lần chuẩn bị; đồng thời 100% nội dung được dùng phải có nguồn giáo viên đã kiểm. |
| **Boundary** | Không tự tạo fact không có nguồn; không tự chốt tài liệu; không dùng dữ liệu định danh học sinh; giáo viên kiểm tra trước khi dạy. |

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:
- **Mơ hồ** cao
- **Phức tạp** thấp

Vì sao:
- **Mơ hồ:** cao — có nhiều tài liệu chấp nhận được, “phù hợp” phụ thuộc lớp, mục tiêu và phán đoán của giáo viên.
- **Phức tạp:** thấp–trung bình — các bước cố định, nhưng có nhiều nguồn và cần kiểm chứng.
- **Hệ quả:** Không chọn Agent. Nếu có AI, chỉ là Workflow hẹp ở bước tóm tắt/so sánh nguồn, trước bước giáo viên quyết định.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** | Thư viện Drive/Word được tag + checklist 4 tiêu chí. | Giáo viên chủ yếu dùng lại nguồn cũ. | Vẫn phải đọc nhiều nguồn mới. | Baseline bắt buộc. |
| **Rule** | Lọc whitelist theo chủ điểm/lớp; cảnh báo thiếu nguồn/tag. | Nguồn đã có tag ổn định. | Không đánh giá được ý nghĩa/phù hợp sâu. | Có thể đủ. |
| **Workflow** | Rule lọc → AI tóm tắt/so sánh có citation → giáo viên duyệt. | Xác nhận đọc/đối chiếu vẫn là bottleneck sau Rule. | AI dẫn sai link, bỏ sót nguồn tốt, suy diễn cấp độ. | Chỉ chọn có điều kiện. |
| **Agent** | AI tự tìm web, tự chọn nguồn, tự tạo/dạy nội dung. | Không có lý do đủ mạnh. | Sai nguồn, khó kiểm soát, vượt boundary. | Không chọn. |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
