#  Food Category App - Mobile Programing

Đây là dự án bài tập Android minh họa cách kết nối API, xử lý dữ liệu JSON và hiển thị danh sách hình ảnh sử dụng các thư viện phổ biến nhất hiện nay.

## Ảnh sản phẩm

<p align="center"><img width="322" height="686" alt="Image" src="https://github.com/user-attachments/assets/ea79d9b2-827e-445b-b298-f58b07c0845f" /></p>

##  Tính năng chính
- **Gọi API:** Lấy danh sách danh mục món ăn từ Server.
- **Hiển thị danh sách:** Sử dụng `RecyclerView` với `LinearLayoutManager` (Horizontal).
- **Xử lý hình ảnh:** Tải ảnh từ URL và cache ảnh tự động bằng `Glide`.
- **Mô hình hóa dữ liệu:** Chuyển đổi JSON sang Java Object bằng `GSON`.

##  Công nghệ & Thư viện sử dụng
- **Ngôn ngữ:** Java
- **Retrofit 2:** `com.squareup.retrofit2:retrofit:2.9.0` (Networking)
- **GSON:** `com.squareup.retrofit2:converter-gson:2.9.0` (JSON Parsing)
- **Glide:** `com.github.bumptech.glide:glide:4.14.2` (Image Loading)
- **Thành phần UI:** `RecyclerView`, `CardView`, `ConstraintLayout`.

##  Thông tin API
Dự án sử dụng API nội bộ:
- **Base URL:** `http://app.iotstar.vn:8081/appfoods/`
- **Endpoint:** `categories.php`
- **Method:** `GET`

##  Cấu trúc Project
```text
com.example.baitap5
├── model
│   └── Category.java        # Model ánh xạ dữ liệu JSON
├── api
│   ├── RetrofitClient.java  # Cấu hình Retrofit (Singleton Pattern)
│   └── APIService.java      # Interface định nghĩa các API request
├── adapter
│   └── CategoryAdapter.java # Adapter xử lý hiển thị cho RecyclerView
└── MainActivity.java        # Màn hình chính gọi API và hiển thị dữ liệu
```

## Tác giả
**Tên: Dương Đình Ngọc Khang** 

**MSSV: 23162036**
