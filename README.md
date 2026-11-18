# 📡 RTL8720DN WiFi Scanner – BW16

Hệ thống quét và phân tích mạng WiFi băng tần kép (2.4GHz & 5GHz) chạy trên bo mạch **BW16 (chip RTL8720DN)**, tích hợp giao diện điều khiển Web trực quan được Việt hóa hoàn toàn.

![Platform](https://img.shields.io/badge/Platform-Arduino%20%2F%20RTL8720DN%20SDK-blue)
![Hardware](https://img.shields.io/badge/Board-BW16%20(RTL8720DN)-green)
![Version](https://img.shields.io/badge/Version-1.0.0-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📋 Mục Lục
- [Thông Tin Các Phiên Bản](#-thông-tin-các-phiên-bản)
- [Thông Tin Kết Nối](#-thông-tin-kết-nối)
- [Tính Năng Nổi Bật](#-tính-năng-nổi-bật)
- [Thông Tin Phần Cứng & Sơ Đồ Chân](#-thông-tin-phần-cứng--sơ-đồ-chân)
- [Hướng Dẫn Biên Dịch & Nạp Code](#-hướng-dẫn-biên-dịch--nạp-code)
- [Ảnh Demo](#-ảnh-demo)
- [Tuyên Bố Miễn Trừ Trách Nhiệm (Disclaimer)](#-tuyên-bố-miễn-trừ-trách-nhiệm-disclaimer)
- [Giấy Phép (License)](#-giấy-phép-license)

---

## 🚀 Thông Tin Các Phiên Bản

### **Ver 1.0.0**
* **Giao diện Việt hóa:** Tối ưu khả năng quản lý và hiển thị thông tin các mạng WiFi được phát hiện xung quanh.
* **WiFi Dual Band:** Hỗ trợ quét đồng thời hai băng tần `2.4GHz` và `5GHz`, hiển thị đầy đủ tên WiFi (SSID), địa chỉ BSSID, kênh hoạt động và cường độ tín hiệu (RSSI).
* **Smart Pairing:** Tự động nhận diện và ghép cặp các mạng WiFi có cùng tên cơ sở nhưng phát trên hai băng tần khác nhau.
* **RSSI Distance:** Ước tính khoảng cách tương đối dựa trên cường độ tín hiệu WiFi để đánh giá độ mạnh/yếu.
* **LED Status Indicator:** Tối ưu hệ thống LED RGB thông báo trực quan 3 trạng thái hoạt động (Đỏ, Xanh dương, Xanh lá).
* **Web Interface:** Điều khiển trực tiếp qua trình duyệt trên điện thoại hoặc máy tính mà không cần cài đặt ứng dụng bên thứ ba.

> *Lưu ý: Thông tin phiên bản sẽ tiếp tục được cập nhật khi có những thay đổi mới trong mã nguồn.*

---

## 📶 Thông Tin Kết Nối

Sau khi cấp nguồn cho mạch **BW16**, thiết bị sẽ tự động phát một điểm truy cập WiFi (Access Point) riêng. Hãy kết nối vào mạng này theo thông tin dưới đây:

* **SSID:** `Deauther_2-4_5GHZ`
* **Password:** `123456789`
* **Địa chỉ IP:** `192.168.4.1`
* **Port:** `80`

Sau khi kết nối thành công, mở trình duyệt web và truy cập địa chỉ: **`http://192.168.4.1`**

---

## ✨ Tính Năng Nổi Bật

### 1. WiFi Scanner (Quét Mạng Băng Tần Kép)
Quét và liệt kê chi tiết toàn bộ các Access Point trong khu vực với các thông số:
* **SSID:** Tên mạng WiFi.
* **BSSID:** Địa chỉ MAC vật lý của thiết bị phát.
* **Channel:** Kênh tần số WiFi đang hoạt động.
* **RSSI:** Cường độ tín hiệu thu được (đơn vị `dBm`).
* **Distance:** Khoảng cách ước tính từ thiết bị tới nguồn phát dựa trên chỉ số RSSI.
* **Frequency:** Phân loại tự động băng tần `2.4GHz` hoặc `5GHz`.

### 2. Smart Pairing 2.4GHz / 5GHz
Hệ thống tự động nhận diện và liên kết các mạng WiFi thuộc cùng một router dựa trên tên gốc và các hậu tố phân biệt băng tần phổ biến như:
* `-2.4GHz` / `-5GHz`
* `-2.4G` / `-5G`
* `_2.4G` / `_5G`

### 3. Hệ Thống Chỉ Thị LED RGB
Mạch sử dụng đèn LED RGB tích hợp trên bo mạch BW16 để phản hồi trạng thái vật lý theo thời gian thực:

| Màu LED | Chân GPIO | Trạng thái hoạt động |
| :--- | :---: | :--- |
| 🔴 **Đỏ** | `PA12` | Hoạt động đặc biệt |
| 🔵 **Xanh dương** | `PA13` | Đang thực hiện quét WiFi |
| 🟢 **Xanh lá** | `PA14` | Trạng thái chờ (Idle) |

> **Lưu ý phần cứng:** Hệ thống LED trên BW16 hoạt động ở chế độ **Active LOW** (mức logic `LOW` sẽ bật LED và mức `HIGH` sẽ tắt LED).

### 4. Giao Diện Quản Lý Web
Giao diện thiết kế đáp ứng (Responsive), hiển thị tốt trên cả màn hình điện thoại và máy tính:
* Bảng danh sách mạng WiFi trực quan, dễ theo dõi.
* Hiển thị chi tiết BSSID, băng tần, kênh, RSSI và khoảng cách ước tính.
* Đồng bộ hiển thị trạng thái đèn LED ngay trên giao diện.
* Nút thao tác quét lại (Rescan) mạng WiFi nhanh chóng.

## 💻 Hướng Dẫn Biên Dịch & Nạp Code

1. **Chuẩn bị phần cứng:** Bo mạch **BW16** sử dụng chip **RTL8720DN** và cáp dữ liệu Micro-USB / Type-C (tùy phiên bản board).
2. **Cài đặt môi trường:** Tải và cài đặt **Arduino IDE**.
3. **Cài đặt SDK & Thư viện:** Thêm Board Manager URL của Realtek AmebaD (`RTL8720DN`) vào Arduino IDE và cài đặt phiên bản SDK tương thích.
4. **Mở mã nguồn:** Mở file `.ino` của dự án trong Arduino IDE.
5. **Kiểm tra cấu hình:** Đối chiếu lại định nghĩa chân LED (`PA12`, `PA13`, `PA14`) và thông số cấu hình WiFi AP trong code.
6. **Biên dịch & Nạp (Upload):** Chọn đúng Board **Ai-Thinker BW16 (RTL8720DN)**, chọn cổng COM tương ứng, đưa mạch về chế độ Upload (nếu cần) và nhấn **Upload**.

> **Lưu ý:** Cần sử dụng đúng phiên bản AmebaD SDK và các thư viện đi kèm theo yêu cầu của mã nguồn để tránh lỗi xung đột khi biên dịch.

---

## 📸 Ảnh Demo

đang cập nhật


```markdown
![Web Interface Demo](images/web-demo.png)
![Hardware Setup](images/bw16-led.png)
