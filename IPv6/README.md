# IPv6
* IPV6 đã được phát triển để thay thế IPV4 sắp hết địa chỉ.
* Mặc dù nó đã được khoảng gần 10 năm nhưng nó vẫn chưa được triển khai và hỗ trợ rộng rãi.
* Tất cả các máy tính và điện thoại di động hiện đại đều hỗ trợ cả IPv4 và IPv6, và nếu bạn nhìn vào địa chỉ IP của thiết bị, bạn có thể sẽ thấy cả hai.

## IPv6 Address
* Địa chỉ Ipv6 sử dụng 128 bit thay vì 32 bit trong IPv4.
* Địa chỉ IPv6 được viết bằng hệ thập lục phân, trái ngược với số thập phân có dấu chấm trong IPv4
* Được chia làm 8 octet, mỗi octet được biểu diễn bằng 4 ký tự thập lục phân</br>![Imgur](https://i.imgur.com/7hxXgzJ.png)
## Network And Node Addresses
* Trong IPv4, một địa chỉ được chia thành hai thành phần, một thành phần **Network** và một thành phần **Host**.
    * Điều này được thực hiện ban đầu bằng cách sử dụng các Address classes và sau đó sử dụng subnet mask.
* Trong IPv6 cũng làm như vậy. Bước đầu tiên là chia địa chỉ thành hai phần.
    * Địa chỉ được chia thành 2 đoạn 64 bit, 64 bit trên cùng là phần **Network** và 64 bit dưới là phần **Host**:</br>![Imgur](https://i.imgur.com/wZW9wY9.png)
* 64 bit trên được sử dụng để routing - định tuyến.
* 64 bit sau xác định địa chỉ của **interface** hoặc **host** và được lấy từ địa chỉ vật lý hoặc địa chỉ MAC thực sử dụng định dạng Số nhận dạng duy nhất mở rộng (EUI-64) của IEEE. 
* 64 bit phía trước, chúng ta có thể thấy rằng nó được chia thành 2 khối 48 và 16 bit tương ứng 16 bit phía dưới được sử dụng cho các mạng con trên mạng nội bộ và được kiểm soát bởi quản trị viên mạng Hoặc được gọi là **Subnet ID**.
    * **Subnet ID**: được sử dụng với chức năng miêu tả cấu trúc trang của mạng. Một IPv6 subnet có cấu trúc tương đương với một nhánh mạng đơn như subnet của IPv4.
* 48 bit trên được sử dụng cho các **global network addresses - địa chỉ mạng toàn cầu** và được sử dụng để định tuyến qua internet.</br>![Imgur](https://i.imgur.com/pvvnaL0.png)
## Loại địa chỉ và phạm vi
Địa chỉ IPv6 có ba loại:
* **Global Unicast Address**: Phạm vi Internet- được định tuyến trên Internet
* **Unique Local**: Phạm vi Mạng nội bộ hoặc VPN có thể định tuyến nội bộ, nhưng Không được định tuyến trên Internet
* **Link Local**: Phạm vi liên kết mạng- Không được định tuyến nội bộ hoặc bên ngoài.

![Imgur](https://i.imgur.com/JoHZfuN.png)
### Global and Public Addresses
Địa chỉ toàn cầu có thể định tuyến được trên internet và bắt đầu từ năm 2001:
* Các địa chỉ này được gọi là global **Unicast addresses - địa chỉ Unicast toàn cầu** và tương đương với **IP public - public addresses - địa chỉ công cộng** của mạng IPv4.
* Các cơ quan quản lý Internet phân bổ các khối địa chỉ cho các ISP, những người này sẽ phân bổ chúng cho khách hàng của họ

### Internal Addresses- Link Local and Unique Local
* Trong địa chỉ nội bộ IPv4 sử dụng các dải số dành riêng **10.0.0.0/8**, **172.16.0.0/12** và **192.168.0.0/16** và **169.254.0.0/16**.
* Các địa chỉ này không được định tuyến trên Internet và được dành riêng cho các mạng nội bộ.
* IPv6 cũng có hai loại địa chỉ Nội bộ.
    * Link Local
    * Unique Local
### Link Local
* Chúng được sử dụng bên trong mạng nội bộ và một lần nữa chúng không được định tuyến trên Internet.
* Nó tương đương với địa chỉ IPv4 **169.254.0.0/16** được cấp phát trên mạng IPv4 khi không tìm thấy máy chủ DHCP.
* Liên kết địa chỉ cục bộ bắt đầu bằng **fe80**
* **Link Local addresses** được tự chỉ định, tức là chúng không yêu cầu máy chủ DHCP.
* là bắt buộc trên mọi giao diện IP6 ngay cả khi không có định tuyến.
### Unique Local
* Unique Local được sử dụng trong mạng nội bộ.
* Chúng được định tuyến trên mạng Nội bộ nhưng không được định tuyến trên Internet.
* Chúng tương đương với các địa chỉ IPv4 là **10.0.0.0/8**, **172.16.0.0/12** và **192.168.0.0/16**
* Không gian địa chỉ được chia thành hai không gian /8: 
    * **fc00::/8** cho **globally assigned addressing** - địa chỉ được chỉ định toàn cục 
    * **fd00::/8** cho **locally assigned addressing** - địa chỉ được chỉ định cục bộ.
* Để được tổ chức chỉ định theo cách thủ công, hãy sử dụng tiền tố prefix **fd00**.
## Using IPv6 Addresses in URLs
Trên mạng IPv4, bạn có thể truy cập vào nguồn mạng, ví dụ: một trang web sử dụng định dạng
* `http://192.168.1.21/webpage`
Tuy nhiên, địa chỉ IPv6 chứa dấu hai chấm làm dấu phân cách và do đó phải được đặt trong dấu ngoặc vuông.
* http://[IPv6 address]/webpage.
## IPv6 Loop Back
Địa chỉ Loop Back IPv4 là `127.0.0.1`

Địa chỉ Loop Back IPv6 là `::1`. You can ping it as follows:</br>![Imgur](https://i.imgur.com/9tpdQvJ.png)
## 

* 
* 
* 





