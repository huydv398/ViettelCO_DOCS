# Add NAS to Unbuntu
Bước 1: Tạo mới Folder hoặc Folder có sẵn(Nếu đã có folder thực hiện luôn bước 6):

![image](/images/Screenshot_105.png)

Bước 2: Đặt tên cho Folder

![image](/images/Screenshot_106.png)

Bước 3: Next 

![image](/images/Screenshot_107.png)

Bước 4: Tích Rồi Next:

![image](/images/Screenshot_108.png)

Bước 5: Apply

![image](/images/Screenshot_109.png)

Bước 6: Chọn folder -> Edit

![image](/images/Screenshot_110.png)

Bước 7: Phân quyền cho người dùng Window: Permission -> Tích Vào ô phân quyền cho User

![image](/images/Screenshot_111.png)

Bước 8: Phân quyền cho người dùng Ubuntu

Create -> NFS Permission 

![image](/images/Screenshot_112.png)

Bước 9: Hostname or IP

Địa chỉ Ip của máy Ubuntu đang sử dụng

Kiểm tra địa chỉ ip: ip a. Máy phải ping được đến ip NAS

![image](/images/Screenshot_115.png)

Nhập địa chỉ IP subnetmask

![image](/images/Screenshot_113.png)

Bươc 10: OK

![image](/images/Screenshot_114.png)

## Thực hiện add Bên máy Ubuntu

Bước 11:  Thực hiện lệnh với terminal:

```
sudo apt install update
sudo apt install nfs-common -y
sudo mkdir /DATA

sudo mount -t nfs 192.168.174.40:/volume1/Fileshare /DATA
```

* 192.168.174.40: Địa chỉ IP NAS
* /volume1: tên của volume(số 2 bước 2)
* /Fileshare: Folder tạo để Share(số 1 bước 2)
* /DATA: thư mục được tạo để gắn NAS

Tạo thành công sẽ được như sau:

![image](/images/Screenshot_116.png)

## Add to Window
Windows + r

![image](/images/Screenshot_117.png)

rồi map với This PC

![image](/images/Screenshot_118.png)