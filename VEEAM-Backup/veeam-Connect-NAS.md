# Hướng cấu hình Veeam - NAS



Tại máy đang cài đặt Veeam Backup thực hiện truy cập đường Link: find.synology.com

Khi tìm thấy Thiết bị NAS thực hiện **Connect**:

![image](/images/Screenshot_56.png)

Tích vào checkbox, Click **Next**:

![image](/images/Screenshot_57.png)

Click **Continue**:

![image](/images/Screenshot_58.png)

Thực hiện setup bước đầu cho NAS Synology, Click **Setup**:

![image](/images/Screenshot_59.png)

Click **Install** 

![image](/images/Screenshot_60.png)

Thời gian thực hiện cài đặt 5-10 phút

Thực hiện setup Tài khoản, mật khẩu đăng nhập cho Thiết bị NAS, Click Next sau khi Điền đầy đủ Thông tin(Username không được để chữ hoa): 

![image](/images/Screenshot_63.png)

Thông báo khi có bản cập nhập cho DSM:

![image](/images/Screenshot_64.png)

**Skip this step**

![image](/images/Screenshot_65.png)

Tick vào checkbox để share thiết bị:

![image](/images/Screenshot_66.png)

Đã thực hiện cài đặt xong 
## Đăng nhập quản trị

![image](/images/Screenshot_67.png)

Thực hiện cấu hình thiết bị lưu trữ:

**Menu** -> **Storage Manager**:


![image](/images/Screenshot_68.png)

Tạo pool, **Storage Pool** -> **Create**

![image](/images/Screenshot_69.png)

**Better performance** -> **Next**

![image](/images/Screenshot_70.png)

Chọn Raid 5 nếu có 3 thiết bị disk trở nên

![image](/images/Screenshot_71.png)

Kéo các thiết bị vào Storage pool

![image](/images/Screenshot_72.png)

**Next**

![image](/images/Screenshot_73.png)

OK, cảnh tất cả các dữ liệu có trên các ổ có thể bị xóa.

![image](/images/Screenshot_74.png)

Thực hiện Apply cấu hình:

![image](/images/Screenshot_75.png)

### Cấu hình Volume

**Volume** -> **Create**

![image](/images/Screenshot_76.png)

Chọn Pool mà vừa tạo ở bước trước rồi click **Next**

![image](/images/Screenshot_77.png)

**Next**

![image](/images/Screenshot_78.png)

Chọn Loại file system:

![image](/images/Screenshot_79.png)

Click **Apply**

![image](/images/Screenshot_80.png)

## Thay đổi địa chỉ IP tĩnh

**Control Panel** -> **Network** -> **Network Interface** -> Chọn Interface mà NAS đăng sử dụng -> **Edit**

![image](/images/Screenshot_81.png)

Tick **Use nanual configuration**, Điền địa chỉ IP tĩnh, chọn **OK**:

![image](/images/Screenshot_82.png)

NAS sẽ tự đọng reset phiên về địa chỉ IP mới:

![image](/images/Screenshot_83.png)

## Thực hiện tạo folder
Chọn **File Station**

![image](/images/Screenshot_89.png)

**Create** -> **Create New Shared Folder**

![image](/images/Screenshot_90.png)

Tạo tên Folder và Volome 

![image](/images/Screenshot_91.png)

**Next**

![image](/images/Screenshot_92.png)

Tick Enabe checksum, **Next** 

![image](/images/Screenshot_93.png)

**Apply**

![image](/images/Screenshot_94.png)

Tick **Read/write** 

![image](/images/Screenshot_95.png)

Thư mục sau khi tạo xong

![image](/images/Screenshot_96.png)


## Thực hiện cấu hình thêm NAS cho Veeam Backup:

Mở bảng điều khiển Veeam Backup

![image](/images/Screenshot_84.png)

**Backup Infrastructure** -> **Add Repository**

![image](/images/Screenshot_85.png)

Chọn **Network Attached Storage**

![image](/images/Screenshot_86.png)

Chọn **Share Folder**

![image](/images/Screenshot_87.png)

Nhập tên cho repo mới

![image](/images/Screenshot_88.png)

Thêm Share folder: **\ \192.168.174.40\BACKUP** (\ \IP_address\Folder_name)

Tick **This share requires access credentials:** - Xác thực

Chọn Add để điền thông tin xác thực(thông tin đăng nhập NAS)

![image](/images/Screenshot_97.png)

User/pass của NAS synology, chọn OK

![image](/images/Screenshot_98.png)

Next 

![image](/images/Screenshot_99.png)

Thông tin folder, Next:

![image](/images/Screenshot_100.png)

Gắn vào máy chủ veeam hiện tại, Next;

![image](/images/Screenshot_101.png)

Kiểm tra lại thông tin, Apply :

![image](/images/Screenshot_102.png)

Finish để hoàn thành cài đặt:

![image](/images/Screenshot_103.png)

Repo sau khi tạo sẽ được như hình bên dưới.

![image](/images/Screenshot_104.png)

Link Tham khảo:
* https://xpertstec.com/how-to-add-nas-volume-veeam-backup-repository/
* https://chunguyenbn.com/huong-dan-cai-dat-xpenology-tren-vmware-workstation/
* https://drive.google.com/drive/folders/1eutR4OTDnMs4TUiyFrgwhMkc_jEmMfyq
