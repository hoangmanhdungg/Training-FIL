# IPv4 và IPv6
## 1.IPv4
### 1.1.Mục đích của IPv4
- Địa chỉ IPv4 là địa chỉ mạng logic xác định một máy chủ cụ thể. Địa chỉ này phải được cấu hình đúng và duy nhất trong mạng LAN để giao tiếp cục bộ. Địa chỉ này cũng phải được cấu hình đúng và duy nhất trên thế giới để giao tiếp từ xa.
- Mỗi gói tin được gửi qua internet đều có địa chỉ IPv4 nguồn và đích. Thông tin này được các thiết bị mạng yêu cầu để đảm bảo thông tin đến được đích và mọi phản hồi đều được trả về nguồn.
### 1.2.Cấu trúc địa chỉ IPv4
- Địa chỉ IP gồm 32 bit nhị phân chia thành 4 cụm 8 bit ( gọi là các octet ). Các octet được biểu diễn dưới dạng thập phân và được ngăn cách nhau bằng dấu chấm.
- Địa chỉ IP được ngăn cách thành 2 phần là phần host và phần network.
![Cấu trúc địa chỉ IP](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-18%20231400.png?raw=true)
### 1.3.Quy tắc đặt địa chỉ IP
- Các bit phần mạng không được đồng thời bằng không (VD: 0.0.0.1 với phần mạng là 0.0.0 và phần host là 1 là không hợp lệ).
- Nếu các bit phần host đồng thời bằng 0 ta có một địa chỉ mạng.
- Nếu các bit phần host đồng thời bằng 1 ta có địa chỉ broadcast.
### 1.4.IPv4 Unicast, Broadcast and Multicast
- Unicast: giao tiếp 1 - 1, 1 thiết bị gửi tin tới một thiết bị khác.
![Hình ảnh minh họa Unicast](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-18%20233249.png?raw=true)
- Broadcast: 1 - tất cả, 1 thiết bị gửi tin tới tất cả thiết bị trong mạng.
![Hình ảnh minh họa Broadcast](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-18%20233315.png?raw=true)
- Multicast: cho phép host gửi tin tới một tập hợp host được chọn(multicast group).
![Hình ảnh minh họa Multicast](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-18%20233301.png?raw=true)
### 1.5.Các kiểu địa chỉ IPv4
- Bao gồm public và private
- + Private: mạng nội bộ, lặp đi lặp lại trong các mạng LAN khác nhau.
- + Public: sử dụng cho các gói tin đi trên 1 trường internet. Là địa chỉ duy nhất cho mỗi gói tin tham gia vào internet.
- Để gói tin từ mạng nội bộ tham gia vào internet, ta phải sử dụng phương pháp NAT để chuyển đổi địa chỉ IP từ private sang public.
- Dải địa chỉ IPv4 private:
![Hình ảnh bảng địa chỉ IPv4 private](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-18%20234339.png?raw=true)
- Nằm ngoài dải trên thì là địa chỉ public.
### 1.6.Địa chỉ các lớp kế thừa
#### 1.6.1.Lớp A
- 1 octet đầu làm phần mạng, 3  octet sau làm phần host
- Bit đầu của 1 địa chỉ lớp A luôn giữ là 0. Do đó lớp A: 1.0.0.0 - 127.0.0.0
- Tuy nhiên 127.0.0.0 thường là địa chỉ loopback nên địa chỉ mạng lớp A gồm 1.0.0.0 - 126.0.0.0
![Hình ảnh địa chỉ lớp A](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-19%20154454.png?raw=true)
#### 1.6.2.Lớp B
- 2 octet đầu làm phần mạng, 2 octet sau làm phần host
- 2 bit đầu luôn là 10 => địa chỉ lớp B: 128.0.0.0 - 191.255.0.0
![Hình ảnh địa chỉ lớp B](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-19%20154607.png?raw=true)
#### 1.6.3.Lớp C
- 3 octet đầu làm phần mạng, 1 octet cuối làm phần host
- 3 bit đầu luôn là 110 -> địa chỉ lớp C: 192.0.0.0 -> 223.255.255.0
![Hình ảnh địa chỉ lớp C](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-19%20154511.png?raw=true)
#### 1.6.4.Lớp D
- Được dùng làm địa chỉ multicast
- Dải địa chỉ: 224.0.0.0 - 239.255.255.255
#### 1.6.5.Lớp E
- Dùng để dự phòng
- 240.0.0.0 trở đi
#### 1.6.6.Chú ý
- Các địa chỉ IP có thể sử dụng để đặt cho các host là A,B,C
- Dể thuận tiện cho việc nhận diện 1 địa chỉ IP thuộc lớp nào, ta quan sát octet đầu của địa chỉ: 
- + 1->126: class A
- + 128->191: class B
- + 192->223: class C
- + 224->239: class D
- + 240->255: class E
### 1.7.Địa chỉ IPv4 sử dụng đặc biệt 
- Địa chỉ vòng lặp: 127.0.0.0/8 được máy chủ sử dụng để chuyển hướng lưu lượng đến chính nó 
- Địa chỉ liên kết cục bộ (169.254.0.0 /16 hoặc 169.254.0.1 đến 169.254.255.254) thường được gọi là địa chỉ Địa chỉ IP Riêng tư Tự động (APIPA) hoặc địa chỉ tự gán. Chúng được máy khách Windows sử dụng để tự cấu hình trong trường hợp máy khách không thể lấy được địa chỉ IP thông qua các phương pháp khác. Địa chỉ liên kết cục bộ có thể được sử dụng trong kết nối ngang hàng nhưng không thường được sử dụng cho mục đích này.
### 1.8.Subnet và số prefix
- Subnet mask là 1 dải 32 bit nhị phân đi kèm 1 địa chỉ IP, được các host sử dụng để xác định địa chỉ mạng của IP này thông qua toán tử "AND"
- Số prefix: thể hiện 1 cách đoen giản số bit mạng trong địa chỉ IP
- Nguyên lý cơ bản của việc chia mạng con: mượn bit host để tạo thêm các mạng con
- Chia mạng con làm giảm lưu lượng mạng tổng thể và cải thiện hiệu suất mạng. Nó cũng cho phép người quản trị triển khai các chính sách bảo mật như mạng con nào được phép hoặc không được phép giao tiếp với nhau. Một lý do khác là nó làm giảm số lượng thiết bị bị ảnh hưởng bởi lưu lượng phát sóng bất thường do cấu hình sai, sự cố phần cứng/phần mềm hoặc ý định xấu
- Các ví dụ về cách chia mạng con:
![Hình ảnh phân mạng theo vị trí](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-20%20232103.png?raw=true)
![Hình ảnh phân mạng theo nhóm hoặc chức năng](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-20%20232113.png?raw=true)
![Hình ảnh phân mạng theo loại thiết bị](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-20%20232124.png?raw=true)
## 2.IPv6
### 2.1.Vấn đề của IPv4 và nhu cầu của IPv6
- IPv4 đang dần cạn kiệt địa chỉ => IPv6 được thiết kế để trở thành phiên bản kế nhiệm của IPv4.
- IPv6 có không gian địa chỉ 128 bit lớn hơn.
- IPv4 có tối đa lý thuyết là 4,3 tỷ địa chỉ. Địa chỉ riêng kết hợp với Dịch địa chỉ mạng (NAT) đã đóng vai trò quan trọng trong việc làm chậm quá trình cạn kiệt không gian địa chỉ IPv4. Tuy nhiên, NAT gây ra vấn đề cho nhiều ứng dụng, tạo ra độ trễ và có những hạn chế cản trở nghiêm trọng đến giao tiếp ngang hàng.
- Sự ra đời của IoT cũng khiến không gian địa chỉ IPv4 càng thêm hạn chế
### 2.2.Sự đồng tồn tại của IPv4 và IPv6
#### 2.2.1.Cơ chế Duel Stack
- Dual stack cho phép IPv4 và IPv6 cùng tồn tại trên cùng một phân đoạn mạng. Thiết bị Dual stack chạy cả hai ngăn xếp giao thức IPv4 và IPv6 cùng lúc. Được gọi là IPv6 gốc, điều này có nghĩa là mạng của khách hàng có kết nối IPv6 với ISP của họ và có thể truy cập nội dung tìm thấy trên internet qua IPv6.
![Hình ảnh cơ chế Duel Stack](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-21%20224508.png?raw=true)
### 2.2.2.Cơ chế đào hầm
- Đường hầm là phương pháp vận chuyển gói tin IPv6 qua mạng IPv4. Gói tin IPv6 được đóng gói bên trong gói tin IPv4, tương tự như các loại dữ liệu khác.
![Hình ảnh cơ chế Đào Hầm ](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-21%20224518.png?raw=true)
### 2.2.3.Bản dịch
- Network Address Translation 64 (NAT64) cho phép các thiết bị hỗ trợ IPv6 giao tiếp với các thiết bị hỗ trợ IPv4 bằng kỹ thuật dịch tương tự như NAT cho IPv4. Một gói tin IPv6 được dịch thành một gói tin IPv4 và một gói tin IPv4 được dịch thành một gói tin IPv6.
![Hình ảnh cơ chế Đào Hầm ](https://github.com/hoangmanhdungg/Training-FIL/blob/main/images/Screenshot%202025-02-21%20224526.png?raw=true)
## 2.3.Địa chỉ IPv6
### 2.3.1.
