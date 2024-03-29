# Sửa thiết bị:
Để bắt đầu thực hiện chức năng **Sửa**, người dùng vào **Quản lý > Thiết bị** 

 <span class="icon-left4">![Manage device ](/docs/assets/images/web-interface/device/manage-device-1.png)

  
Khi click vào  <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-edit.svg) **Sửa** của thiết bị đó, sẽ xuất hiện hộp thoại như sau: 

<div id="suathietbi">
</div>


<span style="display:block;text-align:left">![search device ](/docs/assets/images/web-interface/device/edit-device-basic-1.png)

### Cơ bản 

- ***Thông tin thiết bị*** 
    - **IMEI**: Mã số nhận dạng của thiết bị. (Không cho phép sửa).
    - **Tài khoản**: Tên tài khoản/ tên đăng nhập của bạn. (Không cho phép sửa).
    - **Biểu tượng**: Click vào ô ngay dưới để chọn biểu tượng xe/phương tiệ    mà mình lắp thiết bị. 
    - **Số SIM**: Nhập số điện thoại bạn đang sử dụng.
    - **Tên thiết bị**: Có thể thay đổi tên thiết bị cho dễ nhớ, dễ nhìn.
    - **Loại thiết bị**: Chọn tên loại thiết bị tương ứng đúng với thiết bị mình đang sử dụng.
    - **Nhóm thiết bị**: Là nhóm các thiết bị có chung một điểm nào đó với nhau trong một tài khoản.
        
        <span style="display:block;text-align:left">![search device ](/docs/assets/images/web-interface/device/Add-a-device-group.png)
    
        
        - Bước 1: Click  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) để thêm nhóm  thiết bị.
        - Bước 2: Chọn tài khoản muốn thêm nhóm thiết bị. Nhập tên nhóm thiết bị.
        - Bước 3: Click vào **Thêm** để hoàn thành thao tác.

            Ngoài ra, có thể tạo thêm nhóm thiết bị bằng cách như hình dưới đây: 

            <span style="display:block;text-align:left">![search device ](/docs/assets/images/web-interface/device/Add-a-device-group-2.png)
        
        Tham khảo thêm chi tiết [tại đây](vi/modules/web-interface/configuration/device-group/#device-group) <div id="device-group" >

    - **Loại SIM**: Chọn loại SIM tương ứng với nhà mạng của số điện thoại.
- ***Dịch vụ***  
    - **Hạn dịch vụ** : Hạn sử dụng dịch vụ.
    - **Kích hoạt** : Có thể bật / tắt khi muốn / không muốn sử dụng dịch vụ.
- ***Bảo hành*** 
    - **Kích hoạt bảo hành**: Có thể bật/tắt.
    - **Ngày kích hoạt bảo hành**: Ngày bật kích hoạt bảo hành thiết bị.
    - **Hạn bảo hành**: Ngày hết hạn bảo hành thiết bị theo gói bảo hành của dịch vụ đó.
- ***Ghi chú***  
    - **Tổng quãng đường (km)** : Khi xe chạy hết ngày sẽ tự động tính tổng quãng đường mà xe đã chạy từ trước tới ngày hôm qua.
      - Nếu sửa về số khác, thì nó sẽ tính thêm từ số đó với số km đã chạy tính từ thời điểm sửa đó.
    - **Thời gian nổ máy (giờ)** : Nếu chọn đúng tín hiệu động cơ (Khóa điện/động cơ) mà khi lắp thiết bị thì sẽ tự động tính thời gian nổ máy.
      - Nếu sửa về số khác, thì nó sẽ tính thêm từ số đó với số km đã chạy tính từ thời điểm sửa đó.
    - **Ghi chú** : Nhập ghi chú nếu bạn muốn chú thích điều gì đó.
    - **Ghi chú (quản lý)** : Chỉ tài khoản **Đại lý** mới hiển thị textbox này và có quyền nhập ghi chú.
    - **Phiên bản** : Nhập phiên bản firmware khi xuất kho.
- ***Thông tin bán***  
    - **Đã bán** : Khi thiết bị đã bán sang tài khoán sẽ tự động bật. Nếu chư   bán sẽ ỏ chế độ tắt.
    - **Ngày bán** : Cài đặt ngày bán thiết bị sang tài khoản khác (nếu có).
    - **Ngày cập nhật** : Hệ thống tự động cập nhật ngày bán thiết bị khi có thay đổi .

<div id="advanced">
</div>

### Nâng cao 
  
<span class="icon-left9">![search device ](/docs/assets/images/web-interface/device/advanced-device.png)  

- ***Thông tin xe*** 
    - **Biển số** : Biến số xe mà đã lắp thiết bị định vị. Biển số phải nhập đúng định dạng : **Viết liền, có cả chữ và số** thì mới trên lên Tổng cục đường bộ.  
    - **Số VIN** : Số khung xe gồm 17 ký tự. (Dành cho oto).
    - **Hệ số quãng đường** : Là khoảng cách tính bằng km trong 1 đơn vị vectơ  Theo mặc định, hệ số khoảng cách là 1,0.
    - **Số khung** : Là số nhận dạng xe. Một chuỗi seri và kí tự được đục trê   khung xe. (Dành cho xe máy).
    - **Số máy** : Số máy xe của bạn. (Dành cho xe máy).
    - **Lái xe**: Tên người lái xe của xe/phương tiện đã lắp thiết bị định vị.
        Nếu chưa có thì click vào <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)

        <span style="display:block;text-align:left">![search device ](/docs/assets/images/web-interface/device/add-a-driver.png)

        - **Tài khoản** : Tên tài khoản muốn thêm người lái xe.
        - **Tên** : Tên người lái xe lắp thiết bị.
        - **Số điện thoại** : Số điện thoại người lái xe.
        - **Giấy phép lái xe** : Hạng giấy phép lái xe.
        - **Ngày cấp phép** : Ngày cấp giấy phép lái xe.
        - **Ngày hết hạn** : Ngày hết hạn sử dụng giấy phép lái xe.
        - **Mã** : Mã giấy phép lái xe.
        - **Email** : Email của người lái xe.
        - **Địa chỉ** : Địa chỉ của người lái xe.
        - **Mô tả** : Mô tả thêm thông tin cần thiết,...

        Click vào **Thêm** để lưu người lái xe.

    Ngoài ra, có thể thêm người lái xe bằng cách như hình dưới đây :
    <span style="display:block;text-align:left">![search device ](/docs/assets/images/web-interface/device/add-a-driver-2.png)

     Tham khảo thêm chi tiết [tại đây](vi/modules/web-interface/configuration/driver/#driver) <div id="driver">

- ***Nhiên liệu*** 
    - **Định mức tiêu hao (lít/100km)** : Đặt giới hạn tiêu hao nhiên liệu của xe cho bao nhiêu lít/100km.
- ***Tính năng nâng cao*** 
    - **Trạm thu phí** : Có thể bật / tắt. Khi bật lên khi xe qua các trạm thu phí sẽ cảnh báo và tương ứng với loại hình vận tải thì sẽ tính được xe mất bao nhiêu phí khi đi qua.
    - **Loại hình vận tải** : Chọn 1 trong 5 loại hình vận tải.(Chỉ áp dụng ở Việt Nam)
    <span class="icon-left4">![delete device](/docs/assets/images/web-interface/device/Price-list.png)

- ***Bộ Giao thông vận tải***
    - **Gửi dữ liệu**: Có thể  bật / tắt. Chỉ khi nào bật lên dữ liệu mới trên lên Tổng cục đường bộ.
    - **Sở Giao thông vận tải** : Chọn tỉnh để gửi dữ liệu. (Chỉ chọn đượkhi bật chế độ gửi dữ liệu).
    - **Loại hình vận tải QVCN** : Chọn 1 trong các loại hình đó, đúng với xe / phương tiện mà bạn lắp thiết bị. (Chỉ chọn được khi bật chế độ gửi dữ liệu).

<div id="sensor">
</div>

### Cảm biến 


* Trước khi thêm cảm biến mới, hãy xem sơ đồ bên dưới, cách các thông số được gửi từ thiết bị gps và cách chúng cần được ghép nối với các cảm biến.

    <span class="icon-left6">![delete device](/docs/assets/images/web-interface/device/sensor-device-1.png)

* Khi click vào  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)**Thêm cảm biến** , sẽ xuất hiện hộp thoại như sau:  

    <span class="icon-left6">![delete device](/docs/assets/images/web-interface/device/Sensor-device.png)
    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/advanced-sensor-device.png)

