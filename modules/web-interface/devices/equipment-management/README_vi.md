# Quản lý thiết bị
Sau khi thêm thiết bị xong, người dùng có thể tìm kiếm/sửa/đổi mật khẩu/xóa thiết bị.
# 1. Tìm kiếm thiết bị:
Có thể tìm kiếm theo các tiêu chí sau:

<span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/search-device.png)

- Tìm kiếm theo **IMEI / Tên thiết bị / Mã máy/Biến số** : Người dùng có thể nhập cả tên hoặc một vài ký tự có trong IMEI / Tên thiết bị / Mã máy/Biến số đã thêm. Chọn **Tìm kiếm** sẽ hiển thị ra kết quả cần tìm.
- Tìm kiếm theo **Tài khoản con** : Bạn có thể tick vào ô vuông (□) đó, chọn **Tìm kiếm** để hiển thị thêm tất cả các thiết bị mà tài khoản con đã thêm.
- Khi click vào **Tìm kiếm nâng cao** sẽ hiện thị thêm các tiêu chí như hình dưới đây:

<span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/advanced-search.png)

<p> &emsp;&emsp;&emsp;  - Có thể tìm kiếm theo :
<p>
  &emsp;&emsp;&emsp;&emsp;  + <b> Loại thiết bị / Số sim / Loại sim </b> : Loại thiết bị / Số điện thoại / Loại sim đã đăng ký khi thêm thiết bị trước đó. </p>
  &emsp;&emsp;&emsp;&emsp;  + <b>Hạn dịch vụ / Trạng thái kích hoạt / Trạng thái </b>: Thời gian sử dụng dịch vụ / Trạng thái kích hoạt / Trạng thái thiết bị

- <b>Đặt lại </b> : Sẽ xóa đi các ký tự bạn vừa nhập để tìm kiếm và hiển thị lại theo chế độ mặc định ban đầu.

# 2. Sửa thiết bị:
Khi click vào icon **Sửa** của thiết bị đó, sẽ xuất hiện hộp thoại như sau: 
* **Cơ bản**:<br>
    <span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/edit-device-basic-1.png)
    <span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/edit-device-basic-2.png)

    - ***Thông tin thiết bị***: 
        - **IMEI**: Mã số nhận dạng của thiết bị. (Không cho phép sửa).
        - **Tài khoản**: Tên tài khoản/ tên đăng nhập của bạn. (Không cho phép sửa).
        - **Biểu tượng**: Click vào ô ngay dưới để chọn biểu tượng xe/phương tiện mà mình lắp thiết bị. 
        - **Số SIM**: Nhập số điện thoại bạn đang sử dụng.
        - **Tên thiết bị**: Có thể thay đổi tên thiết bị cho dễ nhớ, dễ nhìn.
        - **Loại thiết bị**: Chọn tên loại thiết bị tương ứng đúng với thiết bị mình đang sử dụng.
        - **Nhóm thiết bị**: Là nhóm các thiết bị có chung một điểm nào đó với nhau trong một tài khoản.
         
     <span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/Add-a-device-group.png)

            - Bước 1: Chọn tài khoản muốn tạo nhóm thiết bị.
            - Bước 2: Nhập tên nhóm thiết bị.
            - Bước 3: Click vào **Thêm** để hoàn thành thao tác.

        - **Loại SIM**: Chọn loại SIM tương ứng với nhà mạng của số điện thoại.
    - ***Dịch vụ***:   
        - **Hạn dịch vụ** : Hạn sử dụng dịch vụ.
        - **Kích hoạt bảo hành**: Có thể bật/tắt.
        - **Ngày kích hoạt bảo hành**: Ngày bật kích hoạt bảo hành thiết bị.
        - **Hạn bảo hành**: Ngày hết hạn bảo hành thiết bị theo gói bảo hành của dịch vụ đó.
     -  **Ghi chú**: Nhập ghi chú nếu bạn muốn chú thích điều gì đó.


