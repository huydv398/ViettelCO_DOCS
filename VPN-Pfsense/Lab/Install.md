# 

## /VPN-Pfsense/DOCS/intro.md
* CPU tương thích 64-bit amd64 (x86-64)
* RAM 1GB trở lên
* Ổ đĩa 8 GB hoặc lớn hơn (SSD, HDD, v.v.)
* Một hoặc nhiều network adapter tương thích
* Ổ USB có khả năng khởi động hoặc ổ đĩa quang dung lượng cao (DVD hoặc BD) để cài đặt ban đầu

Download [tại đây](https://www.pfsense.org/download/), sau khi tải xuống giải nén file.

## Hướng dẫn cài đặt


### Lựa chọn Partition / Filesystem (phân vùng/hệ thống tập tin)

Bước Phân vùng chọn hệ thống tệp cho đĩa đích của tường lửa.

Loại hệ thống tệp ZFS đáng tin cậy hơn và có nhiều tính năng hơn UFS, tuy nhiên ZFS có thể bị đói bộ nhớ. Một trong hai hệ thống tệp sẽ hoạt động trên phần cứng có RAM vài GB, nhưng nếu việc sử dụng RAM là quan trọng đối với các tác vụ khác sẽ chạy trên tường lửa này, thì UFS là một lựa chọn thận trọng hơn. Đối với phần cứng yêu cầu UEFI, hãy sử dụng ZFS.

Các tùy chọn trên màn hình này hoạt động như sau:

* **Auto (ZFS)**: Khởi chạy phần cấu hình ZFS của trình cài đặt. Xem ZFS để biết thêm chi tiết.
* **Auto (UFS) BIOS**: Tự động tạo phân vùng và định dạng đĩa bằng UFS và môi trường khởi động kiểu BIOS traditional/legacy.
**Auto (UFS) UEFI**: Tự động tạo phân vùng và định dạng đĩa bằng UFS và môi trường khởi động UEFI.
    >**Ghi chú**: Đôi khi có sự không tương thích giữa việc triển khai FreeBSD và UEFI. Nếu hệ thống không khởi động được sau khi cài đặt với tùy chọn UEFI, hãy định cấu hình phần cứng để khởi động BIOS/legacy và chọn tùy chọn cài đặt đó thay thế.
* **Manual**: Tạo phân vùng và hệ thống tệp theo cách thủ công.
* **Shell**: Mở shell prompt để định cấu hình disks, partitions, và filesystems bằng tay.