#### Cơ bản 

- **Tên cảm biến** : Đặt tên cảm biến cho dễ nhớ, dễ nhìn. 
- **Phương pháp tính**: Chọn 1 trong 3 phương pháp:  Calibration (Hiệuchuẩn), Linear (tuyến tính), Original (Nguyên bản). 
- **Tham số**: Chọn tham số tương ứng.
- **Đơn vị**: Chọn đơn vị cần đo .
- **Loại cảm biến** : Chọn loại cảm biến tương ứng với đơn vị đo. 
- **Công thức** : Nhập giá trị đúng như ví dụ (Chỉ xuất hiện khi chọn phương pháp  Linear (tuyến tính), Original (Nguyên bản)
- **Tối thiểu**  : Nhập giá trị nhỏ nhất của hiệu chuẩn.
- **Tối đa**: Nhập giá trị lớn nhất của hiệu chuẩn.

#### Nâng cao

-  **Tăng tối thiểu** : Nhập giá trị cảm biến thay đổi khi tăng bất thường.
-  **Giảm tối thiểu** : Nhập giá trị cảm biến thay đổi khi giảm bất thường.
-  **Cân đối bù trừ** : Nhập giá trị chỉnh "không" khi tính toán ra ADC để xuất ra giá trị nhiệt độ(loại cảm biến) đúng.
- **Làm tròn** : Làm tròn giá trị cảm biến bao nhiêu đó sau dấu (,).
- **Sắp xếp**: Sắp xếp giá trị cảm biến thay đổi lên vị trí nào. 
- **Mô tả** : Có thể ghi thêm thông tin về cảm biến,...
- **Hiển thị bản đồ trên map** : Bật / tắt để hiển thị / không hiển thị tên cảm biến trên bản đồ. 

Click **Thêm** để lưu cảm biến. 

### Camera 

#### Đối với loại camera : Basic
    
<span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/add-camera-1.png)

