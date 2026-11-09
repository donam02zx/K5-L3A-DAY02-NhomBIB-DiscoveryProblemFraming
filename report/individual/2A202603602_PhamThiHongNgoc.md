# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Thị Hồng Ngọc
- MSSV: 2A202603602
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomBIB
- Link repo nhóm: https://github.com/donam02zx/K5-L3A-DAY02-NhomBIB-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)
Nhân vật: Huyền, GV tiếng anh , dùng Word và các công cụ tìm kiếm để soạn bài cho buổi dạy. Mỗi buổi học, Huyền cần ôn lại bài cũ và dạy kiến thức mới cho học sinh.
Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---|---|---|---|---|
| 1 | **Lặp lại** | Khi chuẩn bị một buổi học mới, tôi muốn hệ thống hóa kiến thức đã dạy ở buổi trước và kết nối với nội dung buổi tiếp theo để đảm bảo tính liên tục trong giảng dạy. | Giáo viên | Mất khoảng **45 phút/buổi** để tổng hợp kiến thức đã dạy và chuẩn bị nội dung cho buổi học tiếp theo. |
| 2 | **Tốn thời gian** | Khi chuẩn bị một bài kiểm tra mới, tôi muốn nhanh chóng tìm kiếm, chọn lọc và tổng hợp kiến thức trong chương trình học cùng các tài liệu tham khảo đáng tin cậy để tiết kiệm thời gian biên soạn đề. | Giáo viên | Mất khoảng **60 phút/bài kiểm tra**, trung bình **10 phút/đơn vị kiến thức** để tìm kiếm và tổng hợp nội dung. |
| 3 | **Pain từ người khác** | Khi ôn tập, học sinh muốn xác định những đơn vị kiến thức chưa nắm vững và tập trung luyện tập các phần đó thay vì tiếp tục làm những dạng bài đã thành thạo để nâng cao hiệu quả ôn tập. | Giáo viên, học sinh | Học sinh có nhu cầu tập trung ôn luyện những phần kiến thức chưa nắm vững; cần theo dõi kết quả học tập để xác định phần đã thành thạo và chưa thành thạo. |
| 4 | **Cần đọc, tổng hợp nhiều thông tin** | Khi chuẩn bị nội dung giảng dạy, tôi muốn kết hợp kiến thức trong chương trình chính khóa với kiến thức nâng cao phù hợp để đảm bảo nội dung vừa đáp ứng chương trình vừa mở rộng năng lực học sinh. | Giáo viên, học sinh | Mất khoảng **20 phút/đơn vị kiến thức** để tìm kiếm, chọn lọc và bổ sung kiến thức nâng cao. |
| 5 | **Lặp lại** | Khi tạo đề ôn tập mới, tôi muốn kiểm soát các đơn vị kiến thức và dạng bài đã xuất hiện trong những đề trước để hạn chế trùng lặp không cần thiết và đảm bảo độ bao phủ kiến thức. | Giáo viên, học sinh | Mất khoảng **15–20 phút** để rà soát đề cũ, kiểm tra mức độ trùng lặp câu hỏi và dạng bài. |

