## 1. Thông tin học viên

- **Họ tên:** Đỗ Phương Nam
- **MSSV:** 2A202603621
- **Email trường** (không bắt buộc, repo có thể để public):
- **Tên nhóm:** NhomBIB
- **Link repo nhóm:** https://github.com/donam02zx/K5-L3A-DAY02-NhomBIB-DiscoveryProblemFraming

## 2. Scan problem (CP1)

**Bối cảnh:** em là backend developer dự án ERP kế toán PM_KT (Java Spring Boot/JPA, PostgreSQL, quản lý ticket trên Plane), đồng thời dạy lập trình tại MindX và là sinh viên HCMUS. Em scan 5 problem, các con số là tự ghi nhận theo trí nhớ các tuần gần nhất, chưa bấm giờ thật nên ghi (ước lượng).

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận thông báo bug kế toán trên dự án PM_KT, tôi muốn nhanh chóng truy xuất đúng luồng code và dữ liệu liên quan, để khoanh vùng vị trí gây lỗi mà không phải dò dẫm thủ công qua hàng chục package | Backend developer, QA, kế toán dùng hệ thống | 3–4 lần/tuần; 90–120 phút/lần để trace log và đọc 5–7 file Java/JPA cùng schema PostgreSQL (ước lượng); ghi nhận qua ticket bug trên Plane |
| 2 | Lặp lại | Khi kết thúc buổi dạy lập trình, tôi muốn tổng hợp các lỗi sai phổ biến và mức độ hoàn thành bài tập của học sinh, để gửi nhận xét và chuẩn bị nội dung cho buổi học tiếp theo | Giáo viên MindX, 12–15 học sinh, phụ huynh | 2 lần/tuần; ~75 phút/buổi để duyệt bài nộp của 12–15 học sinh trên LMS và viết nhận xét thủ công (ước lượng) |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị cho các kỳ thi Cấu trúc dữ liệu và Thuật toán (DSA), tôi muốn tổng hợp các dạng bài tập, mã nguồn mẫu và các lỗi sai về độ phức tạp từ tài liệu rải rác, để có bộ tài liệu ôn tập tập trung | Em, bạn trong nhóm học tập | 2–3 lần/học kỳ; 3–4 giờ/lần lục slide PDF và bài lab OnlineGDB cho 8–10 chủ đề chính (ước lượng) |
| 4 | Lặp lại | Khi đến chiều thứ Sáu hằng tuần, tôi muốn tổng hợp các việc đã hoàn thành, code đã đẩy lên và các điểm nghẽn trong tuần, để gửi báo cáo công việc cho người quản lý đúng hạn | Backend developer, Tech Lead | 1 lần/tuần; ~60 phút xem lại lịch sử Git, tra task trên Plane, đọc lại tin nhắn Slack/Zalo (ước lượng) |
| 5 | Tốn thời gian | Khi chuẩn bị chuyển nơi sinh sống và học tập sang thành phố mới, tôi muốn tổng hợp chi phí sinh hoạt, giá thuê nhà và các phương án di chuyển, để cân đối ngân sách cá nhân chính xác | Em, người thân đi cùng | Mỗi lần có kế hoạch di dời dài hạn; 4–5 giờ đọc bài viết, hội nhóm, trang web nhưng thông tin vẫn phân tán (ước lượng) |

**AI gợi ý thêm:** sau khi tự scan 5 ý, em hỏi AI theo prompt mẫu. AI gợi ý thêm 3 ý; em không thêm dòng mới vì:
- "QA báo lỗi thiếu bước tái hiện" → gộp vào #1, vì là một bước nhỏ trong quy trình xử lý bug, tách riêng sẽ đếm trùng thời gian.
- "Biết học sinh yếu phần nào để soạn giáo án" → gộp vào #2, vì chính là vế "chuẩn bị nội dung buổi học tiếp theo".
- "Trả lời phụ huynh hỏi tiến độ" → bỏ, vì em chưa đếm được số tin nhắn thật, và pain này đã nằm trong #2.

## 3. Top 3 Problem Cards (CP2)

