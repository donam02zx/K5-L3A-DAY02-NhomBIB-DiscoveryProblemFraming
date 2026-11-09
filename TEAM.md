# Team

> Bản chung của nhóm. Mỗi thành viên tự xác nhận phần việc và điền đóng góp thực tế của mình.

## Thông tin nhóm

- Tên nhóm: BIB
- Candidate problem nhóm chọn (1 câu): Khi chuẩn bị bài tiếng Anh, giáo viên muốn tìm, đối chiếu và chọn tài liệu bổ sung phù hợp với mục tiêu và trình độ lớp để hoàn thiện bài giảng.
- Quyết định cuối (Go / Not Yet / No-Go): **Not Yet**.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Đỗ Phương Nam | 2A202603621 | Điều phối và tổng hợp Problem Statement | donam02zx |
| 2 | Hồ Anh Dũng | 2A202603613 | Vẽ quy trình trước/sau | ITCSIU21172 |
| 3 | Hồ Đức Mạnh | 2A202603609 | Rà soát nguồn tham khảo và hỗ trợ ghi chép | hoducmanhtemperature |
| 4 | Ngô Huy Hoàng | 2A202603622 | Phản biện và đối chiếu mức can thiệp | HuyHoangg10 |
| 5 | Phạm Thị Hồng Ngọc | 2A202603602 | Kiểm chứng nhu cầu giáo viên | [Tự điền] |
| 6 | Trương Hoàng Tùng | 2A202603651 | Rà soát rủi ro và quyết định | Dobit25 |

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Đỗ Phương Nam | Ngô Huy Hoàng | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Phạm Thị Hồng Ngọc | Trương Hoàng Tùng | Assumption map, snapshot hoặc survey |
| CP4 — Research | Hồ Đức Mạnh | Hồ Anh Dũng | Bảng research có link |
| CP5 — Quy trình trước/sau | Hồ Anh Dũng | Hồ Đức Mạnh | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Đỗ Phương Nam | Phạm Thị Hồng Ngọc | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Ngô Huy Hoàng | Đỗ Phương Nam | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Trương Hoàng Tùng | Phạm Thị Hồng Ngọc | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

### DoPhuongNam-2A202603621

**Phần việc phụ trách:**

