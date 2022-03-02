# Hướng dẫn tạo máy ảo giả lập thiết bị NAS Synology
Trước khi thiết lập tải file sau về và giải nén.[Link tải](https://drive.google.com/drive/folders/1GTUyKcog-JNJ5UiRNxoZKauasqqRo3qi)

Sau khi giải nén sẽ được 2 file vmdk và pat. dùng để thiết lập các bước bên dưới.S

Tạo một máy ảo mới trên VMware Workstarion
</br>![Imgur](https://i.imgur.com/DS3Qsyu.png)</br>
Chọn phiên bản cho VMware
</br>![Imgur](https://i.imgur.com/mz4K4gH.png)</br>
Cài đặt một OS đã tạo từ trước
</br>![Imgur](https://i.imgur.com/5haqbBe.png)</br>
Hệ điều hành Linux -> Other Linux 2.4.x kernel 
</br>![Imgur](https://i.imgur.com/2KDnikU.png)</br>
Đặt tên cho máy ảo
</br>![Imgur](https://i.imgur.com/pBADaWS.png)</br>
Set Processors
</br>![Imgur](https://i.imgur.com/h1JMkDC.png)</br>
Set ram
</br>![Imgur](https://i.imgur.com/5HzPuBM.png)</br>
Set I/O controller
</br>![Imgur](https://i.imgur.com/spv6Lr9.png)</br>
Sử dụng loại DISK
</br>![Imgur](https://i.imgur.com/VYQHAmZ.png)</br>
Bước này sẽ chọn File mà bạn đã tải về ở bước đầu tiên
</br>![Imgur](https://i.imgur.com/nkVn0Js.png)</br>
Chọn file
</br>![Imgur](https://i.imgur.com/uvnTZAW.png)</br>
Chọn file VMDK
</br>![Imgur](https://i.imgur.com/ZXVZcHD.png)</br>
Next 
</br>![Imgur](https://i.imgur.com/WnYpDy1.png)</br>
Giữ nguyên định dạng disk 
</br>![Imgur](https://i.imgur.com/DU8j7WX.png)</br>
Sau khi thiết lập máy ảo xong bật máy ảo. Lưu ý máy ảo phải được đặt ở dải mạng có DHCP, Đối với NAS Synology vật lý cũng vậy. Sau đó truy cập trang [find.synology.com](find.synology.com)
</br>![Imgur](https://i.imgur.com/pEWxxIn.png)</br>
sau đó sẽ hiện thị thiết bị để cài đặt
</br>![Imgur](https://i.imgur.com/BEvBjk9.png)</br>

</br>![Imgur](https://i.imgur.com/bFuOC1X.png)</br>

</br>![Imgur](https://i.imgur.com/sT4WMDG.png)</br>

</br>![Imgur](https://i.imgur.com/NmRrMuO.png)</br>
Chọn Set manual
</br>![Imgur](https://i.imgur.com/Zew2ccC.png)</br>
Chọn file đuôi .PAT
</br>![Imgur](https://i.imgur.com/ke3Z4gi.png)</br>

</br>![Imgur](https://i.imgur.com/8MtOlrg.png)</br>

</br>![Imgur](https://i.imgur.com/BYUBD5M.png)</br>
Đây là giao diện sau khi đã cài đặt thành công.
</br>![Imgur](https://i.imgur.com/xqx44Eh.png)</br>