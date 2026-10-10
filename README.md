# [Bài tập] Thiết kế Trang Giới Thiệu Sản Phẩm (Apple iPhone Product Page)

Dự án bài tập thực hành thiết kế giao diện **Trang Giới Thiệu Sản Phẩm** lấy cảm hứng từ trang giới thiệu sản phẩm cao cấp [Apple iPhone Product Page](https://www.apple.com/iphone/), vận dụng linh hoạt **Bootstrap Grid System**, **Flexbox** (`justify-content`, `align-items`), **Display & Spacing Utilities** (`margin`, `padding`), kết hợp biểu tượng **Font Awesome 6**.

---

## 🎯 Mục Tiêu Bài Tập

- Luyện tập sử dụng các thuộc tính `display`, `margin`, `padding`, `contents` trong Bootstrap 5.
- Vận dụng thành thạo **Flexbox** (`d-flex`, `justify-content-center`, `justify-content-between`, `align-items-center`, `flex-column`, `flex-md-row`, `gap-*`) để căn chỉnh và phân bổ nội dung hợp lý.
- Sử dụng **Bootstrap Grid System** (`container`, `row`, `col-*`, `g-4`) để xây dựng bố cục trang đáp ứng (responsive).
- Tận dụng icon từ **Font Awesome 6.5.2** để làm nổi bật các tính năng và thông số kỹ thuật sản phẩm.
- Tuân thủ nguyên tắc: **Hạn chế việc viết thêm CSS mới, tập trung sử dụng các lớp có sẵn trong Bootstrap**.

---

## 🏗️ Bố Cục Trang Web (Apple iPhone Style Architecture)

```plaintext
Trang Giới Thiệu Sản Phẩm (iPhone 16 Pro)
│
├── 1. Navbar Toàn Cầu (Apple Navigation):
│   ├── Logo Apple, thanh menu danh mục, thanh tìm kiếm & giỏ hàng
│
├── 2. Sub-Navbar Sản Phẩm (Sticky-top):
│   ├── Tên sản phẩm "iPhone 16 Pro", liên kết điều hướng nhanh và nút "Mua ngay"
│
├── 3. Hero Section 1: iPhone 16 Pro (Titanium Flagship):
│   ├── Tiêu đề lớn & khẩu hiệu sản phẩm
│   ├── Flexbox CTA Buttons ("Mua ngay", "Xem phim giới thiệu")
│   └── Hình ảnh sản phẩm lớn Titanium (img-fluid mx-auto d-block)
│
├── 4. Hero Section 2: iPhone 16 (Đầy Màu Sắc & Quyền Năng):
│   ├── Giới thiệu phiên bản tiêu chuẩn với các nút hành động và hình ảnh nổi bật
│
├── 5. Đặc Điểm Nổi Bật (Bento Grid - 4 Cột Tính Năng):
│   ├── Chip A18 Pro (fas fa-microchip)
│   ├── Camera 48MP Fusion & Zoom quang học 5x (fas fa-camera)
│   ├── Nút Điều Khiển Camera mới (fas fa-sliders)
│   └── Thời lượng pin vượt trội lên đến 33 giờ (fas fa-battery-full)
│
├── 6. Bảng So Sánh Các Dòng Sản Phẩm (Compare Models - 3 Cột):
│   ├── iPhone 16 Pro Max (6.9 inch)
│   ├── iPhone 16 Pro (6.3 inch)
│   └── iPhone 16 (6.1 inch)
│
├── 7. Khu Vực Kêu Gọi Hành Động (CTA Section - Đặt Mua & Tìm Cửa Hàng)
│
└── 8. Chân Trang (Footer Chuẩn Phong Cách Apple):
    └── Thông tin bản quyền, danh mục liên kết và điều khoản dịch vụ
```

---

## 💡 Các Lớp Bootstrap Được Áp Dụng Triệt Để

| Nhóm thuộc tính | Các lớp Bootstrap được sử dụng | Mục đích áp dụng |
| :--- | :--- | :--- |
| **Flexbox & Canh Lề** | `d-flex`, `justify-content-center`, `justify-content-between`, `align-items-center`, `flex-column`, `flex-md-row`, `gap-3` | Bố trí hàng nút bấm, căn chỉnh navbar và thẻ tính năng theo cả 2 trục |
| **Grid System** | `container`, `row`, `col-12`, `col-md-6`, `col-lg-3`, `col-md-4`, `g-4`, `g-0` | Bố cục dạng lưới đa cột tự động co giãn từ Mobile đến Desktop |
| **Margin & Padding** | `py-5`, `py-4`, `py-2`, `my-4`, `mb-3`, `mb-4`, `p-4`, `px-4`, `pt-3` | Tạo khoảng cách thông thoáng, chuẩn tỷ lệ vàng giữa các section |
| **Display & Responsive** | `d-none`, `d-md-flex`, `d-block`, `d-flex` | Kiểm soát hiển thị các thành phần theo từng kích thước màn hình |
| **Theme & Colors** | `bg-black`, `bg-dark`, `text-white`, `text-secondary`, `btn-apple`, `rounded-pill`, `rounded-4` | Tái hiện giao diện Dark Mode sang trọng đặc trưng của Apple |

---

## 📱 Khả Năng Tương Thích & Responsive

- **Desktop (≥ 992px)**: Hiển thị đầy đủ menu điều hướng, bento grid 4 cột ngang, bảng so sánh 3 cột chi tiết.
- **Tablet (768px - 991px)**: Lưới tính năng tự động chuyển thành 2 cột x 2 hàng, căn chỉnh cân xứng.
- **Mobile (< 768px)**: Các cột tự động xếp chồng (stacking), nút bấm mở rộng dễ chạm trên màn hình cảm ứng.

---

## 🚀 Hướng Dẫn Xem Dự Án

1. **Xem trực tiếp**: Nhấp đúp vào tệp [index.html](file:///d:/BaiTapGithub/index.html) để mở trên trình duyệt web.
2. **Xem qua Live Server**: Chuột phải vào `index.html` trong IDE và chọn **Open with Live Server** (`http://127.0.0.1:5500/index.html`).

---

## 👨‍💻 Thông Tin Học Viên

- **Học viên**: dtc245200059
- **Email**: dtc245200059@ictu.edu.vn
- **Bài tập**: Thiết kế Trang Giới Thiệu Sản Phẩm (Phong cách Apple iPhone)
