RTL8720DN WiFi Scanner – BW16
Thông Tin Các Phiên Bản

Dưới đây là thông tin về các chức năng và những điểm nổi bật của phiên bản RTL8720DN WiFi Scanner dành cho bo mạch BW16 sử dụng chip RTL8720DN.

Nội Dung Cập Nhật
Ver 1.0.0: Phiên bản giao diện web được Việt hóa, tối ưu khả năng quản lý và hiển thị thông tin các mạng WiFi được phát hiện xung quanh.
WiFi Dual Band: Hỗ trợ quét các mạng WiFi thuộc hai băng tần 2.4GHz và 5GHz, hiển thị tên WiFi, địa chỉ BSSID, kênh hoạt động và cường độ tín hiệu RSSI.
Smart Pairing: Bổ sung khả năng nhận diện và ghép cặp các mạng WiFi có cùng tên cơ sở nhưng khác băng tần 2.4GHz và 5GHz.
RSSI Distance: Hiển thị khoảng cách ước tính từ cường độ tín hiệu WiFi, giúp người dùng tham khảo mức độ mạnh yếu của tín hiệu.
LED Status Indicator: Tối ưu hệ thống LED RGB với ba trạng thái hoạt động:
Đỏ: Trạng thái hoạt động đặc biệt.
Xanh dương: Đang quét WiFi.
Xanh lá: Trạng thái chờ.
Web Interface: Giao diện điều khiển trực tiếp thông qua trình duyệt điện thoại hoặc máy tính, không cần cài đặt ứng dụng bổ sung.
Lưu ý: Các thông tin phiên bản sẽ được cập nhật khi có những thay đổi mới trong source code.
Thông Tin Kết Nối

Sau khi cấp nguồn cho mạch BW16, thiết bị sẽ khởi tạo mạng WiFi riêng để người dùng kết nối và truy cập giao diện quản lý.

SSID: Deauther_2-4_5GHZ

PASSWORD: 123456789

IP: 192.168.4.1

PORT: 80

Sau khi kết nối WiFi của thiết bị, mở trình duyệt và nhập địa chỉ IP bên trên để truy cập giao diện web.

Giới Thiệu Chức Năng
1. WiFi Scanner

Chức năng quét và hiển thị những mạng WiFi được phát hiện trong khu vực.

Thông tin hiển thị bao gồm:

SSID: Tên mạng WiFi.
BSSID: Địa chỉ MAC của Access Point.
Channel: Kênh WiFi đang sử dụng.
RSSI: Cường độ tín hiệu WiFi (dBm).
Distance: Khoảng cách ước tính dựa trên RSSI.
Frequency: Nhận diện băng tần 2.4GHz hoặc 5GHz.
2. Smart Pairing 2.4GHz / 5GHz

Hệ thống có khả năng nhận diện các mạng WiFi có tên tương đồng và hậu tố phân biệt băng tần như:

2.4GHz
5GHz
2.4G
5G

Nhờ đó, người dùng có thể dễ dàng nhận biết những mạng có cùng tên cơ sở nhưng hoạt động trên hai băng tần khác nhau.

3. Hệ Thống LED RGB

Mạch sử dụng ba chân LED được cấu hình như sau:

Màu LED	Chân GPIO	Trạng thái
Đỏ	PA12	Hoạt động đặc biệt
Xanh dương	PA13	Đang quét WiFi
Xanh lá	PA14	Đang chờ

Lưu ý: LED sử dụng chế độ Active LOW, nghĩa là mức LOW sẽ bật LED và mức HIGH sẽ tắt LED.

4. Giao Diện Web

Giao diện được thiết kế thân thiện, tương thích với điện thoại và máy tính.

Các thành phần chính:

Bảng danh sách WiFi.
Thông tin địa chỉ BSSID.
Hiển thị băng tần và kênh hoạt động.
Cường độ tín hiệu RSSI.
Khoảng cách ước tính.
Trạng thái LED.
Chức năng quét lại mạng WiFi.
Thông Tin Phần Cứng
Thành phần	Thông số
Board	BW16
Chip	RTL8720DN
WiFi	2.4GHz / 5GHz
Web Server	Port 80
IP mặc định	192.168.4.1
LED Đỏ	PA12
LED Xanh dương	PA13
LED Xanh lá	PA14
Nguồn	Theo thông số bo mạch BW16
Hướng Dẫn Biên Dịch
Chuẩn bị bo mạch BW16 sử dụng chip RTL8720DN.
Cài đặt môi trường Arduino tương thích với RTL8720DN.
Cài đặt đầy đủ thư viện và SDK tương ứng.
Mở source code trong Arduino IDE.
Kiểm tra cấu hình chân LED và thông số WiFi.
Biên dịch và nạp firmware phù hợp với bo mạch.

Lưu ý: Cần sử dụng đúng SDK và thư viện tương thích với phiên bản RTL8720DN để tránh lỗi biên dịch.

Ảnh Demo

Có thể bổ sung hình ảnh giao diện web, bảng danh sách WiFi và trạng thái LED tại đây.

Tuyên Bố Miễn Trừ Trách Nhiệm
DISCLAIMER

Toàn bộ mã nguồn và tài liệu được chia sẻ nhằm mục đích học tập, nghiên cứu và thử nghiệm phần cứng trong môi trường được phép.

Người sử dụng có trách nhiệm đảm bảo mọi hoạt động thử nghiệm đều được thực hiện trên thiết bị và hệ thống thuộc quyền sở hữu hoặc đã được chủ sở hữu cho phép.

Không sử dụng thiết bị hoặc mã nguồn để gây gián đoạn kết nối, can thiệp trái phép vào hệ thống mạng, ảnh hưởng đến quyền riêng tư hoặc gây thiệt hại cho cá nhân và tổ chức khác.

Tác giả không khuyến khích các hành vi sử dụng sai mục đích. Người sử dụng phải tự chịu trách nhiệm đối với hoạt động của mình và tuân thủ pháp luật hiện hành.

Hãy sử dụng công nghệ một cách có trách nhiệm!

Project: RTL8720DN – BW16

Platform: Arduino / RTL8720DN SDK

Development: Community Project

License: Bổ sung giấy phép phù hợp khi công bố dự án.
