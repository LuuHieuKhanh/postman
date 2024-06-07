1. Giới thiệu về Postman:
Postman là gì?
Postman là một ứng dụng desktop giúp phát triển và kiểm thử các API một cách dễ dàng. Nó cho phép bạn gửi các yêu cầu HTTP đến các điểm cuối API, kiểm tra phản hồi và tổ chức các yêu cầu trong bộ sưu tập.

Các tính năng chính của Postman:
Postman cung cấp giao diện dễ sử dụng để tạo, gửi và kiểm tra các yêu cầu HTTP, hỗ trợ các phương thức HTTP như GET, POST, PUT, DELETE. Nó cũng có các tính năng như quản lý biến, bộ sưu tập dữ liệu và kiểm thử tự động.

Cách cài đặt và sử dụng Postman:
Truy cập trang web của Postman để tải xuống và cài đặt phiên bản miễn phí. Sau khi cài đặt, khởi động Postman và tham khảo phần hướng dẫn sử dụng để hiểu cách sử dụng các tính năng chính.

2. Kiểm thử API cơ bản:
Tạo các yêu cầu HTTP (GET, POST, PUT, DELETE) trong Postman và gửi đến API.
Kiểm tra mã trạng thái HTTP và nội dung phản hồi để đảm bảo tính chính xác của API.
Sử dụng biến để lưu trữ và truy cập dữ liệu, cũng như tạo bộ sưu tập dữ liệu để quản lý nhiều yêu cầu và biến.
Sử dụng công cụ JSON validator để xác minh tính hợp lệ của JSON.
3. Kiểm thử API nâng cao:
Kiểm tra xác thực và ủy quyền bằng cách bao gồm thông tin xác thực trong các yêu cầu HTTP.
Đo thời gian phản hồi để kiểm tra hiệu suất của API.
Tìm hiểu về các lỗ hổng bảo mật phổ biến và viết các yêu cầu HTTP để kiểm tra bảo mật của API.
Sử dụng các công cụ kiểm thử tự động trong Postman để viết các kịch bản kiểm thử.
# API kiểm thử: https://openweathermap.org/api
# Báo cáo kiểm thử API
**1. Mục tiêu kiểm thử**
- Mục tiêu của kiểm thử là đảm bảo rằng các chức năng chính của Random Data API hoạt động chính xác và hiệu quả. Phạm vi kiểm thử bao gồm các endpoint chính như /people, /people/{id}, /random, và /search.

**2. Kết quả kiểm thử**

***2.1. GET /people***
- Mã trạng thái: 200 OK
- Nội dung phản hồi: Danh sách các thông tin về người.
- Kết quả: Thành công
  
***2.2. GET /people/{id} (ID hợp lệ)***
- Mã trạng thái: 200 OK
- Nội dung phản hồi: Thông tin chi tiết về người có ID = afa4b392-2059-437b-9456-c2de74315db8.
- Kết quả: Thành công
  
***2.3. GET /people/{id} (ID không hợp lệ)***
- Mã trạng thái: 404 Not Found
- Nội dung phản hồi: Lỗi "Not Found".
- Kết quả: Thành công
  
***2.4. GET /search?q={query} (có kết quả)***
- Mã trạng thái: 200 OK
- Nội dung phản hồi: Danh sách các thông tin về người phù hợp với từ khóa "John".
- Kết quả: Thành công

***2.5. GET /search?q={query} (không có kết quả)***
- Mã trạng thái: 404 Not Found
- Nội dung phản hồi: Lỗi "Not Found".
- Kết quả: Thành công

**3. Tóm tắt**
- API Random Data đã được kiểm thử và chứng minh rằng các chức năng chính hoạt động chính xác và hiệu quả. Tất cả các endpoint đã được kiểm tra và trả về các kết quả phù hợp với yêu cầu.
