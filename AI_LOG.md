# AI_LOG

## Ngày 2026-10-30

### Hiện tượng và dữ kiện ban đầu

- Ghi chú có sẵn trong file AI_LOG trước khi cập nhật nêu các hiện tượng: CSS không hiển thị, ảnh dự án bị lỗi và đường dẫn avatar sai.
- Đối chiếu HTML với thư mục dự án cho thấy `index.html` và `ket-qua.html` tham chiếu `style.css` ở thư mục gốc; các tệp thực tế nằm ở `css/style.css`. Avatar và ảnh dự án được tham chiếu ở thư mục gốc, trong khi các tệp thực tế nằm trong `assets/`.
- Người dùng yêu cầu dùng tên Kiều Cao Thăng, cung cấp email `caothangzzz55@gmail.com`, rồi xác nhận repository, GitHub Pages và hồ sơ tác giả. Các URL được ghi trong README.
- Repository không có metadata Git trong bản làm việc này; không có hash commit local để xác nhận.

### Nhận định trước khi dùng AI

Ghi chú ban đầu cho rằng tài nguyên bị lỗi do đường dẫn. Nhận định cần được kiểm tra bằng cách so sánh `href`/`src` trong HTML với vị trí tệp thật trước khi sửa; không nên chỉ đổi tên hiển thị mà bỏ qua các liên kết bị sai.

### Công cụ và yêu cầu gửi cho AI

Đã dùng trợ lý AI trong VS Code. Các yêu cầu chính của người dùng trong phiên:

- “Sửa full tên thành Kiều Cao Thăng”
- “email các thứ nữa”
- Tạo/cập nhật README, AI_LOG và RELEASE_NOTES với thông tin phù hợp sản phẩm.

Người dùng cung cấp URL repository `https://github.com/caothangzzz55-cmyk/K20_Portfolio_CNTT20-04`, URL Pages `https://caothangzzz55-cmyk.github.io/K20_Portfolio_CNTT20-04/` và hồ sơ `https://github.com/caothangzzz55-cmyk`.

### Gợi ý của AI

- Dùng tên và thông tin liên hệ đã được người dùng xác nhận; không tự đoán URL repository hoặc Pages.
- Sửa các đường dẫn tương đối theo đúng thư mục `css/` và `assets/`.
- Viết hướng dẫn chạy website tĩnh, mô tả đúng hành vi form GET và nêu rõ trạng thái xuất bản/commit nào chưa xác minh.

### Quyết định và lý do

Chấp nhận sửa đường dẫn vì cấu trúc thư mục xác nhận các đường dẫn cũ không trỏ tới tệp hiện có. Dùng URL repository/Pages do người dùng cung cấp. Không tạo hash commit giả vì workspace không có thư mục `.git`. Các dự án khác không có URL công khai được xác nhận nên không giữ các liên kết giả; chúng được ghi là chưa có liên kết công khai.

### Phần đã sửa

- `index.html`: sửa stylesheet và ảnh sang `css/` và `assets/`; đồng nhất tên hiển thị; cập nhật liên kết hồ sơ GitHub; thay các địa chỉ dự án chưa xác nhận bằng trạng thái phù hợp.
- `ket-qua.html`: sửa đường dẫn stylesheet.
- `README.md`: bổ sung thông tin sản phẩm, liên kết, cấu trúc thư mục, cách chạy và checklist kiểm tra.
- `RELEASE_NOTES.md`: ghi nội dung bàn giao v7 và các giới hạn đã biết.

### Cách thử lại và kết quả

- Chạy kiểm tra local qua HTTP server: trang chính, `ket-qua.html`, stylesheet, avatar và cả ba ảnh đều trả HTTP 200; các đường dẫn tài nguyên local trong HTML đều trỏ đến tệp hiện có.
- Xác nhận form trong HTML dùng GET và trỏ đến `ket-qua.html`. Chưa ghi nhận thao tác gửi form thực tế hoặc kiểm tra responsive bằng trình duyệt tự động; README hướng dẫn cách kiểm tra thủ công.
- URL Pages có thể mở khi kiểm tra, nhưng nội dung đang được phục vụ chưa phản ánh các sửa đổi đường dẫn local ở lần kiểm tra này. Cần đẩy mã lên repository, đợi GitHub Pages triển khai lại và kiểm tra lại tài nguyên trên URL công khai.

### Sử dụng AI

Có sử dụng AI để hỗ trợ rà soát, chỉnh sửa mã và soạn tài liệu. Các quyết định về tên, email và URL được lấy từ thông tin người dùng cung cấp; kết quả xuất bản chưa được xem là hoàn tất khi chưa kiểm tra lại sau deploy.
