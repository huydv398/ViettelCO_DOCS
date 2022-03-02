* Yêu cầu quyền Administrator để đang nhập vào vCenter.
* Đặt DNS với DNS của vCenter đang sử dụng
* Yêu cầu mở các port sau:
    * vCenter Server: port 443, 10443
    * Port từ vcenter tới ESXi host để tranfer dữ liệu(Protocol NFS): 902
    * NFC storage connection
    * `Test-NetConnection -ComputerName [IP-ESXi] -Port 902`
    * Components:
        * Installer using port 6160
        * Transport using port 6162
    * 6184: được sử dụng để liên lạc với Veeam Agent cho Dịch vụ Microsoft Windows
    * 6160, 11731: Các cổng mặc định được sử dụng để giao tiếp với Dịch vụ trình cài đặt Veeam
    * 1443: Port của cơ sở dữ liệu
    * 2500-3300 TCP/UDP
* Backup Cluster:
    * https://www.veeam.com/kb2463