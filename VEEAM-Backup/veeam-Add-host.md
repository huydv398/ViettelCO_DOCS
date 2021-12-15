# Hướng dẫn thêm máy chủ vào Veeam Backup

* Thêm VMware vSphere Servers

## Đăng nhập vào Veeam Backup & Replication
Đăng nhập bằng tài khoản mặc định khi setup ban đầu

![image](/images/Screenshot_23.png)

## Cấu hình Virtualization Servers và Hosts

Bạn có thể thêm các loại server và hosts sau vào cơ sở hạ tầng backup:
* VMware vSphere Server
* VMware vCloud Director
* Microsoft Windows Server
* Linux Server

### Thêm VMware vSphere Servers
Bạn có thể thêm Máy chủ vCenter và máy chủ ESXi. Nếu máy chủ ESXi được quản lý bởi Máy chủ vCenter, bạn nên thêm Máy chủ vCenter, không phải máy chủ ESXi độc lập. Nếu bạn di chuyển các máy ảo giữa các máy chủ ESXi do vCenter Server quản lý, bạn sẽ không phải cấu hình lại các công việc trong Veeam Backup & Replication . Veeam Backup & Replication sẽ tự động xác định vị trí các máy ảo được di chuyển và tiếp tục xử lý chúng như bình thường.

**Bước 1**. Khởi chạy trình hướng dẫn máy chủ VMware mới

Mở chế độ xem **Backup Infrastructure**. Chọn nút **Add Server**

![image](/images/Screenshot_24.png)



![image](/images/Screenshot_25.png)



![image](/images/Screenshot_26.png)

**Bước 2**: Chỉ định tên máy chủ hoặc địa chỉ

Nhập tên DNS đầy đủ hoặc địa chỉ IP của Máy chủ vCenter hoặc máy chủ ESXi độc lập.

![image](/images/Screenshot_27.png)

**Bước 3** Chỉ định thông tin đăng nhập

Chọn **Add**

![image](/images/Screenshot_30.png)

Nhập thông tin đăng nhập vCenter

![image](/images/Screenshot_31.png)

Chọn **Continue**

![image](/images/Screenshot_28.png)

**Finish** để thêm host

![image](/images/Screenshot_29.png)

### Thêm Windows Server

Bạn phải thêm vào cơ sở hạ tầng sao lưu Các máy chủ Microsoft Windows mà bạn định sử dụng làm thành phần cơ sở hạ tầng dự phòng và máy chủ mà bạn định sử dụng cho các loại hoạt động khôi phục khác nhau.

![image](/images/Screenshot_32.png)

**Bước 2**: Chỉ định tên máy chủ hoặc địa chỉ

Nhập tên DNS đầy đủ hoặc địa chỉ IP của Máy chủ.

![image](/images/Screenshot_27.png)

**Bước 3** Chỉ định thông tin đăng nhập

Chọn **Add**

![image](/images/Screenshot_30.png)

Nhập thông tin đăng nhập của Window server 

![image](/images/Screenshot_33.png)

Cài đặt các thành phần cần thiết.

![image](/images/Screenshot_34.png)



![image](/images/Screenshot_35.png)

Kiểm tra lại các thông tin. Finish

![image](/images/Screenshot_36.png)

## Thêm máy chủ Linux
Bạn phải thêm vào cơ sở hạ tầng sao lưu các máy chủ Linux mà bạn định sử dụng làm kho lưu trữ sao lưu và máy chủ mà bạn định sử dụng cho các loại hoạt động khôi phục khác nhau.

![image](/images/Screenshot_37.png)

Nhập tên DNS đầy đủ hoặc địa chỉ IP của Máy chủ.

![image](/images/Screenshot_27.png)

Chọn **Add**

![image](/images/Screenshot_30.png)

Nhập thông tin đăng nhập của linux


![image](/images/Screenshot_38.png)

Làm các bước như hình:


![image](/images/Screenshot_39.png)



![image](/images/Screenshot_40.png)

Finish để kết thúc cài đặt

![image](/images/Screenshot_41.png)