- Điều phối nhóm và tổng hợp Problem Statement.
- CP3 — Hội tụ nhóm (người chính): cluster, cây OST, bảng chấm điểm.
- CP5 — Problem Statement v0 (người chính).
- CP6 — Mức can thiệp + Problem Statement v1 (hỗ trợ).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Pitch 2 candidate: khoanh vùng bug kế toán PM_KT (#7) và tổng hợp, nhận xét bài tập MindX (#8). Candidate bug vào shortlist với 28 điểm; nhóm loại vì cần quyền truy cập code, log và dữ liệu nghiệp vụ không có trong buổi lab.
- Đặt câu hỏi phản biện cho pitch #2 (thế nào là câu hỏi "trùng lặp") và pitch #10 (học viên không tìm thấy hay không biết cách tìm).
- Tổng hợp cluster, cây OST và bảng chấm điểm shortlist ở CP3.
- Soạn Problem Statement v0 và hỗ trợ bảng thay đổi v0 → v1.
- Chuẩn bị kịch bản và slide thuyết trình của nhóm.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`, mục 2.1: pitch #7, #8 và câu hỏi phản biện cho #2, #10.
- `report/team/group_report.md`, mục 2.2–2.4: cluster, cây OST, chấm điểm shortlist.
- `report/team/group_report.md`, mục 5: Problem Statement v0.
- `report/individual/2A202603621_DoPhuongNam.md`, mục 2–4: CP1, CP2 và phần tham gia nhóm.
- về phần commit do có 1 file làm chung nên 1 bạn đại diện làm nên file group_report.md không có commit


**Điều mình học được từ phần nhóm:**

- Problem có tần suất và impact cao chưa chắc là candidate tốt nhất cho nhóm: card bug PM_KT của em có số liệu rõ nhưng bị loại vì nhóm không có quyền truy cập code, log và dữ liệu để kiểm chứng trong buổi lab.
- Phản biện "thử chuẩn hoá log và liên kết ticket trước khi dùng AI" giúp mình thấy phải loại trừ phương án No AI / Rule trước, thay vì mặc định AI là lời giải.
- Số tự ước lượng phải được ghi rõ là ước lượng; khi viết Problem Statement, phần khó nhất là đặt metric đo được khi baseline mới chỉ là self-report.

### HoAnhDung-2A202603613

**Phần việc phụ trách:**
- Lên ý tưởng (Pitch) bài toán nghiệp vụ góc nhìn Business Analyst.
- Phản biện, rà soát bẫy "Solution-first" (giải pháp đi trước vấn đề) của nhóm.
- Chuẩn hóa và tối ưu hóa luồng quy trình nghiệp vụ (As-Is / To-Be).
- Phân tích rủi ro kinh doanh (Viability) và tinh chỉnh các chỉ số đo lường (Success Metrics, Before/After).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Giai đoạn Pitch & OST: Đóng góp 2 Problem Cards (#5, #6) về nỗi đau tổng hợp thông tin/điều phối task của BA, làm cơ sở hình thành Cluster B. Đặt câu hỏi phản biện giúp team nhận ra nhiều bài toán chỉ cần sửa Quy ước (Rule) thay vì dùng AI.
- Giai đoạn Research (CP4): Chỉ ra cho nhóm thấy Giả định #2 và #3 chính là LoFA (Leap of Faith Assumption - Giả định rủi ro nhất) cần ưu tiên đi phỏng vấn xác thực.
- Giai đoạn Quy trình (CP5): Đề xuất chẻ nhỏ Bottleneck 20 phút ở luồng As-Is thành 2 thao tác (Skimming và Deep Reading) để thấy rõ nỗi đau. Bổ sung "Bước 0: Setup Knowledge Base" (chi phí ẩn) và luồng ngoại lệ (Unhappy path) vào quy trình To-Be.
- Giai đoạn Đánh giá & Quyết định (CP6): Đưa góc nhìn BA vào bảng 4.3 (Trước/Sau) bằng cách bổ sung chỉ số Cognitive Load (Tải trọng nhận thức)và Context Switching (Chuyển đổi ngữ cảnh). Bổ sung rủi ro Willingness to pay (Sự sẵn sàng chi trả) vào mục Viability, củng cố vững chắc cho quyết định "Not Yet".

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 2.1: Candidate #5, #6 và các câu hỏi phản biện trực tiếp Đỗ Phương Nam, Ngô Huy Hoàng.
- Mục 3.1 & 8.1: Các đánh giá về rủi ro Viability và xác định LoFA (thời gian setup, khả năng chi trả của giáo viên).
- Mục 4.1 & 4.2: Bản nháp quy trình đã được phân tách bước nghẽn và làm rõ các thao tác kiểm duyệt của con người (Human-in-the-loop).
- Mục 4.3 & 5: Bảng so sánh Before/After và Success Metrics có chứa các chỉ số về chất lượng (Tỷ lệ chấp nhận tài liệu) và rủi ro thời gian setup.

**Điều mình học được từ phần nhóm:**
- Không vội "say đắm" giải pháp (Solution-first): Em nhận ra team làm Tech rất dễ sa đà vào việc nghĩ tính năng (AI chấm tự luận, app riêng) trước khi hiểu thấu đáo nỗi đau. Vai trò của BA là phải liên tục "kéo" team về lại thực tế bằng cách hỏi: "Người dùng có thực sự cần không? Quy trình tay hiện tại đã tối ưu chưa?".
- Cẩn thận với "Chi phí ẩn" của AI: Một quy trình AI trông có vẻ giảm thời gian (từ 40 phút xuống 22 phút) nhưng lại sinh ra chi phí chuẩn bị dữ liệu (KB setup, upload, tag). Nếu công setup lớn hơn thời gian tiết kiệm được, dự án sẽ thất bại.
- Góc nhìn đa chiều khi đánh giá: Em học được cách không chỉ đo lường bằng số bước, số phút, mà còn phải đánh giá sự "mệt mỏi não bộ" (Cognitive load) của người dùng và tính khả thi về mặt kinh doanh (Willingness to pay). Quyết định "Not Yet" của nhóm không phải là thất bại, mà là một bước lùi dũng cảm, tỉnh táo để tránh lãng phí nguồn lực khi bằng chứng (Evidence) chưa đủ.
### HoDucManh-2A202603609

**Phần việc phụ trách:**

- CP4 — Research: rà soát đường dẫn và ghi nguồn tham khảo.
- Hỗ trợ CP5: kiểm tra cách trình bày và thời gian trong bảng trước/sau.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Hỗ trợ đối chiếu nguồn về NotebookLM/Gemini Notebook, Diffit và MagicSchool; ghi rõ chức năng công bố chưa phải kết quả thử nghiệm của nhóm.
- Chuyển lại phản hồi giáo viên về sự khác biệt với general agent, giúp bổ sung tín hiệu phản bác trong phần kiểm chứng.
- Góp ý phân biệt self-report 20 phút với tổng 40 phút mô phỏng, đồng thời tính cả công kiểm tra và chuẩn bị tài liệu khi so sánh trước/sau.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo nhóm](report/team/group_report.md): mục 3.2–3.3 ghi phản hồi và research; mục 4.3 đối chiếu thời gian và trạng thái số liệu.
- [Báo cáo cá nhân](report/individual/2A202603609_HoDucManh.md): mục 4 ghi nội dung đóng góp và phản biện.

**Điều mình học được từ phần nhóm:**

- Có phân luồng theo level hoặc thêm KB chưa đủ chứng minh khác biệt với công cụ sẵn có. Cần so cùng tác vụ và tính cả thời gian chuẩn bị, kiểm tra, sửa đầu ra trước khi quyết định xây thêm.

### NgoHuyHoang-2A202603622

**Phần việc phụ trách:**

- Phụ trách chính CP6: đối chiếu mức can thiệp No AI / Rule / Workflow / Agent và hỗ trợ hoàn thiện Problem Statement v1.
- Hỗ trợ CP3: pitch, phản biện và hội tụ các candidate problem của nhóm.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Pitch và phản biện hai vấn đề: PM phải liên tục hỏi tiến độ và học viên khó tìm lại câu hỏi/câu trả lời cũ.
- Cùng nhóm gom cluster, dựng cây OST, chấm điểm và chọn shortlist.
- So sánh các mức can thiệp, bổ sung AI Canvas, PAIR và tiêu chí đánh giá cho candidate được chọn.
- Đề xuất chưa đi thẳng lên Agent khi quy trình còn có thể định nghĩa trước và bằng chứng người dùng chưa đủ; ưu tiên Workflow có human review để kiểm chứng trước.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md`: mục 2.1–2.4 (pitch, phản biện và hội tụ nhóm).
- `group_report.md`: mục 6.2–6.4 (so sánh mức can thiệp, AI Canvas và PAIR).
- `group_report.md`: mục 7 (Problem Statement v1 và tiêu chí đánh giá).

**Điều mình học được từ phần nhóm:**

- Em hiểu rõ hơn sự khác nhau giữa Workflow và Agent: nếu các bước và quy tắc đã xác định được thì chưa cần Agent.
- Trước khi chọn giải pháp AI cần so sánh với phương án không AI, Rule và Workflow, đồng thời giữ con người ở bước quyết định quan trọng.
- Khi bằng chứng kiểm chứng chưa đủ, quyết định hợp lý là bàn luận thêm thay vì cố chốt giải pháp sớm.

### PhamThiHongNgoc-2A202603602

**Phần việc phụ trách:**

- [Thành viên tự điền]

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- [Thành viên tự điền]

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Thành viên tự điền]

