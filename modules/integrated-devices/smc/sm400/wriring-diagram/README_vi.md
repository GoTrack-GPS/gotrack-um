
# Sơ đồ đấu dây

### 1. Sơ đồ đấu dây của đầu ghi hình SD

&emsp;<span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/diagram-sd.png)

### 2. Sơ đồ đấu dây của đầu ghi hình HDD

&emsp;<span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/diagram-hdd.png)

### 3. Thiết lập nhanh

#### 3.1. Kiểm tra dây và khởi động

* Nguồn điện của máy chủ có ba dây, màu đỏ, đen và vàng. Dây màu đỏ và đen được nối trực tiếp với ắc quy ô tô, dây màu đỏ nối với điện cực dương, dây màu đen nối với điện cực âm, dây màu vàng nối với dây đánh lửa (ACC). Nếu bạn thử nghiệm trong nhà, dây màu đỏ và màu vàng có thể được kết nối với nhau. Cực dương, sau đó sử dụng trực tiếp nguồn điện DC12V.
  
  **1.** Kiểm tra xem dây nguồn được kết nối bình thường và xác nhận rằng khối chìa khóa đã được bật vào tệp LOCK sau khi đường dây được kết nối, sau đó nó sẽ khởi động bình thường và đèn nguồn sẽ có màu xanh lam sau khi khởi động bình thường.

   **2.** Kết nối đường ra AV-OUT với màn hình hiển thị và kết nối thiết bị tương ứng với thiết bị đầu cuối. Xác nhận xem kết nối có đúng không. Hình dưới đây cho thấy hệ thống dây cấp nguồn lắp đặt thực tế :

&emsp;<span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/power-cable.png)

&emsp;<span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/car-battery.png)

#### 3.2. Xe nhanh chóng báo về máy chủ

> Lưu ý: Đối với các máy chủ không có chức năng mô-đun WIFI và 3G, các mô tả sau đây không hợp lệ và không cần phải báo cáo cho nền tảng.

* Bước 1: Lắp thẻ SIM, chọn thẻ SIM theo mô-đun tương ứng.
  
* Bước 2: Khởi động vào menu hệ thống, trước tiên hãy sửa đổi số điện thoại di động trong cài đặt thiết bị đầu cuối (đó là ID duy nhất của máy chủ báo cáo) và sau đó sửa đổi biển số xe tương ứng.
  
* Bước 3: Nhập các cài đặt mạng quan trọng, sửa đổi IP và số cổng tương ứng theo IP triển khai máy chủ khác nhau của từng khách hàng, và chọn nền tảng của giao thức chuẩn, chọn máy chủ GPS chính trên trang tiếp theo để sửa đổi IP và số cổng.

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/terminal-sv-.png)

#### 3.3. Sử dụng cổng nối tiếp IO

* Thiết bị có 4 đầu vào cảnh báo và 2 giao diện đầu ra cảnh báo. Phát hiện đầu vào cảnh báo là phát hiện tất cả các mức, có thể được kết nối với các trạng thái lái xe khác nhau, chẳng hạn như phanh, lái, chuyển xe và nút cảnh báo, như thể hiện trong Hình 4-2. 
  
    &emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/+12V.png)

* Khi đạp đĩa phanh, MDVR có thể bảo vệ mức cao, nếu không mức thấp, đầu ra cảnh báo là tất cả đầu ra mức và dung lượng ổ đĩa là 200mA. Nếu bạn kết nối một thiết bị công suất lớn hơn, bạn phải kết nối một rơ le. Như trong Hình 4-3:
  
    &emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/24V.png)


#### 3.4. Kết nối PTZ và cài đặt

* Các bước thiết lập:
  
   * **Đầu tiên** ： chọn giao thức PTZ: PELCO-D và PELCO-P tương ứng.
   * **Thứ hai** ： đặt tốc độ truyền và chọn nó trên thiết bị đầu cuối theo tốc độ truyền tương ứng của PTZ.
   * **Thứ ba** ： đặt mã địa chỉ: nhập trực tiếp mã địa chỉ tương ứng với giá trị địa chỉ PTZ.
   * **Thứ tư** đấu dây: dây điều khiển 485 trên PTZ được kết nối với RS485-A dương, dây còn lại Kết nối với RS458-B âm.

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/method1.png)

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/method2.png)