**Nếu có dùng AI để gợi ý thêm:** Sau khi tự scan 3 ý, tôi  hỏi AI và giữ lại ý #4 và #5. Bỏ ý "điều chỉnh độ khó và dạng bài phù hợp với năng lực của từng nhóm học sinh" vì thấy khó cá nhân hóa khi đồng thời cùng giảng dạy giữa các nhóm.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| **Rank** | **Problem** | **Vì sao chọn** | **Điều còn chưa chắc** |
| -------- | ----------- | --------------- | ---------------------- |
| 1 | Theo dõi mức độ nắm vững kiến thức (#3) | Ảnh hưởng trực tiếp đến hiệu quả ôn tập, có tiềm năng ứng dụng AI | Dữ liệu đánh giá mức độ thành thạo có đủ không? |
| 2 | Tìm kiếm, chọn lọc tài liệu (#2) | Quy trình lặp lại, tốn thời gian, có baseline đo được | Độ tin cậy và phù hợp của tài liệu AI đề xuất? |
| 3 | Rà soát đề kiểm tra (#5) | Pain rõ ràng, có thể đo mức độ trùng lặp | Thế nào được xem là câu hỏi trùng lặp hoặc tương tự? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nội dung ôn tập, tôi muốn biết học sinh đã nắm vững và chưa nắm vững những đơn vị kiến thức nào, để tập trung luyện tập vào những phần các em còn yếu. |
| Actor | Huyền – giáo viên tiếng Anh, phụ trách giảng dạy và đánh giá học sinh. |
| Thời điểm / bối cảnh | Sau mỗi bài kiểm tra và trong quá trình chuẩn bị buổi ôn tập. |
| Quy trình hiện tại (3–7 bước) | 1. Tổ chức bài kiểm tra · 2. Chấm bài và ghi nhận kết quả · 3. Xem lại câu trả lời sai · 4. Phân loại lỗi sai theo chủ điểm kiến thức · 5. Xác định nội dung cần ôn tập · 6. Soạn bài tập bổ sung. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Phân loại lỗi sai theo từng đơn vị kiến thức và đánh giá mức độ thành thạo của từng học sinh. Chưa có số liệu thời gian cụ thể. |
| Impact (nếu không giải thì sao) | Giáo viên mất thời gian tổng hợp kết quả; học sinh có thể tiếp tục luyện những kiến thức đã thành thạo trong khi phần còn yếu chưa được chú trọng. |
| Success metric (baseline → target) | Thời gian phân tích kết quả: chưa đo → giảm ít nhất 50%; xác định đúng các đơn vị kiến thức học sinh còn yếu. |
| Phương án không dùng AI | Sử dụng Excel để ghi nhận điểm số, phân loại câu hỏi theo chủ điểm và theo dõi kết quả từng học sinh. |
| Giả thuyết về AI (nếu có) | AI phân tích kết quả bài kiểm tra, phân loại lỗi sai theo chủ điểm và đề xuất các đơn vị kiến thức cần ưu tiên ôn tập. |
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```HIỆN TẠI — Chưa đo được tổng thời gian

[1 Tổ chức bài kiểm tra] → [2 Chấm bài] → [3 Xem lại câu trả lời sai]
→ [4 Phân loại lỗi sai theo chủ điểm] ← BOTTLENECK
→ [5 Xác định kiến thức học sinh chưa nắm vững]
→ [6 Soạn bài tập ôn tập bổ sung]

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nội dung giảng dạy, tôi muốn nhanh chóng tìm kiếm và chọn lọc kiến thức nâng cao phù hợp với chương trình và trình độ học sinh, để hoàn thiện bài giảng. |
| Actor | Huyền – giáo viên tiếng Anh. |
| Thời điểm / bối cảnh | Trước mỗi buổi học, khi cần bổ sung kiến thức hoặc bài tập nâng cao. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định chủ điểm cần bổ sung · 2. Tìm kiếm tài liệu trên Internet · 3. Đọc và đối chiếu nhiều nguồn · 4. Chọn lọc nội dung phù hợp · 5. Điều chỉnh nội dung theo trình độ học sinh · 6. Tổng hợp vào Word. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và 4: Đọc, đối chiếu và chọn lọc thông tin từ nhiều nguồn khác nhau, mất khoảng 20 phút/đơn vị kiến thức. |
| Impact (nếu không giải thì sao) | Tốn thời gian chuẩn bị bài giảng; có nguy cơ lựa chọn nội dung không phù hợp với chương trình hoặc trình độ học sinh. |
| Success metric (baseline → target) | 20 phút/đơn vị kiến thức → dưới 10 phút; nội dung được đề xuất chính xác và phù hợp với trình độ học sinh. |
| Phương án không dùng AI | Xây dựng thư viện tài liệu tham khảo theo chủ điểm, lưu trữ các nguồn uy tín và tái sử dụng nội dung phù hợp. |
| Giả thuyết về AI (nếu có) | AI hỗ trợ tìm kiếm, tổng hợp và phân loại kiến thức từ các nguồn tài liệu đáng tin cậy theo chủ điểm và mức độ khó. |
| Cảm nhận nhanh | Workflow / Agent |
Quy trình nháp hiện tại:

```[1 Xác định chủ điểm cần bổ sung]
→ [2 Tìm kiếm tài liệu trên Internet]
→ [3 Đọc và đối chiếu nhiều nguồn: ~20'/đơn vị kiến thức] ← BOTTLENECK
→ [4 Chọn lọc kiến thức phù hợp]
→ [5 Điều chỉnh theo trình độ học sinh]
→ [6 Tổng hợp vào Word]
BOTTLENECK: Tốn khoảng 20 phút cho mỗi đơn vị kiến thức
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tạo đề kiểm tra hoặc đề ôn tập mới, tôi muốn kiểm tra các câu hỏi và dạng bài đã sử dụng trước đó, để hạn chế trùng lặp và đảm bảo bao phủ kiến thức cần ôn tập. |
| Actor | Huyền – giáo viên tiếng Anh, phụ trách biên soạn đề kiểm tra và đề ôn tập. |
| Thời điểm / bối cảnh | Khi chuẩn bị đề kiểm tra định kỳ hoặc đề ôn tập cho học sinh. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định phạm vi kiến thức · 2. Tìm kiếm câu hỏi phù hợp · 3. Soạn câu hỏi trong Word · 4. Mở lại các đề đã sử dụng · 5. Đối chiếu câu hỏi và dạng bài · 6. Điều chỉnh đề để hạn chế trùng lặp. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 và 5: Rà soát và đối chiếu câu hỏi với các đề đã sử dụng trước đó, mất khoảng 15–20 phút. |
| Impact (nếu không giải thì sao) | Có nguy cơ lặp lại câu hỏi hoặc dạng bài, đồng thời chưa đảm bảo bao phủ đầy đủ các đơn vị kiến thức cần ôn tập. |
| Success metric (baseline → target) | 15–20 phút rà soát → dưới 10 phút; giảm số câu hỏi trùng lặp và đảm bảo các đơn vị kiến thức trong phạm vi ôn tập được bao phủ. |
| Phương án không dùng AI | Lưu trữ đề kiểm tra theo chủ điểm, đánh dấu các câu hỏi đã sử dụng và dùng checklist để kiểm tra trước khi hoàn thiện đề mới. |
| Giả thuyết về AI (nếu có) | AI nhận diện câu hỏi trùng lặp hoặc tương tự, phân loại câu hỏi theo chủ điểm và thống kê mức độ bao phủ kiến thức. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```HIỆN TẠI — Chưa đo được tổng thời gian

[1 Xác định phạm vi kiến thức]
→ [2 Tìm kiếm và soạn câu hỏi]
→ [3 Mở lại các đề đã sử dụng]
→ [4 Đối chiếu câu hỏi và dạng bài: ~15–20']
→ [5 Kiểm tra mức độ trùng lặp] ← BOTTLENECK
→ [6 Điều chỉnh và hoàn thiện đề mới]

BOTTLENECK: Tốn khoảng 15–20 phút để rà soát đề cũ
```

### Card muốn pitch nhất

- Card số: 2 – Tìm kiếm và chọn lọc tài liệu.
- Vì sao:Đây là công việc lặp lại trong quá trình chuẩn bị bài giảng, tiêu tốn khoảng 20 phút cho mỗi đơn vị kiến thức. AI có thể hỗ trợ tìm kiếm, tổng hợp và phân loại tài liệu theo chủ đề, mức độ khó và trình độ học sinh, giúp giáo viên giảm thời gian chuẩn bị nhưng vẫn chủ động kiểm tra nội dung trước khi sử dụng.
- Câu hỏi muốn nhóm phản biện: Làm thế nào để đảm bảo tài liệu do AI tìm kiếm và tổng hợp có nguồn đáng tin cậy, chính xác và phù hợp với trình độ học sinh?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa xác định rõ tiêu chí đánh giá một tài liệu là phù hợp với chương trình và trình độ học sinh. | Đồng ý | Bổ sung tiêu chí phân loại tài liệu theo chủ đề, mức độ khó và trình độ học sinh. |
| AI có thể tổng hợp thông tin thiếu chính xác hoặc sử dụng nguồn không đáng tin cậy. | Đồng ý | Bổ sung yêu cầu cung cấp nguồn tham khảo để giáo viên kiểm tra và xác minh trước khi sử dụng. |
| Chưa có tiêu chí cụ thể để đo lường hiệu quả của giải pháp AI. | Đồng ý | Sử dụng thời gian tìm kiếm và chọn lọc hiện tại (khoảng 20 phút/đơn vị kiến thức) làm baseline; đề xuất mục tiêu giảm xuống dưới 10 phút. |
| Chưa làm rõ liệu AI có thực sự cần thiết hay có thể giải quyết bằng cách lưu trữ tài liệu theo chủ đề. | Đồng ý một phần | Bổ sung phương án không dùng AI: xây dựng thư viện tài liệu theo chủ đề và tái sử dụng nguồn có sẵn. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
