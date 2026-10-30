# Release notes - v7

## Thông tin bàn giao

- **Sản phẩm:** Portfolio CV cá nhân - Kiều Cao Thăng
- **Phiên bản:** v7
- **Ngày cập nhật:** 2026-10-30
- **Repository đích:** [K20_Portfolio_CNTT20-04](https://github.com/caothangzzz55-cmyk/K20_Portfolio_CNTT20-04)
- **GitHub Pages:** [Mở portfolio](https://caothangzzz55-cmyk.github.io/K20_Portfolio_CNTT20-04/)

## Thay đổi chính

- Đồng nhất tên tác giả và cập nhật thông tin liên hệ theo dữ liệu người dùng xác nhận.
- Sửa các đường dẫn stylesheet, avatar và ảnh dự án theo cấu trúc thật của `css/` và `assets/`.
- Bổ sung hướng dẫn chạy, kiểm tra và nhật ký sử dụng AI.

## Lỗi đã sửa

- Trang chính và trang kết quả trỏ đến `style.css` ở sai vị trí.
- Avatar và ảnh dự án được tham chiếu ở thư mục gốc thay vì `assets/`.
- Một số chuỗi hồ sơ/dự án không có URL công khai đã xác nhận.

## Commit và bản mã

- **Commit liên quan:** chưa có hash commit local để ghi nhận; thư mục làm việc hiện tại không có metadata `.git`. Không dùng commit trên remote làm bằng chứng cho các chỉnh sửa local chưa được xác nhận đã đẩy lên.
- **Mã nguồn v7 trong bản làm việc:** [index.html](./index.html), [ket-qua.html](./ket-qua.html), [css/style.css](./css/style.css), [assets/](./assets/).
- Repository và Pages ở trên là đích lưu trữ/xuất bản. Tại thời điểm ghi chú, URL Pages còn phục vụ phiên bản chưa phản ánh các sửa đường dẫn local; cần đồng bộ mã v7 lên repository rồi kiểm tra lại sau khi Pages triển khai.

## Hạn chế còn lại và bước bàn giao

- Form liên hệ chỉ kiểm tra dữ liệu HTML5 và chuyển bằng GET; không gửi email, không lưu dữ liệu, và nội dung nhập có thể xuất hiện trên URL.
- Hai dự án thực hành không có repository công khai đã xác nhận.
- Font Inter tải từ Google Fonts nên cần kết nối mạng để dùng font bên ngoài.
- Sau khi đồng bộ các tệp v7 lên nhánh xuất bản, ghi lại hash commit thực tế; kiểm tra CSS, ảnh, menu, giao diện responsive và luồng form trên cả `index.html`, `ket-qua.html` lẫn URL Pages.

## Kiểm tra trong bản làm việc

Chạy website bằng HTTP server local: trang chính, trang kết quả, stylesheet, avatar và ba ảnh đều trả HTTP 200; form trong HTML dùng GET đến `ket-qua.html`. Chưa xác nhận thao tác gửi form hoặc kiểm thử giao diện trên trình duyệt. URL Pages cần được kiểm tra lại sau khi đồng bộ và triển khai v7.
