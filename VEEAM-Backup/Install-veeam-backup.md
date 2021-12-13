# Hướng dẫn cài đặt Veeam Backup & Replication
 Phiên bản Cài đặt VEEAM Backup & Replication 9.5.4.2615.Update4
## Yêu cầu
* **Hệ điều hành**: Windows XP / Vista / 7/8 / 8.1 / 10
* **Bộ nhớ (RAM)**: Yêu cầu 4 GB RAM.
* **Dung lượng đĩa cứng**: Cần 4 GB dung lượng trống.
* **Bộ xử lý**: Bộ xử lý Intel Dual Core trở lên.
* **VMware infrastructure**: vSphere 6.x, vSphere 5.x, ESXi 6.x, ESXi 5.x, vCenter Server 6.x (optional), vCenter Server 5.x (optional), vCloud Director 8.x, and 9.x (optional)
* Tất cả các hệ điều hành được hỗ trợ bởi VMware

Tải VEEAM Backup theo đường dẫn, [tại đây](https://drive.google.com/file/d/1Y2N3jqScBqb1BGyobGX2Da7l87O60CPI/view).

## Hướng dẫn cài đặt Veeam Backup & Replication
* Giải nén phần mềm vừa Download.
* Chuột phải, chọn **Mount** file ISO
![image](/images/Screenshot_1.png)

* Chạy file Setup -> Install để cài đặt phần mềm


![image](/images/Screenshot_2.png)

**Install**

![image](/images/Screenshot_3.png)

Tick 2 checkbox -> Next 

![image](/images/Screenshot_4.png)

Để trống -> Next 

![image](/images/Screenshot_5.png)

Có thể thay đổi nơi cài đặt tại bước này -> Next 

![image](/images/Screenshot_6.png)

Thực hiện **Install** để cài đặt các Plug-in đi kèm.

![image](/images/Screenshot_7.png)

Sau khi thực hiện cài đặt các phần mềm yêu cầu -> Next.

![image](/images/Screenshot_8.png)

**Install** để cài đặt Veeam

![image](/images/Screenshot_9.png)

Quá trình cài đặt có thể mất từ 5-20p, Sau khi cài đặt xong nhấn Finish

![image](/images/Screenshot_10.png)

Thực hiện tại **Task Manager** -> **Service**, thực Stop 2 dịch vụ sau:

* VeeanBackupSvc:

![image](/images/Screenshot_11.png)

* VeeamCatalogSvc

![image](/images/Screenshot_12.png)

Tại thư mục giải nén Veeam One. Copy thư mục **Program Files**

![image](/images/Screenshot_13.png)

Đi tới thư mục:  **C:**

Thực hiện Paste thư mục **Program Files** đã copy ở bước trước. 


![image](/images/Screenshot_14.png)

Thực hiện bật lại 2 service 

![image](/images/Screenshot_15.png)

Thực hiện chạy ứng ụng từ màn hình desktop.

![image](/images/Screenshot_16.png)

Thực hiện Update License

![image](/images/Screenshot_17.png)

Chọn **Install License**

![image](/images/Screenshot_18.png)

Chọn file **License.lic**

![image](/images/Screenshot_19.png)

Thực hiện Update License thành công

![image](/images/Screenshot_20.png)

Tổng quan giao diện Veeam Backup & Replication

![image](/images/Screenshot_21.png)

Kết thúc