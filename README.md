# 🏃‍♂️ Mapty - Map Your Workouts

Ứng dụng web giúp bạn theo dõi và ghi lại các hoạt động thể thao (chạy bộ và đạp xe) trên bản đồ tương tác.

![Mapty App](./logo.png)

## ✨ Tính năng

- 📍 **Định vị tự động**: Tự động xác định vị trí hiện tại của bạn
- 🗺️ **Bản đồ tương tác**: Sử dụng Leaflet.js để hiển thị bản đồ OpenStreetMap
- 🏃‍♂️ **Theo dõi chạy bộ**: Ghi lại khoảng cách, thời gian, tốc độ và nhịp bước
- 🚴‍♀️ **Theo dõi đạp xe**: Ghi lại khoảng cách, thời gian, tốc độ và độ cao
- 💾 **Lưu trữ cục bộ**: Tự động lưu dữ liệu vào Local Storage
- 🎯 **Điều hướng nhanh**: Click vào workout để di chuyển đến vị trí trên bản đồ

## 🚀 Live Demo

👉 **[Xem Demo Trực Tiếp](https://sai-ctruong.github.io/Mapty/)**

Nhấp vào bất kỳ vị trí nào trên bản đồ để thêm workout mới!

## 🛠️ Công nghệ sử dụng

- **HTML5** - Cấu trúc trang web
- **CSS3** - Styling và responsive design
- **JavaScript (ES6+)** - Logic ứng dụng với OOP
- **Leaflet.js** - Thư viện bản đồ tương tác
- **Geolocation API** - Lấy vị trí người dùng
- **Local Storage API** - Lưu trữ dữ liệu

## 📦 Cài đặt

1. Clone repository này:
```bash
git clone https://github.com/sai-ctruong/Mapty.git
```

2. Di chuyển vào thư mục dự án:
```bash
cd mapty
```

3. Mở file `index.html` trong trình duyệt hoặc sử dụng Live Server

## 💻 Sử dụng

1. **Cho phép truy cập vị trí**: Khi mở ứng dụng, cho phép trình duyệt truy cập vị trí của bạn
2. **Thêm workout mới**: Click vào bất kỳ vị trí nào trên bản đồ
3. **Điền thông tin**: 
   - Chọn loại hoạt động (Running/Cycling)
   - Nhập khoảng cách (km)
   - Nhập thời gian (phút)
   - Nhập cadence (chạy bộ) hoặc elevation gain (đạp xe)
4. **Xem workout**: Workout sẽ hiển thị trong danh sách bên trái và marker trên bản đồ
5. **Điều hướng**: Click vào workout trong danh sách để di chuyển đến vị trí đó trên bản đồ

## 📱 Responsive Design

Ứng dụng được thiết kế để hoạt động tốt trên các thiết bị desktop. Mobile responsive có thể được cải thiện trong các phiên bản tương lai.

## 🎨 Cấu trúc dự án

```
mapty/
│
├── index.html          # File HTML chính
├── style.css           # Styling
├── script.js           # Logic ứng dụng
├── logo.png            # Logo ứng dụng
├── icon.png            # Favicon
└── README.md           # Tài liệu
```

## 🔧 Kiến trúc Code

Ứng dụng sử dụng lập trình hướng đối tượng (OOP) với các class:

- **`Workout`**: Class cha cho các loại workout
- **`Running`**: Class con cho hoạt động chạy bộ
- **`Cycling`**: Class con cho hoạt động đạp xe
- **`App`**: Class chính quản lý toàn bộ ứng dụng

## 🌟 Tính năng nổi bật

### Local Storage
Tất cả workout được tự động lưu vào Local Storage, dữ liệu sẽ được giữ lại ngay cả khi đóng trình duyệt.

### Tính toán tự động
- **Chạy bộ**: Tự động tính pace (phút/km)
- **Đạp xe**: Tự động tính speed (km/h)

## 🐛 Debug

Để xóa tất cả workout và reset ứng dụng, mở Console và chạy:
```javascript
app.reset()
```

## 📝 License

Dự án này được tạo ra cho mục đích học tập. 

© Copyright by [Jonas Schmedtmann](https://twitter.com/jonasschmedtman). Sử dụng cho học tập hoặc portfolio cá nhân.
