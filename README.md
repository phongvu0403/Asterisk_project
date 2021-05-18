**Đây là project của môn học Mạng thông tin. Project làm về một số yêu cầu kỹ thuật khi tiếp cận với Asterisk Server (là hệ thống chuyển mạch mềm).**
-
**Các yêu cầu kỹ thuật bao gồm:**
1. Cài đặt Asterisk Server và các Client VoIP.
2. Thực hiện đàm thoạt voice + text conference giữa ít nhất 3 user.
3. Ghi âm cuộc gọi vào cơ sở dữ liệu, ghi lại tốc độ dòng số của từng người dùng và tổng dung lượng thông tin trao đổi trên mạng.

**Các file config trong project là các config được thêm hoặc sửa đổi từ source code của Asterisk.**

**Cụ thể hơn:**

* *pjsip.conf* định nghĩa về thông tin về người dùng được đăng kí với Server

* *extensions.conf* định nghĩa trình tự các bước, các ứng dụng được chạy và thực hiện trong quá trình gọi điện giữa các user.

* *confbridge.conf* định nghĩa các cài đặt mặc định về cuộc gọi hội nghị và hồ sơ các user có thể tham gia cuộc thoại này.

* *module.conf* định nghĩa các module được hoặc không được sử dụng bên trong Server.

* *cdr.conf* định nghĩa các cấu hình kết nối CDR (Call Detail Record) với trường DSN (Data Source Name) trong database.

* *res_odbc.conf* định nghĩa DSN trong database

* *cdr_adaptive_odbc.conf* định nghĩa các dữ liệu trong CDR sẽ được lưu vào đâu trong databse
