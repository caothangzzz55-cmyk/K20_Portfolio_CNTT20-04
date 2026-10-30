# K20 Portfolio CNTT 20-04

## Thông tin sản phẩm

- **Tên sản phẩm:** Portfolio CV cá nhân
- **Tác giả:** Kiều Cao Thăng
- **Mô tả:** Website tĩnh giới thiệu bản thân, kỹ năng, dự án, quá trình học tập và thông tin liên hệ. Trang có form thực hành kiểm tra dữ liệu bằng HTML5; form không gửi email và không lưu dữ liệu lên máy chủ.

## Liên kết

- **Repository:** [K20_Portfolio_CNTT20-04](https://github.com/caothangzzz55-cmyk/K20_Portfolio_CNTT20-04)
- **GitHub Pages:** [Mở portfolio](https://caothangzzz55-cmyk.github.io/K20_Portfolio_CNTT20-04/)
- **Hồ sơ tác giả:** [github.com/caothangzzz55-cmyk](https://github.com/caothangzzz55-cmyk)
- **Minh chứng:** mã nguồn hai trang là [index.html](./index.html) và [ket-qua.html](./ket-qua.html); ảnh minh họa nằm trong [assets/](./assets/).

## Cấu trúc thư mục

```text
.
├── index.html          # Trang portfolio chính
├── ket-qua.html        # Trang đích sau khi gửi form thực hành
├── README.md           # Hướng dẫn dự án
├── AI_LOG.md           # Nhật ký sử dụng AI
├── RELEASE_NOTES.md    # Ghi chú bàn giao v7
├── css/
│   └── style.css       # Giao diện và responsive
└── assets/
    ├── avatar.svg
    ├── du-an-1.svg
    ├── du-an-2.svg
    └── du-an-3.svg
```

## Chạy trên máy

Đây là website tĩnh, không cần cài thư viện hay build:

1. Tải hoặc clone repository về máy.
2. Mở `index.html` trực tiếp bằng trình duyệt; hoặc chạy server tĩnh tại thư mục dự án:

   ```powershell
   python -m http.server 8000
   ```

3. Mở `http://localhost:8000` trong trình duyệt. Nếu lệnh `python` không có trên máy, có thể dùng `py -m http.server 8000`.

## Nguồn xuất bản

Mã nguồn website nằm ở thư mục gốc của nhánh `main` trong repository; trang GitHub Pages được cung cấp tại URL ở phần liên kết. Cấu hình xuất bản thực tế trong **Settings → Pages** cần được đối chiếu khi bàn giao. Sau khi cập nhật mã, đợi Pages triển khai lại rồi kiểm tra URL công khai.

## Cách kiểm tra các trang và chức năng

1. Mở trang chính và kiểm tra tên tác giả, các mục Giới thiệu, Kỹ năng, Dự án, Học tập và Liên hệ.
2. Kiểm tra giao diện ở chiều rộng desktop và màn hình hẹp; xác nhận CSS, avatar và ba ảnh dự án hiển thị.
3. Chọn liên kết **Xem dự án** và các mục menu để kiểm tra điều hướng đến đúng phần.
4. Thử gửi form liên hệ:
   - Bỏ trống trường bắt buộc hoặc nhập email sai định dạng để kiểm tra xác thực HTML5.
   - Nhập họ tên, email hợp lệ và lời nhắn từ 10 đến 500 ký tự để chuyển đến `ket-qua.html`.
   - Kiểm tra URL có thể chứa dữ liệu form vì form dùng phương thức GET. Form chỉ là bài thực hành, không gửi email và không lưu dữ liệu.
5. Mở trực tiếp `ket-qua.html`, kiểm tra liên kết quay lại phần Liên hệ và xác nhận trang vẫn tải được stylesheet.
6. Sau khi xuất bản, lặp lại các bước kiểm tra trên URL GitHub Pages; mã local chưa được xem là đã triển khai cho tới khi phiên bản trên Pages phản ánh các thay đổi.

## Tài liệu liên quan

- [Nhật ký AI](./AI_LOG.md)
- [Ghi chú phát hành v7](./RELEASE_NOTES.md)
