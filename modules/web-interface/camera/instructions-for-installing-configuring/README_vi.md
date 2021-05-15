# Hướng dẫn cài đặt và sử dụng MDVR (SM400)

### Bước 1 : Chuẩn bị phần cứng 
- Thiết bị đầu ghi SM400 Basic hoặc Livestream.
- Thiết bị hợp chuẩn QCVN31 S200 hoặc S400.
- Camera. 
-  Sim 4G cho thiết bị đầu ghi SM400 livestream (nếu có).
(Thiết bị đầu ghi SM400 base không cần).
- Sim 4G cho thiết bị hợp chuẩn QCVN31.
- Dây nguồn kết nối thiết bị hợp chuẩn và đầu ghi.
- Và các phụ kiện khác đi kèm : thẻ RFID, thẻ nhớ SD card, antena GPS, GSM (nếu có).

* **Các thiết bị để cài SM400 Basic như hình dưới đây :**

    <span class="icon-left6">![Manage device ](/docs/assets/images/web-interface/livestream/mdvr-photo.jpg)

* **Các thiết bị để cài SM400 Livestream như hình dưới đây :**

    <span class="icon-left6">![Manage device ](/docs/assets/images/web-interface/livestream/mdvr-live.jpg)

### Bước 2 : Nối dây

- Áp dụng cho cả thiết bị đầu ghi SM400 Basic và Livestream
    - Cắm dây có đầu nối thiết bị hợp chuẩn QCVN với đầu ghi SM400.
   
    <span class="icon-left16">![Manage device ](/docs/assets/images/web-interface/livestream/connect-sm400-s200.jpg)

    - Cắm camera vào đầu ghi theo thứ tự từ AV1  <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  AV4
    - Lắp thẻ nhớ SD vào đầu ghi SM400 .
    - Lắp sim 4G (chỉ dành cho SM400 livestream) vào đầu ghi SM400.
    - Nối đầu ghi SM400 vào màn hình để cấu hình.
    - Bật nguồn đầu ghi SM400.

### Bước 3 : Cấu hình đầu ghi

**(Chỉ áp dụng cho SM400 Livestream)**

* **Cài đặt IP máy chủ camera**

    <span class="icon-left4">![Manage device ](/docs/assets/images/web-interface/livestream/ip-camera.jpg)

* **Cài đặt chế độ lưu video**
  
* **Cài đặt video: cài đặt cơ bản, cài đặt luồng chính, cài đặt luồng phụ, cài đặt thời gian, quản lý bộ nhớ, cài đặt OSD**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/record.png)

  * **Cài đặt cơ bản: cài đặt thông số ghi cơ bản**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/general.png)

    * Định dạng video: PAL, NTSC, nhấn phím 【OK】 để chọn từ menu thả xuống.
    * Chế độ video: video khởi động, video hẹn giờ, video báo động, ghi hình khởi động: bắt đầu quay tự động khi thiết bị được bật recording Ghi hình theo thời gian: bắt đầu ghi trong khoảng thời gian ghi định thời và không ghi vào những thời điểm khác. Ghi âm báo thức: thiết bị bắt đầu ghi khi có báo động.
    * Định dạng âm thanh: G726-M40K / G726-M32K / G726M40K / G726M32K / G711A.
    * Tăng âm thanh: 0-14 mức tùy chọn, điều chỉnh âm lượng.
    * Ghi âm trước báo thức: ghi lại một khoảng thời gian trước khi báo thức.
    * Độ trễ cảnh báo: quá trình ghi âm sẽ tiếp tục sau khi loại bỏ cảnh báo và thời gian ghi âm là thời gian đã đặt.
    * Bảo vệ báo động: Trong giao diện danh sách tệp video, chọn tệp video để khóa, nó sẽ không tự động bị ghi đè trong quá trình bảo vệ báo động.
    * Loại máy ảnh: Chọn theo độ phân giải của máy ảnh.

  * **Cài đặt luồng chính: cài đặt các thông số ghi cho từng kênh**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/main-rec.png)

    * Tên kênh: màn hình xem trước và phát lại sẽ được hiển thị.
    * Ghi chính: Bật: nghĩa là kênh có chức năng ghi trên.

      ```
       OFF: có nghĩa là kênh không ghi.
      ```

    * Độ phân giải: 720P, D1, HD1 và CIF có thể được chọn. Ví dụ: trong hệ thống PAL: độ phân giải 720P là 1280 * 720, độ phân giải D1 là 704 * 576, độ phân giải HD1 là 704 * 288, độ phân giải CIF là 352 * 288.
    * Tốc độ khung hình: cho biết số khung hình video mỗi giây, hệ thống PAL là 1 ~ 25 khung hình / giây, hệ thống NTSC là 1 ~ 30 khung hình / giây.
    * Chất lượng hình ảnh, hình ảnh rõ nét, 1 ~ 8 mức, chất lượng hình ảnh mức 1 là cao nhất.
    * Ghi âm: Bật / tắt, cho biết có ghi âm thanh trong khi quay video hay không.

  * **Cài đặt luồng phụ: cài đặt các thông số của luồng video truyền mạng 4G**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/sub-rec.png)

    * Sub video: bật / tắt, có bật chức năng video sub stream hay không.
    * Độ phân giải: CIF / HD1 / D1 tùy chọn.
    * Tốc độ khung hình / chất lượng hình ảnh / ghi: giống như các thông số giao diện cài đặt luồng chính.

  * **Cài đặt thời gian: đặt khoảng thời gian ghi thời gian**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/time-rec.png)

    * Bạn có thể thiết lập tối đa 4 khoảng thời gian ghi mỗi ngày.
    * Ngày: Khoảng thời gian quy định có hiệu lực trong 7 ngày từ Thứ Hai đến Chủ Nhật.
    * Múi giờ: thời gian bắt đầu của múi giờ không được lớn hơn thời gian kết thúc.

  * **Quản lý lưu trữ:**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/disk-manage.png)

    * Mục đích: Tùy chọn video chính / video phụ, chọn luồng video.
    * Ưu tiên: cao / trung bình / thấp.

  * **Cài đặt OSD: thông tin xếp chồng và vị trí hiển thị của video quay**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/osd-set.png)

    * Các mục xếp chồng lên nhau: thời gian / biển số xe / số điện thoại / số kênh / thông tin GPS .
    * Kích hoạt: mở / đóng .
    * Tọa độ X / Y: vị trí hiển thị thông tin chồng chéo trên màn hình .

