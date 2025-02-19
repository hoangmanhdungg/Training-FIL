- [Network](#network)
  - [1.Các loại mạng](#1các-loại-mạng)
  - [2.Truyền dữ liệu](#2truyền-dữ-liệu)
    - [2.1.Phân loại dữ liệu](#21phân-loại-dữ-liệu)
    - [2.2.Phương pháp truyền tín hiệu](#22phương-pháp-truyền-tín-hiệu)
  - [3.Băng thông và thông lượng](#3băng-thông-và-thông-lượng)
    - [3.1.Băng thông](#31băng-thông)
    - [3.2.Thông lượng](#32thông-lượng)
  - [4.Máy khách và máy chủ (Client and Server)](#4máy-khách-và-máy-chủ-client-and-server)
    - [4.1.Client](#41client)
    - [4.2.Server](#42server)
    - [4.3.Mạng P2P](#43mạng-p2p)
  - [5.Cơ sở hạ tầng mạng](#5cơ-sở-hạ-tầng-mạng)
    - [5.1.Thiết bị đầu cuối](#51thiết-bị-đầu-cuối)
    - [5.2.Thiết bị trung gian](#52thiết-bị-trung-gian)
    - [5.3.Phương tiện truyền dẫn](#53phương-tiện-truyền-dẫn)
  - [6.Kết nối ISP](#6kết-nối-isp)
  - [7.Mạng không dây và di động](#7mạng-không-dây-và-di-động)
    - [7.1.Máy phát và thu GMS, mạng 4G/5G](#71máy-phát-và-thu-gms-mạng-4g5g)
    - [7.2.GPS](#72gps)
    - [7.3.Wifi](#73wifi)
    - [7.4.Bluetooth](#74bluetooth)
    - [7.5.NFC](#75nfc)
# Network
## 1.Các loại mạng
- Internet là tập hợp các mạng lưới được kết nối trên toàn thế giới, hợp tác với nhau và trao đổi thông tin bằng các tiêu chuẩn chung 
- Các loại mạng: 
  Mạng gia đình < Mạng văn phòng nhỏ < Mạng vừa và lớn < Mạng toàn cầu.
## 2.Truyền dữ liệu 
### 2.1.Phân loại dữ liệu
- Dữ liệu tự nguyện: Được tạo và chia sẻ rõ ràng bởi các các nhân 
- Dữ liệu quan sát: Thu thập bằng cách ghi lại hành động của các nhân
- Dữ liệu suy luận: Có được dựa trên phân tích dữ liệu tự nguyện hoặc quan sát
### 2.2.Phương pháp truyền tín hiệu
- Tín hiệu điện: Truyền tải được thực hiện bằng cách biểu diễn dữ liệu dưới dạng xung điện
- Tín hiệu quang: Truyền dẫn được thực hiện bằng cách chuyển đổi tín hiệu thành xung ánh sáng
- Tín hiệu không dây: Truyền tín hiệu bằng cách sử dụng sóng hồng ngoại, sóng vi ba hoặc sóng vô tuyến
## 3.Băng thông và thông lượng
### 3.1.Băng thông
- Là khả năng của một phương tiện truyền dữ liệu. Băng thông thường được đo bằng số bit có thể được gửi qua phương tiện trong một giây.
- + Kbps: Nghìn bit mỗi giây
- + Mbps: Triệu bit mỗi giây
- + Gbps: Tỷ bit mỗi giây
### 3.2.Thông lượng
- Lượng dữ liệu thực tế mà có thể truyền tại một thời điểm bất kì
- Do nhiều yếu tố ảnh hưởng như đỗ trễ hoặc lượng dữ liệu được gửi và nhận qua kết nối
## 4.Máy khách và máy chủ (Client and Server)
- Tất cả các máy tính được kết nối với mạng tham gia trực tiếp vào giao tiếp mạng được phân loại là host
- Phần mềm được cài đặt trên máy tính sẽ xác định vai trò của nó
### 4.1.Client
- Là host có cài đặt phần mềm cho phép host yêu cầu và hiển thị thông tin thu được từ server
### 4.2.Server
- Là host được cài đặt phần mềm cho phép chúng cung cấp thông tin như email hoặc trang web cho các host khác trên mạng
### 4.3.Mạng P2P
- Mạng mà tại đó nhiều máy hoạt động như cả máy chủ và máy khách 
## 5.Cơ sở hạ tầng mạng
- Là nền tảng hỗ trợ mạng, cung cấp kênh ổn định và đáng tin cậy để chúng ta có thể truyền thông 
- Gồm 3 thành phần: thiết bị đầu cuối, thiết bị trung gian và mạng lưới truyền thông
  ![Cơ sở hạ tầng mạng](https://github.com/hoangmanhdungg/Training-FIL/blob/Networking-Basic/image/Screenshot%202025-02-17%20214221.png?raw=true)
### 5.1.Thiết bị đầu cuối
- Là nguồn hoặc đích của tin nhắn truyền qua mạng
- VD: máy tính, máy in, điện thoại, thiết bị di động,...
### 5.2.Thiết bị trung gian
- Đảm bảo dữ liệu đến đúng đích
- VD: router, switch, firewall,....
### 5.3.Phương tiện truyền dẫn
- Đường dẫn để truyền dữ liệu 
- VD: Cáp đồng, cáp quang, wi-fi,...
## 6.Kết nối ISP
- ISP cung cấp liên kết giữa mạng gia đình và internet. ISP có thể là nhà cung cấp cáp địa phương, nhà cung cấp dịch vụ điện thoại cố định, mạng di động cung cấp dịch vụ điện thoại thông minh của bạn hoặc nhà cung cấp độc lập cho thuê băng thông trên cơ sở hạ tầng mạng vật lý của một công ty khác.
- Sự kết nối giữa các ISP tạo thành xương sống của Internet là một mạng lưới phức tạp gồm các cáp quang với các bộ định tuyến và bộ chuyển mạch mạng đắt tiền giúp định hướng luồng thông tin giữa máy chủ nguồn và máy chủ đích.
## 7.Mạng không dây và di động 
### 7.1.Máy phát và thu GMS, mạng 4G/5G
- Điện thoại di động sử dụng sóng vô tuyến để truyền tín hiệu thoại đến các ăng-ten gắn trên các tháp nằm ở các khu vực địa lý cụ thể. Khi thực hiện cuộc gọi điện thoại, tín hiệu thoại được chuyển tiếp từ tháp này sang tháp khác cho đến khi được truyền đến đích. Loại mạng này được sử dụng khi bạn gọi điện đến một điện thoại di động khác hoặc đến một điện thoại có dây. 
- Loại mạng điện thoại di động phổ biến nhất được gọi là mạng GSM. Các chữ viết tắt 3G, 4G, 4G-LTE và 5G được sử dụng để mô tả các mạng điện thoại di động nâng cao được tối ưu hóa để truyền dữ liệu nhanh.
### 7.2.GPS
- GPS sử dụng vệ tinh để truyền tín hiệu bao phủ toàn cầu. Điện thoại thông minh có thể nhận các tín hiệu này và tính toán vị trí của điện thoại với độ chính xác trong vòng 10 mét.
### 7.3.Wifi
- Bộ phát và thu Wi-Fi nằm trong điện thoại thông minh cho phép điện thoại kết nối với mạng cục bộ và internet. Để nhận và gửi dữ liệu trên mạng Wi-Fi, điện thoại cần nằm trong phạm vi tín hiệu từ điểm truy cập mạng không dây. Mạng Wi-Fi thường là của tư nhân nhưng thường cung cấp điểm truy cập công cộng hoặc dành cho khách. Điểm truy cập là khu vực có tín hiệu Wi-Fi. Kết nối mạng Wi-Fi trên điện thoại tương tự như kết nối mạng trên máy tính xách tay.
### 7.4.Bluetooth
- Bluetooth là công nghệ không dây công suất thấp, phạm vi ngắn hơn, được thiết kế để thay thế kết nối có dây cho các phụ kiện như loa, tai nghe và micrô. Bluetooth cũng có thể được sử dụng để kết nối đồng hồ thông minh với điện thoại thông minh. Vì công nghệ Bluetooth có thể được sử dụng để truyền cả dữ liệu và giọng nói, nên nó có thể được sử dụng để tạo các mạng cục bộ nhỏ. Bluetooth là công nghệ không dây cho phép các thiết bị giao tiếp trong khoảng cách ngắn. Nhiều thiết bị có thể được kết nối cùng lúc với Bluetooth.
### 7.5.NFC
- Giao tiếp trường gần (NFC) là công nghệ giao tiếp không dây cho phép dữ liệu được trao đổi giữa các thiết bị ở rất gần nhau, thường là dưới vài cm. Ví dụ, NFC có thể được sử dụng để kết nối điện thoại thông minh và hệ thống thanh toán. NFC sử dụng trường điện từ để truyền dữ liệu.