- **Nâng cao :**  
  
    <span style="display:block;text-align:center">![search device ](/docs/assets/images/web-interface/web-interface-device/advanced-device.png)  
    - ***Thông tin xe*** : 
        - **Biển số** : Biến số xe mà đã lắp thiết bị định vị.      
        - **Số VIN** : Số khung xe gồm 17 ký tự. (Dành cho oto).
        - **Hệ số quãng đường** : Là khoảng cách tính bằng km trong 1 đơn vị vectơ. Theo mặc định, hệ số khoảng cách là 1,0.
         - **Số khung** : Là số nhận dạng xe. Một chuỗi seri và kí tự được đục trên khung xe. (Dành cho xe máy).
         - **Số máy** : Số máy xe của bạn. (Dành cho xe máy).
         - **Lái xe**: Tên người lái xe của xe/phương tiện đã lắp thiết bị định vị.
    - ***Nhiên liệu*** :
        - **Định mức tiêu hao (lít/100km)** : Đặt giới hạn tiêu hao nhiên liệu của xe cho bao nhiêu lít/100km.
    - ***Tính năng nâng cao*** :
        - **Trạm thu phí** : Có thể bật / tắt. Khi bật lên khi xe qua các trạm thu phí sẽ cảnh báo và tương ứng với loại hình vận tải thì sẽ tính được xe mất bao nhiêu phí khi đi qua.
        - **Loại hình vận tải** : Chọn 1 trong 5 loại hình vận tải.(Chỉ áp dụng ở Việt Nam)
<span style="display:block;text-align:center">![delete device](/docs/assets/images/web-interface/web-interface-device/Price-list.png)

    - ***Bộ Giao thông vận tải***
        - **Gửi dữ liệu**: Có thể  bật / tắt.
        - **Sở Giao thông vận tải** : Chọn tỉnh để gửi dữ liệu. (Chỉ chọn được khi bật chế độ gửi dữ liệu).
        - **Loại hình vận tải QVCN** : Chọn 1 trong các loại hình đó. (Chỉ chọn được khi bật chế độ gửi dữ liệu).
- **Cảm biến :** 

 <span style="display:block;text-align:center">![delete device](/docs/assets/images/web-interface/web-interface-device/Sensor-device.png)
 
 <p> &emsp;&emsp; Khi click vào <b>Thêm cảm biến</b> , sẽ xuất hiện hộp thoại như sau: </P>

 <span style="display:block;text-align:center">![delete device](/docs/assets/images/web-interface/web-interface-device/advanced-sensor-device.png)

<p>  
&emsp;&emsp;&emsp; <b>-  Cơ bản :</b> <br>
 &emsp;&emsp;&emsp;&emsp;   + <b>Tên cảm biến</b> : Đặt tên cảm biến cho dễ nhớ, dễ nhìn. <br>
 &emsp;&emsp;&emsp;&emsp;   + <b>Phương pháp tính</b>: Chọn 1 trong 3 phương pháp:  Calibration (Hiệu chuẩn), Linear (tuyến tính), Original (Nguyên bản). <br>
 Calibration (Hiệu chuẩn), là phương pháp để truyền độ lớn của đơn vị đo lường từ chuẩn có độ chính xác cao nhất tới các phương tiện đo thông thường.<br>


 &emsp;&emsp;&emsp;&emsp;   + <b>Tham số</b>: Chọn tham số tương ứng.<br>
 &emsp;&emsp;&emsp;&emsp;   + <b>Đơn vị</b>: Chọn đơn vị cần đo .<br>
 &emsp;&emsp;&emsp;&emsp;   + <b>Tham số</b>: Chọn loại cảm biến tương ứng với đơn vị đo. <br>
&emsp;&emsp;&emsp;&emsp;   + <b>Hiệu chuẩn </b> : Nhập giá trị đúng như ví dụ (Chỉ xuất hiện khi chọn phương pháp  Calibration (Hiệu chuẩn)<br>
&emsp;&emsp;&emsp;&emsp;&emsp;<b>Công thức</b> : Nhập giá trị đúng như ví dụ (Chỉ xuất hiện khi chọn phương pháp  Linear (tuyến tính), Original (Nguyên bản)<br>
&emsp;&emsp;&emsp;&emsp;   + <b>Tối thiểu </b> : Nhập giá trị nhỏ nhất của hiệu chuẩn.<br>
&emsp;&emsp;&emsp;&emsp;   + <b>Tối đa</b>: Nhập giá trị lớn nhất của hiệu chuẩn.<br>
&emsp;&emsp;&emsp; <b>-  Nâng cao :</b> <br>
&emsp;&emsp;&emsp;&emsp;   + <b>Tối đa</b>:
 </p>



Click **Lưu thay đổi** để hoàn thành thao tác.
# 3. Xóa thiết bị:
CLick  vào icon **Xóa** của thiết bị, sẽ xuất hiện một hộp thoại như hình dưới đây:

<span style="display:block;text-align:center">![delete device](/docs/assets/images/web-interface/web-interface-device/delete-device.png)

Nếu:
- Chọn **Xác nhận**: Sẽ xóa thiết bị đó.
- Chọn **Hủy**: Sẽ hủy thao tác xóa.
