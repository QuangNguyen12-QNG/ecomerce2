# Ecomerce2

Trang web **Ecomerce2** — ứng dụng thương mại điện tử nhỏ, sử dụng PHP + composer, cấu trúc MVC (hoặc tương tự) với các thành phần app, configs, services, utils, public.

---

## 🚀 Mô tả

- Sử dụng PHP (có composer)  
- Cấu trúc dự án tách rõ các phần `app/`, `configs/`, `public/`, `services/`, `utils/`  
- File cấu hình môi trường `.env` để chứa các biến môi trường như kết nối database  
- Điểm vào chính: `index.php`  

---

## 📂 Cấu trúc thư mục

ecomerce2/
│
├── app/ # Chứa mã nguồn lớp xử lý nghiệp vụ, controllers, models
├── configs/ # File cấu hình như database, routing, config chung
├── public/ # File “công khai” (css, js, hình ảnh), entrypoint có thể đặt trong public nếu sử dụng web server đúng cách
├── services/ # Các service xử lý logic đa phần độc lập
├── utils/ # Các hàm tiện ích, helpers
├── .env # Các biến môi trường (DB, host, user, pass...)
├── index.php # Entry point (gọi bootstrap / khởi tạo ứng dụng)
├── composer.json # Khai báo dependencies
├── composer.lock


---

## 🛠 Yêu cầu

- PHP >= 7.x hoặc 8.x  
- Composer  
- Web server (Apache / Nginx)  
- Database (MySQL, MariaDB, v.v.)  
- Khả năng bật `mod_rewrite` nếu bạn sử dụng URL đẹp / routing  

---

## 🔧 Cài đặt & chạy

Các bước cơ bản:

### 1. Clone repo

```bash
Bước 1: git clone https://github.com/QuangNguyen12-QNG/ecomerce2.git
Bước 2: cd ecomerce2
Bước 3: Nếu bạn đã cài Composer, chạy lệnh:
composer install
Nếu chưa: https://getcomposer.org/download/
Bước 4:
+/Mở phpMyAdmin
+/Tạo database mới tên ecomerce_php
+/Import file ecomerce_php.sql
Bước 5:
+/Mở XAMPP Control Panel → Start Apache và MySQL, 
+/Sau đó truy cập: http://localhost/ecomerce2
