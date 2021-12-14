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

#### Advanced

* Backup Settings
* Maintenance Settings

**Remove deleted items data after <N> days**: chỉ định số ngày bạn muốn giữ dữ liệu sao lưu cho các máy ảo đã xóa

**Defragment and compact full backup file**: Trong quá trình hoạt động nhỏ gọn, Veeam Backup & Replication tạo ra một tệp trống mới và sao chép vào đó các khối dữ liệu từ tệp sao lưu đầy đủ. Do đó, toàn bộ tệp sao lưu được chống phân mảnh và tốc độ đọc và ghi từ / đến tệp sao lưu tăng lên.

* Storage

**Compression level list**: chọn mức nén cho bản sao lưuCompression level list
![image](/images/Screenshot_51.png)
* Notifications:

**Send email notifications to the following recipients**: chọn hộp kiểm nếu bạn muốn nhận thông báo về trạng thái hoàn thành công việc qua email. Trong trường bên dưới, hãy chỉ định địa chỉ email của người nhận. Bạn có thể nhập một số địa chỉ được phân tách bằng dấu chấm phẩy.

![image](/images/Screenshot_52.png)
### Bước 9. Chỉ định cài đặt xử lý khách

![image](/images/Screenshot_53.png)
### Bước 10. Xác định lịch trình công việc

Chọn hộp kiểm **Run the job automatically**. Nếu hộp kiểm này không được chọn, bạn sẽ phải bắt đầu công việc theo cách thủ công để tạo bản sao lưu VM. Hình bên dưới là thực hiện 4 ngày thứ 7 trong tháng vào lúc 10 giờ tối

Phần **Automatic retry** xác định xem Veeam Backup & Replication có phải cố gắng chạy lại công việc sao lưu hay không nếu công việc không thành công vì lý do nào đó. Trong quá trình thử lại công việc, quy trình Sao lưu & nhân bản của Veeam chỉ các máy ảo không thành công. Nhập số lần thử thực hiện công việc và xác định khoảng thời gian giữa chúng. Nếu bạn chọn sao lưu liên tục, Veeam Backup & Replication sẽ thử lại công việc trong số lần xác định mà không có bất kỳ khoảng thời gian nào giữa các lần chạy công việc.


![image](/images/Screenshot_54.png)
### Bước 11 Kết thúc làm việc

Chọn hộp kiểm Run the job when I click Finish nếu bạn muốn bắt đầu công việc ngay sau khi kết thúc thao tác với trình hướng dẫn.

![image](/images/Screenshot_55.png)