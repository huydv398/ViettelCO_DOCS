# What is VPN protocols?
Các giao thức được sử dụng trong VPN
1. [VPN protocols?](#vpn-protocols)
1. [Các giao thức VPN hiện đang được sử dụng.](#các-giao-thức-vpn-hiện-đang-được-sử-dụng)
    * [1. OpenVPN](#1-openvpn)
    * [2. IPSec/IKEv2](#2-ipsecikev2)
    * [3. Wireguard](#3-wireguard)
    * [4. SSTP](#4-sstp)
    * [5. L2TP/IPSec](#5-l2tpipsec)
    * [6. PPTP](#6-pptp)
1. [So sánh các giao thức](#so-sánh-các-giao-thức)
1. [Giao thức VPN tốt nhất là gì?](#giao-thức-vpn-tốt-nhất-là-gì)
1. [Giao thức VPN nhanh nhất là gì?](#giao-thức-vpn-nhanh-nhất-là-gì)
1. [Giao thức VPN an toàn nhất là gì?](#giao-thức-vpn-an-toàn-nhất-là-gì)
1. [Giao thức VPN ổn định nhất là gì?](#giao-thức-vpn-ổn-định-nhất-là-gì)
1. [Giao thức VPN dễ thiết lập nhất là gì?](#giao-thức-vpn-dễ-thiết-lập-nhất-là-gì)
## VPN protocols?
Giao thức VPN về cơ bản là công nghệ mà dịch vụ VPN của bạn sử dụng để đảm bảo bạn có được kết nối Internet nhanh nhất và an toàn nhất có thể. Kết hợp các tiêu chuẩn mã hóa và giao thức truyền, giao thức VPN xác định cách dữ liệu của bạn được truyền giữa thiết bị của bạn và máy chủ VPN.

## Các giao thức VPN hiện đang được sử dụng.
### 1. OpenVPN
OpenVPN là một giao thức rất phổ biến và có tính bảo mật cao được nhiều nhà cung cấp VPN sử dụng. Nó chạy trên giao thức Internet TCP hoặc UDP. Cái trước sẽ đảm bảo rằng dữ liệu của bạn sẽ được phân phối đầy đủ và đúng thứ tự trong khi cái sau sẽ tập trung vào tốc độ nhanh hơn. Nhiều VPN, bao gồm cả NordVPN, sẽ cho phép bạn lựa chọn giữa hai.

**Ưu điểm**
* **Open source**, nghĩa là nó minh bạch. Bất kỳ ai cũng có thể kiểm tra code để tìm các hidden backdoors hoặc lỗ hổng bảo mật có thể ảnh hưởng đến bảo mật VPN của bạn.
* **Tính linh hoạt**. Nó có thể được sử dụng với một loạt các giao thức mã hóa và lưu lượng khác nhau, được định cấu hình cho các mục đích sử dụng khác nhau, hoặc an toàn hoặc nhẹ nhàng tùy theo nhu cầu của bạn.
* **Bảo vệ**. Nó có thể chạy hầu hết mọi giao thức mã hóa, làm cho nó rất an toàn.
* **Vượt qua hầu hết các bức tường lửa**. Khả năng tương thích tường lửa, có thể vượt qua tường lửa của mình một cách dễ dàng.

**Nhược điểm**
* **Thiết lập phức tạp**. Người dùng có thể bị tê liệt bởi sự lựa chọn và sự phức tạp nếu họ cố gắng thiết lập OpenVPN của riêng mình.

**Sử dụng khi nào**: OpenVPN không thể thay thế khi bạn cần bảo mật hàng đầu: kết nối với Wi-Fi công cộng, đăng nhập vào cơ sở dữ liệu của công ty bạn hoặc sử dụng các dịch vụ ngân hàng.
### 2. IPSec/IKEv2

IKEv2 đặt nền tảng cho một kết nối VPN an toàn bằng cách thiết lập một kết nối được xác thực và mã hóa. Nó được phát triển bởi Microsoft và Cisco để có tốc độ nhanh, ổn định và an toàn. Nó thành công trên tất cả các mặt trận này, nhưng nơi nó thực sự tỏa sáng là sự ổn định của nó. Là một phần của hộp công cụ bảo mật internet IPSec, IKEv2 sử dụng các công cụ IPSec khác để cung cấp phạm vi phủ sóng VPN toàn diện.

**Ưu điểm**

* **Sự ổn định**. IKEv2 thường sử dụng một công cụ IPSec được gọi là Mobility and Multi-homing Protocol, đảm bảo kết nối VPN khi bạn di chuyển giữa các kết nối internet. Điều này làm cho IKEv2 trở thành giao thức ổn định và đáng tin cậy nhất cho các thiết bị di động.
* **Bảo vệ**. Là một phần của bộ IPSec, IKEv2 hoạt động với hầu hết các thuật toán mã hóa hàng đầu, khiến nó trở thành một trong những VPN an toàn nhất.
* **Tốc độ**. Nó chiếm ít băng thông khi hoạt động và khả năng truyền qua NAT giúp nó kết nối và giao tiếp nhanh hơn. Nó cũng giúp vượt qua tường lửa.

**Nhược điểm**
* **Khả năng tương thích hạn chế**. IKEv2 không tương thích với quá nhiều hệ thống. Đây sẽ không phải là vấn đề đối với người dùng Windows vì Microsoft đã giúp tạo ra giao thức này, nhưng một số hệ điều hành khác sẽ cần các phiên bản thích ứng.

* **Sử dụng nó khi nào**: Độ ổn định của IPSec / IKEv2 đảm bảo rằng bạn sẽ không bị mất kết nối VPN khi chuyển từ Wi-Fi sang dữ liệu di động, vì vậy nó có thể là một lựa chọn tốt khi bạn đang di chuyển. Nó cũng nhanh chóng vượt qua tường lửa và có thể cung cấp tốc độ cao trên các nền tảng phát trực tuyến.
### 3. Wireguard
Wireguard là giao thức tunnelling mới nhất và nhanh nhất mà toàn bộ ngành công nghiệp VPN đang nói đến. Nó sử dụng mật mã hiện đại vượt trội hơn các công nghệ hiện tại - OpenVPN và IPSec/IKEv2.

**Ưu điểm**
* **Free and Open Source**. Bất kỳ ai cũng có thể xem mã của nó, điều này giúp cho việc triển khai, kiểm tra và gỡ lỗi trở nên dễ dàng hơn.
* **Hiện đại và cực kỳ nhanh chóng**. Nó chỉ bao gồm 4.000 dòng mã, khiến nó trở thành "giao thức tốt nhất" trong số tất cả. Để so sánh, mã OpenVPN có số dòng nhiều hơn 100 lần.

**Nhược điểm**
* **Chưa hoàn thiện**. Wireguard được hứa hẹn là “MỘT SẢN PHẨM THAY THẾ TRONG TƯƠNG LAI”, nhưng việc triển khai nó vẫn đang trong giai đoạn đầu và còn rất nhiều chỗ để cải thiện. Nó hiện không cung cấp cho người dùng tính năng ẩn danh đầy đủ, vì vậy các nhà cung cấp VPN cần tìm các giải pháp tùy chỉnh để cung cấp bảo mật cần thiết mà không làm giảm tốc độ.

**Sử dụng khi nào**: Sử dụng Wireguard bất cứ khi nào ưu tiên tốc độ: phát trực tuyến, chơi trò chơi trực tuyến hoặc tải xuống các tệp lớn.

### 4. SSTP

Secure Socket Tunneling Protocol (SSTP) là một giao thức VPN khá an toàn và có khả năng được tạo ra bởi Microsoft. Nó có những mặt trái của nó, có nghĩa là mỗi người dùng phải tự quyết định xem liệu giao thức này có đáng để sử dụng hay không. Mặc dù là một sản phẩm chủ yếu của Microsoft, SSTP vẫn có sẵn trên các hệ thống khác ngoài Windows.

**Ưu điểm**

* **Thuộc sở hữu của Microsoft**. Windows sẽ hỗ trợ SSTP hoặc được tích hợp sẵn. Điều đó cũng có nghĩa là nếu bạn cố gắng tự thiết lập, nó sẽ dễ dàng và bạn có thể mong đợi sự hỗ trợ của Microsoft.

* **Chắc chắn**. Tương tự như các VPN hàng đầu khác, SSTP hỗ trợ giao thức mã hóa AES-256.

***Vượt tường lửa**. SSTP có thể vượt qua hầu hết các tường lửa mà không làm gián đoạn liên lạc của bạn.

**Nhược điểm**

* **Thuộc sở hữu của Microsoft**, có nghĩa là mã này không có sẵn cho các nhà nghiên cứu bảo mật để thử nghiệm. Microsoft đã được biết là hợp tác với NSA và các cơ quan thực thi pháp luật khác, vì vậy một số nghi ngờ rằng hệ thống có thể có cửa hậu. Nhiều nhà cung cấp VPN tránh giao thức này.

**Sử dụng nó khi nào**: SSTP rất tốt để bỏ qua các giới hạn địa lý và tăng cường quyền riêng tư trong khi duyệt internet.
### 5. L2TP/IPSec

**Layer 2 tunneling protocol (L2TP)** không thực sự cung cấp bất kỳ mã hóa hoặc xác thực nào - nó chỉ đơn giản là một giao thức tunneling VPN tạo kết nối giữa bạn và máy chủ VPN. Nó dựa vào các công cụ khác trong bộ IPSec để mã hóa lưu lượng truy cập của bạn và giữ cho nó riêng tư và an toàn. Giao thức này có một vài tính năng tiện lợi, nhưng một số vấn đề nhất định khiến nó không thể trở thành giao thức VPN hàng đầu.

**Ưu điểm**

* **Bảo vệ**. Trớ trêu thay, L2TP không cung cấp bất kỳ bảo mật nào khiến nó khá an toàn. Đó là bởi vì nó có thể chấp nhận một số giao thức mã hóa khác nhau, làm cho giao thức trở nên an toàn hoặc nhẹ như bạn cần.
* **Phổ biến rộng rãi**. L2TP có sẵn trên hầu hết các hệ thống tiêu dùng hiện đại, có nghĩa là quản trị viên sẽ không gặp khó khăn khi tìm kiếm hỗ trợ và làm cho nó chạy.

**Nhược điểm**

* **Có khả năng bị xâm phạm bởi NSA**. Giống như IKEv2, L2TP thường được sử dụng với IPSec, do đó nó có cùng các lỗ hổng đã đề cập trước đó.
* **Chậm**. Giao thức đóng gói dữ liệu hai lần, có thể hữu ích cho một số ứng dụng nhưng làm cho nó chậm hơn so với các giao thức khác chỉ đóng gói dữ liệu của bạn một lần.
* **Gặp khó khăn với tường lửa**. Không giống như các giao thức VPN khác, L2TP không có bất kỳ cách thông minh nào để vượt qua tường lửa. Các quản trị viên hệ thống theo định hướng giám sát sử dụng tường lửa để chặn VPN và những người tự định cấu hình L2TP là một mục tiêu dễ dàng.

**Khi nào sử dụng**: Bạn có thể sử dụng L2TP để mua sắm trực tuyến một cách an toàn và thực hiện các hoạt động ngân hàng. Nó cũng có lợi khi bạn muốn kết nối nhiều chi nhánh công ty thành một mạng.

### 6. PPTP

Giao thức đường hầm điểm tới điểm (PPTP) được tạo ra vào năm 1999 và là giao thức VPN đầu tiên được phổ biến rộng rãi. Nó lần đầu tiên được thiết kế để tạo đường hầm cho lưu lượng quay số! Nó sử dụng một số giao thức mã hóa yếu nhất so với bất kỳ giao thức VPN nào trong danh sách này và có nhiều lỗ hổng bảo mật. 

* Được tạo ra bởi Microsoft, đây là một trong những giao thức lâu đời nhất được sử dụng trên internet hiện nay. Do đó, nó chỉ thực sự hữu ích nếu bạn đang sử dụng nó trên hệ điều hành Windows cũ hơn, mặc dù nó nhanh và dễ triển khai. Tuy nhiên, nếu một dịch vụ VPN chỉ cung cấp điều này, thì điều đó không được khuyến khích.
*  TCP port 1723
* Một PPTP tunnel được khởi tạo bằng cách giao tiếp với nhau trên cổng TCP 1723. Kết nối TCP này sau đó được sử dụng để khởi tạo và quản lý một đường hầm GRE tới GRE ngang hàng. Định dạng gói PPTP GRE không phải là tiêu chuẩn, bao gồm trường số xác nhận mới thay thế trường định tuyến điển hình trong tiêu đề GRE. Tuy nhiên, giống như trong một kết nối GRE thông thường, các gói GRE đã sửa đổi đó được đóng gói trực tiếp thành các gói IP và được coi là giao thức IP số 47. Đường hầm GRE được sử dụng để mang các gói PPP được đóng gói, cho phép tạo đường hầm của bất kỳ giao thức nào có thể được thực hiện bên trong PPP, bao gồm IP, NetBEUI và IPX

**Ưu điểm**

* **Nhanh**. Nó đã lỗi thời, vì vậy các máy hiện đại chạy PPTP rất hiệu quả. Nó nhanh nhưng cung cấp bảo mật tối thiểu, đó là lý do tại sao nó phổ biến đối với những người muốn thiết lập VPN gia đình một cách nghiêm ngặt để truy cập nội dung bị chặn theo địa lý.

* **Tương thích cao**. Trong nhiều năm kể từ khi nó được tạo ra, PPTP về cơ bản đã trở thành tiêu chuẩn tối thiểu nhất để đào đường hầm và mã hóa. Hầu hết mọi hệ thống và thiết bị hiện đại đều hỗ trợ nó. Điều này cũng giúp bạn dễ dàng thiết lập và sử dụng.

**Nhược điểm**

* **Không an toàn**. Nhiều lỗ hổng và cách khai thác đã được xác định cho PPTP. Một số (không phải tất cả) đã được vá và thậm chí Microsoft còn khuyến khích người dùng chuyển sang L2TP hoặc SSTP.

* **Cracked by the NSA**. NSA được cho là thường xuyên giải mã giao thức này như một lẽ tất nhiên.

* **Bị chặn bởi tường lửa**. Là một hệ thống cũ, lỗi thời và thô sơ, các kết nối PPTP dễ bị chặn hơn qua tường lửa. Nếu bạn đang sử dụng giao thức tại một trường học hoặc doanh nghiệp chặn kết nối VPN, điều này có thể làm gián đoạn dịch vụ của bạn.

**Khi nào sử dụng**: Chúng tôi khuyên bạn chỉ nên sử dụng PPTP để phát trực tuyến hoặc truy cập nội dung bị chặn theo địa lý. Đối với bất kỳ điều gì khác, bạn nên sử dụng các giao thức VPN nâng cao hơn.
### So sánh các giao thức
|VPN Protocol|Speed|Encryption|Streaming|Stability|P2P|
|-|-|-|-|-|-|
|OpenVPN|Nhanh|Rất Tốt|Tốt|Tốt|Tốt
|IPSec/IKEv2|Nhanh|Rất tốt|Tốt|Rất tốt|Tốt
|Wireguard|Rất nhanh|Rất tốt|Tốt|Rất tốt|Tốt
|SSTP|Trung bình|Tốt|Trung bình|Trung bình|Tốt|
|L2TP/IPSec|Trung bình|Trung bình|Kém|Tốt|Kém|
|PPTP|Nhanh|Kém|Kém|Tốt|Kém|

## Giao thức VPN tốt nhất là gì?
Không có cái gọi là giao thức VPN tốt nhất phù hợp với tất cả mọi người. Câu trả lời cho câu hỏi này phụ thuộc vào nhu cầu của bạn và những gì bạn làm trên internet. Nếu bạn là một người thích chơi game, bạn có thể sử dụng VPN vì những lý do khác với một người xem nhiều chương trình truyền hình hoặc thường xuyên làm việc tại quán cà phê.

## Giao thức VPN nhanh nhất là gì?
Wireguard được coi là một trong những giao thức VPN nhanh nhất, cung cấp thời gian kết nối / kết nối lại nhanh hơn và cải thiện thời lượng pin cho thiết bị di động. IKEv2/IPsec cũng được coi là một giao thức nhanh và nó có thể phục vụ nhu cầu của nhiều người.

## Giao thức VPN an toàn nhất là gì?
Nhiều chuyên gia VPN khuyến nghị OpenVPN là giao thức an toàn nhất. Nó sử dụng mã hóa 256-bit làm mặc định nhưng cũng cung cấp các mật mã khác như 3DES (tiêu chuẩn mã hóa dữ liệu ba lần), Blowfish, CAST-128 và AES (Tiêu chuẩn mã hóa nâng cao).
## Giao thức VPN ổn định nhất là gì?
IKEv2/IPsec được coi là giao thức VPN ổn định nhất vì nó cung cấp kết nối mạnh mẽ và cho phép người dùng chuyển đổi giữa các mạng mà không gặp rủi ro về bảo mật.
## Giao thức VPN dễ thiết lập nhất là gì?
Giao thức PPTP được tích hợp vào nhiều thiết bị, làm cho nó trở thành một trong những giao thức dễ thiết lập nhất. Tuy nhiên, vì nó đã lỗi thời và nổi tiếng về các vấn đề bảo mật, chúng tôi khuyên bạn không nên sử dụng nó. Xem xét các tùy chọn khác như Wireguard hoặc IKEv2/IPsec.
