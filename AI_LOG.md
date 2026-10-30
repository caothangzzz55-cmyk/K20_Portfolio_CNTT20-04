không hiện css
ảnh dự án bị lỗi ko hiển thị
sai đường dẫn avatar

2026-10-30: Sửa đường dẫn tài nguyên cho GitHub Pages:
- Đổi stylesheet sang `css/style.css` trong `index.html` và `ket-qua.html`.
- Đổi avatar và ba ảnh dự án sang các đường dẫn trong thư mục `assets/`.
- Nguyên nhân: HTML tham chiếu tệp ở thư mục gốc, trong khi các tệp thực tế nằm trong `css/` và `assets/`.
