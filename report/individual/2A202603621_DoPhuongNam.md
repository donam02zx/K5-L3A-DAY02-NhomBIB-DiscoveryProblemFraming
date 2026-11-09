## 1. Thông tin học viên

- **Họ tên:** Đỗ Phương Nam 
- **MSSV:** 2A202603621
- **Email trường** (không bắt buộc, repo có thể để public):
- **Tên nhóm:** NhomBIB
- **Link repo nhóm:** https://github.com/donam02zx/K5-L3A-DAY02-NhomBIB-DiscoveryProblemFraming

## 2. CP1 — Scan 5+ problems · Discover

> Các con số là em tự ghi nhận theo trí nhớ trong các tuần gần nhất, chưa đo bằng công cụ → ghi **(ước lượng)**.

### Problem 1: Xử lý và khoanh vùng bug hệ thống ERP (PM_KT)

| Lăng kính | Phân tích |
|---|---|
| **Lặp lại** | Xảy ra liên tục mỗi tuần khi có thông báo lỗi từ hệ thống kế toán. |
| **Tốn thời gian** | Mất nhiều thời gian mò mẫm qua hàng chục package code và cấu trúc bảng database phức tạp. |
| **Cần đọc, tổng hợp nhiều thông tin** | Phải đọc hiểu đồng thời log hệ thống, mã nguồn Spring Boot/JPA và cấu trúc schema PostgreSQL. |
| **Pain từ người khác** | Team kiểm thử (QA) và kế toán bị gián đoạn công việc khi tính năng bị lỗi. |
| **Job Story** | Khi nhận thông báo bug kế toán trên dự án PM_KT, tôi muốn nhanh chóng truy xuất đúng luồng code và dữ liệu liên quan, để khoanh vùng vị trí gây lỗi mà không phải dò dẫm thủ công qua hàng chục package. |
| **Dấu hiệu thật** | Xảy ra khoảng 3–4 lần/tuần; mất trung bình 90–120 phút cho mỗi lần trace log và đọc qua 5–7 file Java/JPA (ước lượng); được ghi nhận trực tiếp qua các ticket bug trên nền tảng Plane. |

---

### Problem 2: Tổng hợp và đánh giá bài tập học sinh tại MindX

| Lăng kính | Phân tích |
|---|---|
| **Lặp lại** | Lặp lại đều đặn sau mỗi buổi lên lớp (2 buổi/tuần). |
| **Tốn thời gian** | Mất thời gian mở từng file bài nộp của học sinh để chạy thử và kiểm tra lỗi. |
| **Cần đọc, tổng hợp nhiều thông tin** | Phải đọc logic code của từng học sinh để tìm ra các lỗi sai cú pháp/thuật toán phổ biến rồi viết nhận xét riêng. |
| **Pain từ người khác** | Học sinh không nhận được phản hồi chi tiết kịp thời, phụ huynh muốn nắm tiến độ nhưng thông tin chậm. |
| **Job Story** | Khi kết thúc buổi dạy lập trình, tôi muốn tổng hợp các lỗi sai phổ biến và mức độ hoàn thành bài tập của học sinh, để gửi nhận xét và chuẩn bị nội dung cho buổi học tiếp theo. |
| **Dấu hiệu thật** | Diễn ra 2 lần/tuần; mất khoảng 75 phút sau mỗi buổi học để duyệt qua bài nộp của 12–15 học sinh trên LMS và viết nhận xét thủ công (ước lượng). |

---

### Problem 3: Hệ thống hoá tài liệu ôn tập Cấu trúc dữ liệu và Thuật toán (DSA)

| Lăng kính | Phân tích |
|---|---|
| **Lặp lại** | Lặp lại trước mỗi đợt kiểm tra lớn hoặc kỳ thi kết thúc học phần tại HCMUS. |
| **Tốn thời gian** | Tốn nhiều giờ đồng hồ tìm kiếm, lọc lại các tài liệu bị phân tán ở nhiều nơi. |
| **Cần đọc, tổng hợp nhiều thông tin** | Phải đọc hàng loạt slide PDF bài giảng, mã nguồn C++ mẫu trên OnlineGDB và các ghi chú cá nhân để gom nhóm kiến thức. |
| **Pain từ người khác** | Bạn bè trong nhóm học tập cũng gặp khó khăn khi tổng hợp các dạng bài tập và độ phức tạp thuật toán tương tự. |
| **Job Story** | Khi chuẩn bị cho các kỳ thi Cấu trúc dữ liệu và Thuật toán (DSA), tôi muốn tổng hợp các dạng bài tập, mã nguồn mẫu và các lỗi sai về độ phức tạp từ tài liệu rải rác, để có bộ tài liệu ôn tập tập trung. |
| **Dấu hiệu thật** | Xảy ra trước mỗi kỳ thi (2–3 lần/học kỳ); mất 3–4 tiếng lục lọi slide PDF và bài lab OnlineGDB cho 8–10 chủ đề chính (ước lượng). |

