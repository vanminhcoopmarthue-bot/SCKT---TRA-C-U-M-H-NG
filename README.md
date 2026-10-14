# Co.opmart Huế — Tra cứu mã hàng

## 6 tệp đưa lên GitHub
- `index.html` — giao diện tìm kiếm và quét mã vạch.
- `icon.svg` — biểu tượng ứng dụng.
- `manifest.webmanifest` — cấu hình cài đặt PWA.
- `sw.js` — cache tài nguyên giao diện.
- `logo-coopmart.jpg` — logo.
- `README.md` — hướng dẫn.

## Cài đặt GitHub Pages
1. Tải đủ 6 tệp trong thư mục `GITHUB_6_FILES` lên thư mục gốc repository.
2. Vào Settings → Pages.
3. Chọn Deploy from a branch → `main` → `/(root)` → Save.
4. Trong `index.html`, kiểm tra hằng `API_URL` và thay bằng URL Web App Apps Script mới của bạn nếu URL khác.

## Apps Script
Mã backend nằm trong thư mục `../APPS_SCRIPT/Code.gs`. Sau khi dán vào Apps Script, lưu và triển khai dạng Web app. Mở URL với `?action=test` để kiểm tra kết nối.

## Cấu trúc dữ liệu giả định
Code.gs mặc định đọc tab `DATA TỔNG`, hàng 1 là tiêu đề và các cột A–F lần lượt là: mã vạch, SKU, tên hàng, quy cách, tồn kho, giá. Nếu bảng thực tế khác thứ tự này, chỉnh các chỉ số cột trước khi dùng.
