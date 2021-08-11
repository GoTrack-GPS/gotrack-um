
# Hướng dẫn Gửi lệnh kiểm tra kết nối cảm biến trên app GoTrack365

Tính năng gửi lệnh này chỉ dành cho : 
- Tài khoản loại Distributor. 
- Thiết bị S400.

Để  gửi lệnh, thực hiện các bước sau : 

<span class="icon-left5">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/send-command-s400-1.jpg)

- Bước 1 : 
    - Đăng nhập vào tài khoản loại Distributor.
    - Tìm kiếm thiết bị muốn gửi lệnh . 
    - Sau đó chọn thiết bị muốn gửi lệnh ở màn hình **Phương tiện**.

- Bước 2 : Trượt menu ngang để chọn **Gửi lệnh**.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/send-command-s400-2.jpg)

- Bước 3 : Cấu hình baudrate 
    - Click vào <span style="color:orange"> @</span> trên màn hình.
    - Chọn lệnh mẫu : **Cài đặt baud rate**. Tên lệnh sẽ tự động hiện ra màn hình.

    > **< RS232 > : là vị trí cổng RS232, 0 là RS232_0 ở port A , 1 là RS232_1 ở port B <br>
    < SENSOR > : là loại cảm biến, trong đó 2 là SOJI**
    
    Thay các giá trị theo công thức hiện trên màn hình.
    - Cảm biến soji bán ra nước ngoài dùng baudrate 19200

        **Rs232,0,2,19200#**

    - Cảm biến soji bán tại Việt Nam dùng baudrate 9600

        **Rs232,0,2,9600#**
    -  Ấn  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) để Gửi lệnh.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/send-command-s400-3.jpg)

- Bước 4 : Kiểm tra tần suất đọc dữ liệu
    
    - Click vào <span style="color:orange"> @</span> trên màn hình.
    - Chọn lệnh mẫu : **Cài đặt tần suất cập nhật cảm biến**. Tên lệnh sẽ tự động hiện ra màn hình.
        
    Thay các giá trị theo công thức hiện trên màn hình.

    - Tần suất đọc dữ liệu từ cảm biến. Mặc định là 10s và 5 đơn vị
    
        **rs232para,0,10,5#**

    -  Ấn  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) để Gửi lệnh.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/send-command-s400-4.jpg)

- Bước 5 : Lưu cấu hình

    - Click vào <span style="color:orange"> @</span> trên màn hình.
    - Chọn lệnh mẫu : **Khôi phục mặc định**. Tên lệnh sẽ tự động hiện ra màn hình.
    - Ấn  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) Gửi lệnh để lưu và cập nhật cấu hình.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/send-command-s400-5.jpg)

- Bước 6 : Kiểm tra chỉ số cảm biến

    Đợi vài phút.

    - Click vào <span style="color:orange"> @</span> trên màn hình.
    - Chọn lệnh mẫu : **Kiểm tra trạng thái ngoại vi**. Tên lệnh sẽ tự động hiện ra màn hình.
    - Ấn  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) để Gửi lệnh.


- Bước 7 : Yêu cầu thiết bị gửi cập nhật chỉ số lên web

    <span class="icon-left4">![Interface Web](/docs/assets/images/web-interface/app-gotrack365/send-command-sms/press-command.jpg)
    
    - Khi mà trên thiết bị đã đọc được chỉ số cảm biến, nhưng trên web chưa thấy cập nhật giá trị, thì có thể dùng lệnh sau để yêu cầu thiết bị gửi chỉ số cảm biến ngay. 
    
        Điền lệnh sau vào ô **Nhập lệnh** :

        **pack,sensor#**
    
    
> Nếu thiết bị set **cổng 140.40** thì khi phản hồi sẽ tự động update trong hội thoại. <br>
Nếu không set cổng trên thì sẽ phải click vào icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-refresh.svg)  để làm mới dữ liệu.
    
    
    