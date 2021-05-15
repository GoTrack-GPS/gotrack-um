# Cấu hình kết nối cảm biến dầu Soji

### 1. S400, S200

#### 1.1. Nối dây

* RX của Cảm Biến --> TX của S200/S400: Màu vàng

* TX của Cảm Biến --> RX của S200/S400: Màu Xanh

#### 1.2. Cấu hình

* Cảm biến soji bán ra nước ngoài dùng baudrate 19200
    
    **Rs232,0,2,19200#**

* Cảm biến soji bán tại Việt Nam dùng baudrate 9600

    **Rs232,0,2,9600#**

* Gửi lệnh **reset#** để lưu và cập nhật cấu hình

### 2. TG102LE

#### 2.1. Nối dây

* RX của Cảm Biến --> TX của S200/S400: Màu vàng

* TX của Cảm Biến --> RX của S200/S400: Màu Trắng

#### 2.2. Cấu hình

* Cảm biến soji bán ra nước ngoài dùng baudrate 19200
    
    **#w49 8,019200.***
* Cảm biến soji bán tại Việt Nam dùng baudrate 9600

    **#w49 8,009600.***

* Gửi lệnh **#w00.*** để lưu và cập nhật cấu hình

> __cần reset thiết bị bằng lệnh sau khi thực hiện cấu hình__