**Điều mình học được từ phần nhóm:**

- [Thành viên tự điền]

### TruongHoangTung-2A202603651

**Phần việc phụ trách:**

- Đề xuất và pitch candidate về rào cản onboarding của người mới chơi game đối kháng.
- Phản biện candidate được nhóm chọn để tránh solution-first.
- Hỗ trợ research giải pháp có sẵn và so sánh No AI / Rule / Workflow / Agent.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Chuẩn bị Problem Card về việc người mới chơi game đối kháng không chuyển được trận thua lặp lại thành một hành động luyện tập cụ thể.
- Đặt câu hỏi phản biện về việc bổ sung AI chấm bài tự luận; từ phản biện này, nhóm nhận ra đây là một feature khác, không giải quyết trực tiếp bottleneck tìm, đối chiếu và chọn tài liệu.
- Góp phần phân biệt opportunity với solution trong cây OST: chatbot, AI Agent, AI chấm tự luận và nền tảng học tập là solution, không phải pain của người dùng.
- Research MagicSchool, Diffit, Azota/K12Online và phương án thư viện nguồn đã duyệt + checklist.
- Góp ý hướng can thiệp: Rule lọc nguồn đã duyệt trước; chỉ cân nhắc Workflow AI để tóm tắt/so sánh nguồn có citation; không chọn Agent.
- Góp ý boundary: AI không tự tìm nguồn ngoài whitelist, không bịa claim, không tự quyết định tài liệu dùng cho học sinh; giáo viên kiểm nguồn và quyết định cuối.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/individual/2A202603651_TruongHoangTung.md`, mục 2–3: CP1, CP2, Problem Card game đối kháng và bảng phản biện AI.
- `report/team/group_report.md`, mục 2.1: câu hỏi phản biện về AI chấm bài tự luận.
- `report/team/group_report.md`, mục 2.3: phần loại các solution đội lốt opportunity.
- `report/team/group_report.md`, mục 2.4: candidate game đối kháng trong shortlist và lý do không được chọn.
- `report/team/group_report.md`, mục 3.3: research MagicSchool, Diffit và baseline thư viện nguồn + checklist.
- `report/team/group_report.md`, mục 4.2–4.3: boundary, Rule/Workflow, human-in-the-loop và phương án quay về.
- Commit: `[điền mã commit thật sau khi commit phần đóng góp của tôi]`.

**Điều mình học được từ phần nhóm:**

- Một idea có vẻ nhiều tiềm năng AI không tự động là candidate tốt; evidence, actor, quy trình và khả năng đo impact quan trọng hơn.
- Candidate problem phải mô tả pain và bottleneck trước, không bắt đầu bằng feature như chatbot, AI Agent hay AI chấm bài.
- Công cụ có sẵn như MagicSchool, Diffit, Azota và K12Online khiến nhóm phải kiểm chứng gap thực tế thay vì mặc định xây sản phẩm mới.
- Không phải workflow nào có nhiều thông tin cũng cần Agent; với bài toán của nhóm, Rule và human review cần được chứng minh không đủ trước khi chọn Workflow.
