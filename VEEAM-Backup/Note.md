* Yêu cầu quyền Administrator để đang nhập vào vCenter.
* Đặt DNS với DNS của vCenter đang sử dụng
* Yêu cầu mở các port sau:
    * vCenter Server: port 443, 10443
    * Port từ vcenter tới ESXi host để tranfer dữ liệu(Protocol NFS): 902
    * NFC storage connection
    