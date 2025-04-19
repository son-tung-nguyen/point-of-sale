Dưới đây là nội dung `README.md` chi tiết hơn cho repo [point-of-sale](https://github.com/son-tung-nguyen/point-of-sale):

---

# 🧾 Point of Sale (POS) System

Hệ thống quản lý bán hàng đơn giản dành cho các cửa hàng nhỏ lẻ, được phát triển bằng Java (Spring Boot) cho backend và HTML/CSS/JS cho frontend.

## 📌 Mục tiêu dự án

- Hỗ trợ cửa hàng tạo, quản lý sản phẩm và hóa đơn
- Quản lý đơn hàng, tính tổng tiền và hiển thị giao diện thanh toán đơn giản
- Dễ triển khai nội bộ, không cần kết nối Internet

---

## 📁 Cấu trúc thư mục

```
point-of-sale/
│
├── BackEnd/           # Mã nguồn Spring Boot backend
│
├── FrontEnd/          # Giao diện web bán hàng
│   ├── css/
│   ├── js/
│   └── index.html
│
├── webposscrip.sql    # Script tạo bảng dữ liệu (MySQL)
│
├── *.xml              # Cấu hình project IntelliJ
└── README.md
```

---

## ⚙️ Công nghệ sử dụng

| Thành phần | Công nghệ            |
|-----------|----------------------|
| Frontend  | HTML, CSS, JavaScript |
| Backend   | Java, Spring Boot    |
| Database  | MySQL                |

---

## 🚀 Cách triển khai

### 1. Cơ sở dữ liệu

- Tạo database trong MySQL, ví dụ: `pos_system`
- Import file `webposscrip.sql` vào database

```bash
mysql -u root -p pos_system < webposscrip.sql
```

### 2. Backend (Spring Boot)

- Mở thư mục `BackEnd` bằng IntelliJ hoặc Eclipse
- Cấu hình file `application.properties` để kết nối với MySQL
- Chạy ứng dụng Spring Boot

### 3. Frontend

- Mở `FrontEnd/index.html` bằng trình duyệt
- Giao diện sẽ gửi request tới backend để tạo hóa đơn và xử lý sản phẩm

---

## 🎯 Các chức năng chính

- Thêm/sửa/xóa sản phẩm
- Thêm sản phẩm vào hóa đơn
- Tính tổng tiền hóa đơn
- Lưu thông tin hóa đơn vào database

---

## 🧪 Demo nhanh

> Do không có host online, bạn cần chạy local để trải nghiệm

1. Chạy backend Spring Boot
2. Mở `index.html` trong trình duyệt
3. Thêm sản phẩm, tạo đơn hàng, thử thanh toán

---

## 📝 Ghi chú

- Dự án ở trạng thái MVP (minimum viable product)
- Cần hoàn thiện thêm phần kiểm tra lỗi và bảo mật
- Phù hợp với sinh viên học Spring Boot hoặc làm bài tập lớn

---

## 📄 License

Dự án sử dụng [MIT License](LICENSE)

---