---

### Problem 4: Lập báo cáo công việc tuần (Weekly Report)

| Lăng kính | Phân tích |
|---|---|
| **Lặp lại** | Định kỳ đúng vào chiều thứ Sáu hằng tuần. |
| **Tốn thời gian** | Mất thời gian nhớ lại và tìm kiếm lại các công việc đã làm trong tuần qua các công cụ khác nhau. |
| **Cần đọc, tổng hợp nhiều thông tin** | Phải đọc lại lịch sử Git commit, kiểm tra trạng thái ticket trên Plane và lội lại tin nhắn nhóm chat trên Slack/Zalo. |
| **Pain từ người khác** | Tech Lead cần báo cáo tổng hợp đúng giờ để cập nhật tiến độ chung của team. |
| **Job Story** | Khi đến chiều thứ Sáu hằng tuần, tôi muốn tổng hợp các công việc đã hoàn thành, mã nguồn đã đẩy lên hệ thống và các điểm nghẽn trong tuần, để viết báo cáo công việc gửi người quản lý đúng hạn. |
| **Dấu hiệu thật** | Diễn ra 1 lần/tuần cố định; mất khoảng 60 phút lội lịch sử Git, tra cứu task trên Plane và đọc lại tin nhắn để nhặt lại đầu việc (ước lượng). |

---

### Problem 5: Thu thập thông tin và dự toán chi phí di chuyển, sinh hoạt khi chuyển chỗ ở

| Lăng kính | Phân tích |
|---|---|
| **Lặp lại** | Xảy ra mỗi khi có kế hoạch thay đổi môi trường sống hoặc học tập sang thành phố mới. |
| **Tốn thời gian** | Mất hàng giờ lướt qua nhiều hội nhóm và trang web để tìm kiếm dữ liệu. |
| **Cần đọc, tổng hợp nhiều thông tin** | Phải đọc rất nhiều bài viết chia sẻ kinh nghiệm, bảng giá thuê nhà, chi phí đi lại từ nhiều nguồn không đồng nhất. |
| **Pain từ người khác** | Các thành viên khác trong gia đình/nhóm đi cùng cũng hoang mang vì thiếu thông tin tổng quan. |
| **Job Story** | Khi chuẩn bị thay đổi địa điểm sinh sống và học tập sang thành phố mới, tôi muốn tổng hợp chi phí sinh hoạt, giá thuê nhà và các phương án di chuyển, để cân đối ngân sách cá nhân chính xác. |
| **Dấu hiệu thật** | Xảy ra khi có kế hoạch di dời dài hạn; mất khoảng 4–5 tiếng đọc qua nhiều bài viết, hội nhóm nhưng thông tin vẫn bị phân tán, khó đối chiếu (ước lượng). |

---

### Ý gợi ý thêm từ AI (làm sau khi đã tự scan)

| Ý AI gợi ý | Giữ / Bỏ | Lý do |
|---|---|---|
| Khi QA báo lỗi kế toán mà mô tả thiếu bước tái hiện, tôi muốn có đủ dữ liệu và bước tái hiện ngay trong ticket, để không phải hỏi lại | Gộp vào Problem 1 | Là một bước nhỏ trong quy trình xử lý bug của Problem 1, tách riêng sẽ đếm trùng thời gian |
| Khi chuẩn bị giáo án buổi tiếp theo, tôi muốn biết học sinh đang yếu phần nào, để chọn bài tập phù hợp | Gộp vào Problem 2 | Chính là vế "chuẩn bị nội dung buổi học tiếp theo" của Problem 2 |
| Khi phụ huynh hỏi tiến độ học của con, tôi muốn trả lời nhanh với thông tin cụ thể, để giữ niềm tin của phụ huynh | Bỏ | Em chưa đếm được số tin nhắn thật của phụ huynh; phần pain này đã nằm trong Problem 2 |