> Thời gian **từng bước** trong quy trình là em chia nhỏ theo trí nhớ từ tổng thời gian ở CP1 (ước lượng); sẽ bấm giờ thật ở các lần tới để kiểm lại.

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Khoanh vùng bug kế toán PM_KT (#1) | Tần suất cao nhất (3–4 lần/tuần), có bằng chứng trên Plane, ảnh hưởng cả QA và kế toán | Bước nào thật sự tốn nhất: đọc log, lần theo code hay đọc schema? Chưa bấm giờ từng bước |
| 2 | Tổng hợp và nhận xét bài tập MindX (#2) | Lặp đều 2 lần/tuần, quy trình rõ, có dữ liệu trên LMS | Học sinh và phụ huynh có thật sự cần nhận xét chi tiết hơn, hay chỉ cần nhanh hơn? |
| 3 | Báo cáo công việc tuần (#4) | Lặp cố định 1 lần/tuần, nguồn dữ liệu rõ (Git, Plane, Slack/Zalo) | Tech Lead đọc phần nào của báo cáo? Có thể chỉ cần danh sách task là đủ |

Không chọn #3 (ôn thi DSA) và #5 (chuyển nơi ở) vì không lặp đều theo tuần và khó đo baseline trong thời gian lab.

### Problem Card #1 — Khoanh vùng bug kế toán PM_KT

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận thông báo bug kế toán trên dự án PM_KT, tôi muốn nhanh chóng truy xuất đúng luồng code và dữ liệu liên quan, để khoanh vùng vị trí gây lỗi mà không phải dò dẫm thủ công qua hàng chục package |
| Actor | Backend developer dự án PM_KT nhận ticket bug từ QA hoặc người dùng kế toán |
| Thời điểm / bối cảnh | Trong giờ làm, ngay khi ticket bug được giao trên Plane; 3–4 lần/tuần |
| Quy trình hiện tại | 1. Đọc ticket trên Plane, tái hiện lỗi · 2. Đọc log tìm stacktrace / request lỗi · 3. Lần theo code qua controller → service → repository trong hàng chục package · 4. Đọc schema và query PostgreSQL liên quan · 5. Khoanh vùng vị trí lỗi, ghi lại vào ticket |
| Bottleneck | Bước 3, lần theo code qua nhiều package: khoảng 30–40 phút/lần vì không có sơ đồ luồng nghiệp vụ, phải mở 5–7 file Java/JPA (ước lượng) |
| Impact | 90–120 phút/lần × 3–4 lần/tuần ≈ 4,5–8 giờ/tuần cho 1 developer (ước lượng); QA và kế toán phải chờ trong lúc lỗi chưa được khoanh vùng |
| Success metric | Thời gian từ lúc nhận ticket đến lúc khoanh vùng được vị trí lỗi: từ 90–120 phút xuống ≤ 45 phút, đo bằng thời gian ghi trên ticket Plane trong 4 tuần |
| Phương án không dùng AI | Thêm mã liên kết request (correlation ID) vào log; viết sơ đồ luồng nghiệp vụ các module kế toán; checklist debug cho từng loại lỗi thường gặp |
| Giả thuyết về AI | Từ nội dung ticket và log lỗi, AI gợi ý các file, hàm và bảng dữ liệu có khả năng liên quan; developer tự kiểm và quyết định vị trí lỗi |
| Cảm nhận nhanh | Workflow |

```text
HIỆN TẠI — khoảng 100 phút/lần (ước lượng)

[1 Đọc ticket + tái hiện: 15'] → [2 Đọc log tìm stacktrace: 20']
→ [3 Lần theo code qua nhiều package: 35'] ← BOTTLENECK
→ [4 Đọc schema + query DB: 20'] → [5 Khoanh vùng, ghi vào ticket: 10']
```

### Problem Card #2 — Tổng hợp và nhận xét bài tập MindX

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc buổi dạy lập trình, tôi muốn tổng hợp các lỗi sai phổ biến và mức độ hoàn thành bài tập của học sinh, để gửi nhận xét và chuẩn bị nội dung cho buổi học tiếp theo |
| Actor | Giáo viên lập trình MindX phụ trách lớp 12–15 học sinh |
| Thời điểm / bối cảnh | Sau mỗi buổi dạy, 2 buổi/tuần, trước khi soạn bài cho buổi tiếp theo |
| Quy trình hiện tại | 1. Mở LMS, xem danh sách bài nộp · 2. Mở và chạy thử từng bài · 3. Đọc logic code tìm lỗi cú pháp/thuật toán · 4. Gom các lỗi phổ biến của cả lớp · 5. Viết nhận xét riêng cho từng học sinh trên LMS |
| Bottleneck | Bước 2–3, mở, chạy thử và đọc code từng bài: khoảng 40–45 phút/buổi cho 12–15 bài (ước lượng) |
| Impact | ~75 phút/buổi × 2 buổi/tuần ≈ 2,5 giờ/tuần (ước lượng); học sinh nhận phản hồi chậm, phụ huynh khó nắm tiến độ |
| Success metric | Thời gian từ lúc mở LMS đến khi gửi xong nhận xét cho cả lớp: từ ~75 phút xuống ≤ 30 phút/buổi, đo bằng tự bấm giờ trong 4 tuần |
| Phương án không dùng AI | Viết sẵn bộ test case cho mỗi bài tập để chạy tự động, báo đạt/không đạt; dùng mẫu nhận xét có sẵn theo các lỗi thường gặp |
| Giả thuyết về AI | Từ kết quả chạy test và code của học sinh, AI soạn nháp nhận xét và gom lỗi phổ biến của lớp; giáo viên đọc, sửa và gửi |
| Cảm nhận nhanh | Rule (chấm bằng test case) + Workflow (AI soạn nháp nhận xét) |

```text
HIỆN TẠI — khoảng 75 phút/buổi (ước lượng)

[1 Mở LMS, xem bài nộp: 5'] → [2 Mở + chạy thử từng bài: 20']
→ [3 Đọc code tìm lỗi: 20'] ← BOTTLENECK (cùng bước 2)
→ [4 Gom lỗi phổ biến: 10'] → [5 Viết nhận xét từng học sinh: 20']
```

### Problem Card #3 — Báo cáo công việc tuần

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến chiều thứ Sáu hằng tuần, tôi muốn tổng hợp các việc đã hoàn thành, code đã đẩy lên và các điểm nghẽn trong tuần, để gửi báo cáo công việc cho người quản lý đúng hạn |
| Actor | Backend developer dự án PM_KT gửi báo cáo tuần cho Tech Lead |
| Thời điểm / bối cảnh | Chiều thứ Sáu hằng tuần, trước khi Tech Lead cập nhật tiến độ chung của team |
| Quy trình hiện tại | 1. Xem lại lịch sử Git commit trong tuần · 2. Tra trạng thái task trên Plane · 3. Đọc lại tin nhắn Slack/Zalo để nhớ các điểm nghẽn · 4. Viết báo cáo theo mẫu · 5. Gửi cho Tech Lead |
| Bottleneck | Bước 1–3, nhặt lại đầu việc từ 3 nguồn: khoảng 35 phút/tuần (ước lượng) |
| Impact | ~60 phút/tuần cho 1 developer (ước lượng); nếu cả team cùng làm thì nhân theo số người; báo cáo trễ làm Tech Lead chậm cập nhật tiến độ |
| Success metric | Thời gian làm báo cáo tuần: từ ~60 phút xuống ≤ 15 phút, đo bằng tự bấm giờ trong 4 tuần; Tech Lead không phải hỏi lại thông tin |
| Phương án không dùng AI | Bộ lọc có sẵn trên Plane (task của tôi, cập nhật trong tuần) + lệnh `git log` theo tác giả và ngày + template báo cáo cố định; ghi chú điểm nghẽn ngay khi gặp trong tuần |
| Giả thuyết về AI | Từ danh sách task và commit đã lọc, AI soạn nháp phần tóm tắt và điểm nghẽn; developer kiểm và gửi |
| Cảm nhận nhanh | No AI hoặc Rule — lọc dữ liệu và template có thể đã đủ |

```text
HIỆN TẠI — khoảng 60 phút/tuần (ước lượng)

[1 Xem Git commit: 10'] → [2 Tra task trên Plane: 10']
→ [3 Đọc lại Slack/Zalo: 15'] ← BOTTLENECK (cùng bước 1–2)
→ [4 Viết báo cáo: 20'] → [5 Gửi: 5']
```

**AI phản biện card #1:**

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 90–120 phút chỉ dựa trên trí nhớ, chưa bấm giờ từng bước | Đồng ý | Ghi rõ (ước lượng); sẽ bấm giờ 3 ticket bug tiếp theo để kiểm lại bước nghẽn |
| "Khoanh vùng xong" chưa có điểm kết thúc rõ, nên metric khó đo | Đồng ý | Định nghĩa điểm kết thúc: khi đã ghi được file/hàm gây lỗi vào ticket Plane |
| Chưa thử phương án không dùng AI (correlation ID, sơ đồ luồng) | Đồng ý | Thêm vào dòng "Phương án không dùng AI", đưa vào giả định cần kiểm chứng ở CP4 |
| Đưa mã nguồn dự án vào công cụ AI có thể vi phạm chính sách công ty/khách hàng | Đồng ý một phần | Đưa vào rủi ro Viability, cần hỏi Tech Lead trước khi thử |

## 4. Tôi đã tham gia phần nào

| Hoạt động | Tôi đã làm gì? | Kết quả |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài bạn khác | | |
| Nhận phản biện | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |

## 5. Dùng AI

| Checkpoint | Dùng AI để làm gì? | Hữu ích ở đâu? | Sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |

## 6. Reflection

>