# Hướng dẫn Cấu hình Backup

## Active Full Backup

Phương pháp sao lưu này có thể yêu cầu bạn tạo một bản sao lưu đầy đủ vào cuối tuần và chạy sao lưu gia tăng vào các ngày làm việc. Để cho phép bạn tuân thủ các yêu cầu này, Veeam Backup & Replication cho phép bạn tạo các bản sao lưu đầy đủ đang hoạt động.

![image](/images/Screenshot_42.png)

Bạn có thể tạo các bản sao lưu đầy đủ đang hoạt động theo cách thủ công hoặc lên lịch công việc sao lưu để tạo các bản sao lưu đầy đủ đang hoạt động theo định kỳ.

![image](/images/Screenshot_43.png)





### Bước 1. Khởi chạy trình hướng dẫn công việc sao lưu mới

Trên tab Home , bấm Backup và chọn Virtual machine.

![image](/images/Screenshot_44.png)

### Bước 2. Chỉ định tên và mô tả công việc
Trong trường Name, hãy nhập tên cho công việc sao lưu.

![image](/images/Screenshot_45.png)

### Bước 3. Chọn máy ảo để sao lưu

Để thêm máy ảo vào công việc:
* Nhấp vào Add.
* Chọn VM hoặc vùng chứa VM trong danh sách và nhấp vào Add .
* Hoặc sử dụng tìm kiếm ở dưới để nhập tên máy chủ, cum máy chủ, ...

![image](/images/Screenshot_46.png)


### Bước 4. Loại trừ các đối tượng khỏi công việc sao lưu

![image](/images/Screenshot_47.png)

### Bước 5. Xác định thứ tự sao lưu VM
Tùy chọn thứ tự sao lưu của VMs

![image](/images/Screenshot_48.png)



### Bước 6. Chỉ định Cài đặt Bộ nhớ Dự phòng
Tại bước Storage của trình hướng dẫn, hãy chọn các thành phần cơ sở hạ tầng sao lưu cho công việc - proxy sao lưu và kho lưu trữ sao lưu, và chỉ định cài đặt lưu trữ sao lưu.

Chọn vị trí lưu:

![image](/images/Screenshot_49.png)

![image](/images/Screenshot_50.png)

### Advanced

* Backup Settings
* Maintenance Settings

**Remove deleted items data after <N> days**: chỉ định số ngày bạn muốn giữ dữ liệu sao lưu cho các máy ảo đã xóa

**Defragment and compact full backup file**: Trong quá trình hoạt động nhỏ gọn, Veeam Backup & Replication tạo ra một tệp trống mới và sao chép vào đó các khối dữ liệu từ tệp sao lưu đầy đủ. Do đó, toàn bộ tệp sao lưu được chống phân mảnh và tốc độ đọc và ghi từ / đến tệp sao lưu tăng lên.

* Storage

**Compression level list**: Compression level list