### Bước 4 : Cấu hình camera trên platform

#### 4.1. Đầu ghi SM400 Basic

*  Bạn vào https://gps.gotrack.vn để đăng nhập.
* Vào mục **Quản lý > Thiết bị**.
* Nếu lắp camera ở thiết bị nào thì chọn **Sửa** ở thiết bị đó. 
* Click vào **<span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-edit.svg)Sửa > Camera > <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Thêm camera**

    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/add-camera-device-1.png)

    - **Tên** : Nhập tên camera  theo đúng kênh cắm ở đầu ghi.
    - **Loại camera** : **Basic** ( thường ). Chỉ chụp ảnh.
    - **Camera Id** : Nhập mã của camera. ID ghi trên thiết bị SM400
    - **Mô tả** : Có thể nhập thêm thông tin về camera,...
    
    Click **Thêm** để lưu camera.

    Sau khi cấu hình xong các thông tin, click **Lưu thay đổi** để hoàn thành thao tác.

#### 4.2. Đầu ghi SM400 Livestream

* Bạn vào https://gps.gotrack.vn để đăng nhập.
* Vào mục **Quản lý > Thiết bị**.
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/livestream/edit-device.png)
* Nếu lắp camera ở thiết bị nào thì chọn **Sửa** ở thiết bị đó. 
* Click vào **<span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-edit.svg)Sửa > Camera > <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Thêm camera**

    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/device/add-camera-device-2.png)

    - **Tên** : Nhập tên vị trí camera bạn muốn lắp đặt.
    - **Loại camera** : **MDVR**. Ngoài chụp ảnh ra còn có thêm tính năng quay video.
    - **MDVR Id** : Nhập mã của camera. ID ghi trên thiết bị SM400
    - **Host** : Địa chỉ IP hoặc tên miền truy cập server camera.
    - **Cổng** : Cổng kết nối đến đầu ghi hình camera. Mặc định là 6605.
    - **Kênh** : Dây nối camera cắm vào cổng của kênh nào thì chọn kênh đó. Vị trí kênh lắp ở đầu ghi. Chỉ được tạo 1 kênh duy nhất. 
    - **Luồng** : Tùy chọn luồng dữ liệu đầu ra. Luồng dữ liệu **chính** với độ nét cao để phục vụ lưu trữ, xem lại. Còn luồng dữ liệu **phụ** dùng để xem qua mạng – với tốc độ đường truyền hạn chế.
    - **Mô tả** : Có thể nhập thêm thông tin về camera,...

    Click **Thêm** để lưu camera.

    Sau khi cấu hình xong các thông tin, click **Lưu thay đổi** để hoàn thành.

### Bước 5 : Cấu hình QCVN

#### 5.1. Cấu hình nhận ảnh

 **Cấu hình nhận ảnh theo lệnh SMS gửi từ thiết bị S200/S400**

- Cổng rs232

    **rs232,0,9,115200#**

- Tần suất chụp: 300 giây

    **rs232para,0,300,0#**

- Server và đường dẫn upload ảnh:

    * server,file,__photos.gotrack365.com,80__# hoặc * server,file,__125.212.235.150,9191__#

    * server,path,__/api/receive-photos__#

    * __reset#__

#### 5.2. Cài đặt máy chủ

* Cài đặt máy chủ trung tâm kết nối

    <span class="icon-left12">![Manage device ](/docs/assets/images/web-interface/livestream/ip-camera.jpg)

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/bb-sv.png)

  * Cài đặt IP  máy chủ giám sát: Báo cáo địa chỉ IP của máy chủ video (IP chính kết nối với trung tâm giám sát).
  * Thiết lập máy chủ tiêu chuẩn của Bộ: Thiết lập thông số nền tảng giao thức tiêu chuẩn của Bộ, được chia thành máy chủ chính và máy chủ dự phòng.


### Bước 6 : Kiểm tra ảnh, video

#### 6.1. Kiểm tra ảnh

* Vào Báo cáo ảnh để xem ảnh

  Bạn vào **Quản lý > Camera > Lịch sử ảnh**.
  Màn hình hiển thị như hình dưới đây :

  <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/livestream/history-image.png)

#### 6.2. Kiểm tra video

* Sau khi cấu hình xong :
  * Bước 1 : Vào mục **Xem trực tiếp** để xem camera video. 
  * Bước 2 : Chọn xe đã cấu hình camera. Nhấn vào **1 kênh nào đó > Xem tất cả**.

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/livestream/livestream.png)

* Muốn xem lại video camera , vào **Quản lý > Camera > Xem lại**. 
  
  Màn hình hiển thị như hình dưới đây :

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/livestream/playback-1.png)