* Khi click vào  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)**Thêm camera** xuất  hiện hộp thoại như hình trên: 
  - **Tên** : Nhập tên camera  theo đúng kênh cắm ở đầu ghi.
  - **Loại camera** : **Basic** ( thường ). Chỉ chụp ảnh.
  - **Camera Id** : Nhập mã của camera. ID ghi trên thiết bị SM400
  - **Mô tả** : Có thể nhập thêm thông tin về camera,...

<div id="cameraplay">
</div>

#### Đối với loại camera : MDVR

<span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/add-camera-7.png)

* Khi click vào  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)**Thêm camera** xuất  hiện hộp thoại như hình trên: 
  - **Tên** : Nhập tên vị trí camera bạn muốn lắp đặt.
  - **Loại camera** : **MDVR**. Ngoài chụp ảnh ra còn có thêm tính năng quay video.
  - **MDVR Id** : ID in trên thiết bị SM400.
  - **Host** : Địa chỉ IP hoặc tên miền truy cập server camera.
  - **Cổng** : Cổng kết nối đến đầu ghi hình camera. Mặc định là 6605.
  - **Kênh** : Dây nối camera cắm vào cổng của kênh nào thì chọn kênh đó. 
    - Vị trí kênh lắp ở đầu ghi, **AV1  <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  AV4**. (Đối với đầu ghi 8 kênh thì <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  **AV8** ). 
    - Tương ứng từ **CH1 <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) CH8**
    -  Chỉ được tạo 1 kênh duy nhất. 
  - **Vị trí** : Đối với các xe truyền dữ liệu lên Bộ Giao thông vận tải bắt buộc phải lắp camera tại 3 vị trí sau :
      - **Lái xe** : Vị trí nhìn thấy người lái xe, tài xế.
      - **Cửa** :  Vị trí  hành khách đi lên -  xuống xe.
      - **Hành khách** : Vị trí bao quát hết các hành khách đang trên xe.
  - **Mô tả** : Có thể nhập thêm thông tin về camera,...
  - **Nhân bản** : Nếu muốn tạo nhiều kênh cùng 1 lúc thì chọn nhân bản, sao chép bằng đó kênh. Để tiết kiệm thời gian và tạo kênh nhanh hơn. Khi nhân bản thành công chỉ cần chọn lại số kênh.
    
Click **Thêm** để lưu camera.

> Bên nhân viên kỹ thuật sẽ cấu hình địa chỉ  MDVR Id, host, cổng cho thiết bị.

### Mở rộng

<span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/expand-device.png)

- ***Cấu hình*** 
    - **Thời gian chờ GPRS (phút)** : Cấu hình thời gian không sử dụng thiết bị (offline) , nhỏ  hơn số đó là thiết bị vẫn đang hoạt động.
    - **Thời gian dừng (giây)** : Cấu hình thời gian xe dừng tối thiểu. Nếu lớn hơn hoặc bằng thời gian dừng sẽ được tính là 1 điểm dừng.
    - **Lọc tốc độ tối thiểu (km/h)** : Lọc độ nhiễu chính xác nhất. Để xác định được xe đang dừng/ đi. 
      - Nếu xe có tốc độ < Lọc tốc độ tối thiểu ( km/h) thì sẽ là tính xe đang dừng.
    - **Múi giờ**: Chọn múi giờ địa phương.
    - **Lưu dữ liệu thô** : Dữ liệu thô là dữ liệu máy tính chưa qua xử lý. Thông tin này có thể được lưu trữ trong một tệp, hoặc có thể chỉ là một tập hợp các số và ký tự được lưu trữ trên một nơi nào đó trong đĩa cứng của máy tính. Bật nếu cần.
    - **Tín hiệu động cơ** : Là tín hiệu khi lắp thiết bị là nối dây acc/engine.
    Ngoài ra, có thể cấu hình thiết bị bằng cách như hình dưới đây :

    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/device-configuration.png)

### Cảnh báo


<span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/warning-device.png)

Tick <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square1.svg) để bật/tắt các cảnh báo thiết bị mà bạn muốn gửi cảnh báo về.

Ngoài ra, có thể cấu hình thông báo thiết bị bằng cách như hình dưới đây :

<span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/device-notification-configuration.png)

Sau khi sửa xong các thông tin, click **Lưu thay đổi** để hoàn thành thao tác.

