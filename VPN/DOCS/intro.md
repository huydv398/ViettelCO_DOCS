# WHAT IS VPN?

1. [VPN là gì?](#1-vpn-là-gì)
2. [VPN hoạt động như thế nào?](#2-vpn-hoạt-động-như-thế-nào)
* [Lợi ích.](#lợi-ích)
* [Encryption tunnel hoạt động như thế nào?](#encryption-tunnel--mã-hóa-tunnel-hoạt-động-như-thế-nào)
3. [Có những loại VPN nào?](#3-có-những-loại-vpn-nào)
* [Site-to-site VPN](#site-to-site-vpn)
* [Client-to-Server VPN](#client-to-server-vpn)
4. [Tại sao sử dụng VPN?](#4-tại-sao-sử-dụng-vpn)
4. [Các lợi ích bổ sung của VPN](#5-các-lợi-ích-bổ-sung-của-vpn)
4. [VPN disadvantages - Nhược điểm của VPN](#6-vpn-disadvantages)
4. [Có thể sử dụng VPN trên thiết bị nào?](#7-có-thể-sử-dụng-vpn-trên-thiết-bị-nào)
4. [Các yếu tố cần đánh giá khi chọn VPN?](#8-các-yếu-tố-cần-đánh-giá-khi-chọn-vpn)
## 1. VPN là gì?
* Mạng riêng ảo (Virtual private network)
* Thiết lập kết nối mạng được bảo vệ khi sử dụng public networks
* VPN mã hóa lưu lượng truy cập internet của bạn và che giấu danh tính trực tuyến của bạn. Quá trình mã hóa diễn ra trong thời gian thực.
* Tránh bên thứ ba theo dõi các hoạt động của bạn trực tuyến và đánh cắp dữ liệu hơn. 
## 2. VPN hoạt động như thế nào?
![](/VPN/image/Screenshot_1.png)
* Định tuyến kết nối internet của thiết bị của bạn thông qua Máy chủ VPN mà bạn đã chọn thay vì nhà cung cấp dịch vụ internet (ISP) để khi dữ liệu của bạn được truyền tới internet.</br>![](/VPN/image/Screenshot_2.png)</br>client sẽ thông qua VPN để lấy thông tin từ Website chứ không đi thẳng đến Website để lấy thông tin. và ngược lại.
* Dữ liệu của bạn bị chặn bằng cách nào đó, nó sẽ không thể đọc được cho đến khi đến đích cuối cùng.
* VPN tạo một “đường hầm” riêng tư từ thiết bị của bạn tới Internet và ẩn dữ liệu quan trọng của bạn thông qua một thứ được gọi là mã hóa.


VPN ẩn địa chỉ IP của bạn bằng cách cho phép mạng chuyển hướng nó thông qua một máy chủ từ xa được cấu hình đặc biệt do máy chủ VPN chạy. Điều này có nghĩa là nếu bạn lướt web trực tuyến bằng VPN, máy chủ VPN sẽ trở thành nguồn dữ liệu của bạn. Điều này có nghĩa là Nhà cung cấp dịch vụ Internet (ISP) của bạn và các bên thứ ba khác không thể xem trang web nào bạn truy cập hoặc dữ liệu nào bạn gửi và nhận trực tuyến. VPN hoạt động giống như một bộ lọc biến tất cả dữ liệu của bạn thành "vô nghĩa". Ngay cả khi ai đó có được trong tay dữ liệu của bạn, nó sẽ vô ích.

Cách VPN hoạt động

Định tuyến kết nối internet của thiết bị của bạn thông qua Máy chủ VPN mà bạn đã chọn thay vì nhà cung cấp dịch vụ internet (ISP) để khi dữ liệu của bạn được truyền tới internet.

dữ liệu đó đến từ VPN chứ không phải từ máy tính của bạn. VPN hoạt động như một trung gian khi bạn kết nối với internet, do đó ẩn địa chỉ IP của bạn - chuỗi số mà ISP gán cho thiết bị của bạn - và bảo vệ danh tính của bạn. Hơn nữa, nếu dữ liệu của bạn bị chặn bằng cách nào đó, nó sẽ không thể đọc được cho đến khi đến đích cuối cùng.

VPN tạo một "tunnel" riêng tư từ thiết bị của bạn tới Internet và ẩn dữ liệu quan trọng của bạn thông qua một thứ được gọi là mã hóa.

### Lợi ích.
* **MÃ HÓA**: Để đọc dữ liệu, bạn cần có khóa encryption key - key mã hóa. Nếu không có nó, máy tính sẽ mất hàng triệu năm để giải mã trong trường hợp bị tấn công brute force. Với sự trợ giúp của VPN, các hoạt động trực tuyến của bạn được ẩn ngay cả trên các mạng công cộng.
* **Ngụy trang nơi truy cập của bạn**: Máy chủ VPN về cơ bản hoạt động như proxy của bạn trên internet. Các dịch vụ VPN không lưu trữ nhật ký các hoạt động của bạn. Mặt khác, một số nhà cung cấp ghi lại hành vi của bạn, nhưng không chuyển thông tin này cho các bên thứ ba. Điều này có nghĩa là bất kỳ hồ sơ tiềm năng nào về hành vi người dùng của bạn vẫn bị ẩn vĩnh viễn.
* **Secure data transfer - Truyền dữ liệu an toàn**: Nếu bạn làm việc từ xa, bạn có thể cần truy cập các tệp quan trọng trên mạng của công ty mình. Vì lý do bảo mật, loại thông tin này yêu cầu kết nối an toàn. Để có quyền truy cập vào mạng, kết nối VPN thường được yêu cầu. Dịch vụ VPN kết nối với các máy chủ riêng và sử dụng các phương pháp mã hóa để giảm nguy cơ rò rỉ dữ liệu.
### Encryption tunnel- Mã hóa tunnel hoạt động như thế nào?
Encryption là một phương pháp thay đổi văn bản bình thường thành một Chuỗi mã không thể đọc được. Một key hoặc decryptor-trình giải mã, giải mã văn bản và hiển thị văn bản trở lại thành thông tin có thể đọc được. Khi bạn sử dụng VPN, chỉ thiết bị của bạn và nhà cung cấp VPN mới chứa decryption key-khóa giải mã. Bất kỳ ai khác cố gắng theo dõi bạn sẽ chỉ thấy một mớ hỗn độn của các ký tự. Không có decryption key thì không giải mã thành văn bản có nghĩa được.
## 3. Có những loại VPN nào?
Có 2 loại cơ bản
* Site-to-site VPN
* Client-to-site VPN

Có một số giao thức VPN hoặc phương pháp bảo mật. Cũ nhất là PPTP, point-to-point tunneling protocol, vẫn còn được sử dụng cho đến ngày nay nhưng được nhiều người coi là một trong những giao thức kém an toàn nhất. Những thứ khác là IKEv2, L2TP/IPSec, SSL, TLS, SSH và OpenVPN. Là một giao thức mã nguồn mở, OpenVPN là một trong những giao thức an toàn nhất vì bất kỳ lỗ hổng nào trong lập trình của nó sẽ nhanh chóng được chú ý và vá.
### Site-to-site VPN
![](/VPN/image/Screenshot_3.png)

VPN phải được cài đặt ở 2 đầu kết nối.

VPN site-to-site về cơ bản là **private network - một mạng riêng** được thiết kế để ẩn các mạng nội bộ riêng và cho phép người dùng của các mạng an toàn này truy cập tài nguyên của nhau.


Còn được gọi là router-to-router VPN. Loại VPN này chủ yếu được sử dụng trong môi trường doanh nghiệp, cụ thể là khi doanh nghiệp có trụ sở chính ở một số địa điểm khác nhau. VPN site-to-site tạo ra một mạng nội bộ khép kín, nơi các vị trí khác nhau đều có thể kết nối với nhau. Đây được gọi là mạng nội bộ.

VPN site-to-site hữu ích nếu bạn có nhiều địa điểm trong công ty của mình, mỗi địa điểm có mạng cục bộ (LAN) riêng được kết nối với WAN (Mạng diện rộng). VPN site-to-site cũng hữu ích nếu bạn có hai mạng nội bộ riêng biệt mà bạn muốn gửi tệp mà không có người dùng từ một mạng nội bộ truy cập rõ ràng vào mạng kia.

VPN site-to-site chủ yếu được sử dụng trong các công ty lớn. Chúng rất phức tạp để triển khai và không mang lại tính linh hoạt như SSL VPN. Tuy nhiên, chúng là cách hiệu quả nhất để đảm bảo thông tin liên lạc trong và giữa các phòng ban lớn.
### Client-to-Server VPN
![](/VPN/image/Screenshot_4.png)
VPN được cài phía server. Và phía người dùng phải được cài đặt VPN client do server cấp thông tin.

Kết nối qua **VPN client** có thể được tưởng tượng như thể bạn đang kết nối PC ở nhà với công ty bằng cáp mở rộng. Nhân viên có thể dial - quay số vào mạng công ty từ nhà của họ thông qua kết nối an toàn và hoạt động như thể họ đang ngồi trong văn phòng. Tuy nhiên, một **VPN client** trước tiên phải được cài đặt và cấu hình trên máy tính.

Điều này liên quan đến việc người dùng không được kết nối với internet thông qua ISP của riêng mình mà thiết lập kết nối trực tiếp thông qua nhà cung cấp VPN của họ. Điều này về cơ bản rút ngắn giai đoạn tunnel của hành trình VPN. Thay vì sử dụng VPN để tạo đường hầm mã hóa nhằm ngụy trang kết nối internet hiện có, VPN có thể tự động mã hóa dữ liệu trước khi cung cấp cho người dùng.

Đây là một dạng VPN ngày càng phổ biến, đặc biệt hữu ích cho các nhà cung cấp mạng WLAN công cộng không an toàn. Nó ngăn các bên thứ ba truy cập và xâm phạm kết nối mạng và mã hóa dữ liệu đến tận nhà cung cấp. Nó cũng ngăn ISP truy cập vào dữ liệu mà vì bất kỳ lý do gì vẫn chưa được mã hóa và bỏ qua bất kỳ hạn chế nào đối với quyền truy cập internet của người dùng (ví dụ: nếu chính phủ của quốc gia đó hạn chế quyền truy cập internet).

Ưu điểm của kiểu truy cập VPN này là hiệu quả cao hơn và khả năng truy cập phổ biến vào các tài nguyên của công ty. Với điều kiện có sẵn một hệ thống điện thoại thích hợp, chẳng hạn, nhân viên có thể kết nối với hệ thống bằng tai nghe và hành động như thể anh / cô ấy đang ở nơi làm việc của công ty họ. Ví dụ, khách hàng của công ty thậm chí không thể biết được nhân viên đang làm việc tại công ty hay tại văn phòng tại nhà của họ.
## 4. Tại sao sử dụng VPN
Hai mục đích chính là privacy-quyền riêng tư và access-quyền truy cập.
## 5. Các lợi ích bổ sung của VPN
* **Stream từ bất kỳ đâu**: Bạn có thể xem nội dung trực tiếp từ bất kể quốc gia nào mà hạn chế khu vực. Ví dụ, Mỹ cấm VN không được xem trực tiếp hoặc cấm IP VN không cho truy cập tại thời điểm đó. Thì bạn có thể chọn một địa chỉ VPN của Mỹ, giống như bạn đang đứng ở Mỹ để xem nội dung.
* **Truy cập các trang web bị chặn**: Một số tổ chức nhất định - trường học, thư viện, công ty - hạn chế quyền truy cập vào các trang web cụ thể như mạng xã hội, nhưng kết nối được mã hóa do VPN của bạn cung cấp sẽ xuyên qua.
* **Avoid censorship- Tránh kiểm duyệt**: đến đích mà bạn muốn truy cập mà không cần thông qua sự đánh giá hay xác minh.
* **Không bị theo dõi**: Tránh bị theo dõi bởi tin tặc, tội phạm mạng, các tập đoàn, chính phủ hoặc thậm chí là ISP của chính bạn.
## 6. VPN disadvantages
Như với bất kỳ loại công nghệ nào, cũng có một số nhược điểm khi sử dụng VPN.
* **Tốc độ có thể chậm hơn:** lưu lượng truy cập web trải qua nhiều bước hơn bình thường khi được kết nối qua VPN, vì vậy có thể có hiện tượng chậm lại.
* **Những thách thức về QoS**: QoS là viết tắt của “quality of service- chất lượng dịch vụ” và mô tả hiệu suất của một dịch vụ hoặc mạng. VPN chưa có tiêu chuẩn để đánh giá và báo cáo các phép đo như vậy. Không có chỉ số nào để phân tích, bạn cần dựa vào các bài đánh giá chuyên nghiệp và truyền miệng để tìm hiểu điều gì đáng tin cậy nhất.
* **VPN Block**: Một số doanh nghiệp đang trở nên khôn ngoan khi thực tế rằng VPN cho phép người dùng của họ truy cập nội dung. Để chống lại, các công ty đang bắt đầu chặn truy cập từ các địa chỉ IP VPN đã biết. Không dễ bị đánh bại như vậy, VPN có thể chỉ cần bật các địa chỉ IP mới để đánh lừa chúng một lần nữa.
* **Không có bảo vệ cookie**: Mặc dù VPN thực hiện công việc giữ cho bạn riêng tư và được mã hóa, nhưng VPN không thể chặn cookie, một số trong số đó là cần thiết để làm cho các trang web hoạt động bình thường.
## 7. Có thể sử dụng VPN trên thiết bị nào?
Nhà cung cấp dịch vụ sẽ cung cấp tài khoản. PC, Mac, Android và iOS - đăng nhập tài khoản để thăm gia môi trường VPN.

Việc thiết lập VPN khá dễ dàng - hầu hết các dịch vụ VPN đều hướng dẫn bạn tải xuống ứng dụng VPN thông qua trang tải xuống của họ.
## 8. Các yếu tố cần đánh giá khi chọn VPN?
* **Speed**: Đảm bảo VPN cung cấp đủ tốc độ, vì nhiều nhà cung cấp phải vật lộn để duy trì tốc độ đủ nhanh để phát trực tuyến hoặc tải xuống.
* **Máy chủ**: Khi nói đến hiệu suất, nhiều máy chủ hơn đồng nghĩa với việc duyệt web tốt hơn, vì mỗi máy chủ sẽ ít đông đúc hơn. Ngoài ra, càng ở gần máy chủ, kết nối của bạn càng nhanh và đáng tin cậy hơn.
* **Encryption**: Tìm kiếm AES-256 (tiêu chuẩn mã hóa nâng cao), giữ tiêu chuẩn mã hóa cao nhất cho đến nay. Nó hầu như không thể bị phá vỡ, vì nó có nhiều tổ hợp hơn là có các ngôi sao trong vũ trụ.
* **Protocol**: Tránh các giao thức bảo mật yếu hơn như PPTP và sử dụng OpenVPN đáng tin cậy hơn.
* **Nhật ký dữ liệu**: VPN lưu giữ Dât log (về cơ bản, tài khoản riêng của dịch vụ đó về các hoạt động internet của bạn).
* **Tri phí**

### Link tham khảo
* https://www.kaspersky.com/resource-center/definitions/what-is-a-vpn
* https://www.avast.com/c-what-is-a-vpn#:~:text=VPN%20stands%20for%20%22virtual%20private,while%20you%20use%20public%20networks.

