# 📡 RTL8720DN Deauther – BW16

Code deauther này hỗ trợ phá sóng (2.4GHz & 5GHz) chạy trên bo mạch **BW16 (chip RTL8720DN)**, 

![Platform](https://img.shields.io/badge/Platform-Arduino%20%2F%20RTL8720DN%20SDK-blue)
![Hardware](https://img.shields.io/badge/Board-BW16%20(RTL8720DN)-green)
![Version](https://img.shields.io/badge/Version-x.x.x-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

* **Link sản phẩm:**
* **Esp32 có anten:** [Nhấn vào để mua](https://hoantien.vn/go/CWZw07XYms9)
* **Esp32 không anten:** [Nhấn vào để mua](https://hoantien.vn/go/CWZw07XYms9)

---

## 🚀 Thông Tin Các Phiên Bản
**Ver 1.0.0:**
* **Giao diện Việt hóa:** Tối ưu khả năng quản lý và hiển thị thông tin các mạng WiFi được phát hiện xung quanh.
* **WiFi Dual Band:** Hỗ trợ quét hai băng tần `2.4GHz` và `5GHz`, hiển thị đầy đủ tên WiFi (SSID), địa chỉ BSSID, kênh hoạt động và cường độ tín hiệu (RSSI).
* **Smart Pairing:** Tự động nhận diện và ghép cặp các mạng WiFi có cùng tên cơ sở nhưng phát trên hai băng tần khác nhau.
* **RSSI Distance:** Ước tính khoảng cách tương đối dựa trên cường độ tín hiệu WiFi để đánh giá độ mạnh/yếu.
* **Set Time Stop Attack:** Tính năng thiết lập thời gian dừng hoạt động.
* **Mod:** Hỗ trợ các chế độ Deauther và Beacon phục vụ thử nghiệm bảo mật WiFi trong môi trường được phép.
* **Web Interface:** Điều khiển trực tiếp qua trình duyệt trên điện thoại hoặc máy tính mà không cần cài đặt ứng dụng bên thứ ba.

**Ver 1.2.0:**
* **Tối ưu code:** Code được tối ưu lại
* **Cho phép theo ý muốn cấu hình:** Từ phiên bản này cho phép bạn thay ssid và pass theo ý muốn hoặc có thể dùng cấu hình mặt định nếu muốn

> *Lưu ý: Thông tin phiên bản sẽ tiếp tục được cập nhật khi có những thay đổi mới trong mã nguồn.*

---


**Hỗ trợ nếu không thể nạp code**

**Liên Hệ Với Mình Qua:** 
- Telegram: [@quangapi](https://t.me/quangapi)

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

### 1. WiFi Scanner – Quét Mạng Băng Tần Kép

Hỗ trợ quét và hiển thị thông tin các mạng WiFi xung quanh trên cả hai băng tần `2.4GHz` và `5GHz`, bao gồm:

* **SSID:** Tên mạng WiFi.
* **BSSID:** Địa chỉ MAC của thiết bị phát.
* **Channel:** Kênh WiFi đang hoạt động.
* **RSSI:** Cường độ tín hiệu thu được (dBm).
* **Distance:** Ước tính khoảng cách tương đối dựa trên cường độ tín hiệu.
* **Frequency:** Tự động phân loại băng tần `2.4GHz` hoặc `5GHz`.

### 2. Smart Pairing – Tự Động Ghép Cặp WiFi

Tự động nhận diện và ghép cặp các mạng WiFi có cùng tên cơ sở nhưng hoạt động trên hai băng tần khác nhau.

Hỗ trợ nhận diện các hậu tố phổ biến:

* `-2.4GHz` / `-5GHz`
* `-2.4G` / `-5G`
* `_2.4G` / `_5G`

### 3. RSSI Distance – Ước Tính Khoảng Cách

Phân tích cường độ tín hiệu WiFi (RSSI) để đưa ra khoảng cách tương đối giữa thiết bị BW16 và nguồn phát.

Tính năng giúp người dùng đánh giá:

* Mức độ mạnh hoặc yếu của tín hiệu WiFi.
* Khoảng cách tương đối giữa thiết bị quét và Access Point.
* So sánh cường độ tín hiệu giữa các mạng được phát hiện.

> *Lưu ý: Khoảng cách chỉ mang tính ước tính, không phải kết quả đo vị trí chính xác.*

### 4. Set Time Stop Attack – Thiết Lập Thời Gian Dừng

Cho phép cấu hình thời gian hoạt động và thời điểm dừng của chế độ kiểm thử, giúp quản lý thời lượng hoạt động của thiết bị.

### 5. Mod – Deauther & Beacon

Hỗ trợ các chế độ hoạt động:

* **Deauther:** Phá sóng wifi xung quanh nó phát hiện 
* **Beacon:** Chế độ phát tín hiệu Beacon spam ssid wifi

### 6. Web Interface – Giao Diện Quản Lý Web

Điều khiển và theo dõi thiết bị trực tiếp thông qua trình duyệt trên điện thoại hoặc máy tính, không cần cài đặt ứng dụng bên thứ ba.

Các chức năng giao diện bao gồm:

* Hiển thị danh sách mạng WiFi được phát hiện.
* Theo dõi SSID, BSSID, băng tần, kênh, RSSI và khoảng cách ước tính.
* Hiển thị trạng thái đèn LED trực tiếp trên giao diện.
* Phá sóng wifi và spam beacon
* Nút **Rescan** giúp quét lại các mạng WiFi xung quanh nhanh chóng.

---

## 💻 Hướng Dẫn & Nạp Code

- Video: [https://www.youtube.com/embed/y3lydWgAuYs](https://www.youtube.com/embed/y3lydWgAuYs)

**Nếu lỗi hãy thử install board package trên arduino**

```
https://github.com/ambiot/ambd_arduino/raw/master/Arduino_package/package_realtek_amebad_index.json
```
---

## 📸 Ảnh Demo
<table>
  <tr>
    <td>
      <img src="https://chodev.pro/images/1b111422-2916-46c7-8f07-216ff73f4d59.webp" width="400" alt="Ảnh 1">
    </td>
    <td>
      <img src="https://chodev.pro/images/a5778d78-cdfe-4607-b3a3-2d455730e28e.webp" width="400" alt="Ảnh 2">
    </td>
  </tr>
</table>


> [!CAUTION]
**Tuyên bố miễn trừ trách nhiệm pháp lý**<br/><br/>
``Tất cả các thông tin, hướng dẫn, mã nguồn, video hoặc bất kỳ nội dung nào được chia sẻ tại đây hoàn toàn mang mục đích học tập, nghiên cứu và phục vụ cho việc nâng cao kiến thức cá nhân. Tôi không khuyến khích, không xúi giục, và cũng không chịu trách nhiệm đối với bất kỳ hành vi sử dụng nội dung nào từ đây cho mục đích trái pháp luật, phá hoại, gây rối, trục lợi cá nhân, hoặc làm ảnh hưởng tiêu cực đến bất kỳ cá nhân, tổ chức hay tập thể nào tại Việt Nam hoặc bất kỳ quốc gia nào khác.``<br/><br/>
``Việc người dùng tự ý sử dụng các nội dung được cung cấp vào các hoạt động vi phạm pháp luật, gây thiệt hại tài sản, xâm phạm quyền riêng tư, an toàn thông tin, trật tự xã hội… là hoàn toàn nằm ngoài tầm kiểm soát và ý chí của tôi. Tôi không chịu bất kỳ trách nhiệm nào về mặt pháp lý, dân sự hay hình sự, cũng như không có bất kỳ liên quan, liên đới nào dưới bất kỳ hình thức nào đối với hậu quả từ những hành vi đó.``<br/><br/>
``Người sử dụng nội dung cần tự ý thức, tự chịu trách nhiệm trước pháp luật và hoàn toàn tự chịu hậu quả nếu sử dụng nội dung sai mục đích. Tôi khuyến khích mọi người tuân thủ pháp luật, sử dụng nội dung một cách có đạo đức và đúng đắn trong khuôn khổ pháp luật cho phép!``

[![Featured on Chợ Dev](https://chodev.pro/api/badges/deauther-rtl8720dn-bw16?theme=light)](https://chodev.pro/p/deauther-rtl8720dn-bw16)
