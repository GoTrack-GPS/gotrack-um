# Danh sách camera
- Để xem danh sách camera mà đã tạo cho các thiết bị trong tài khoản đó, thực hiện như sau :
  - Vào **Camera > Danh sách camera**. Màn hình hiển thị như sau :
    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/list-camera.png)

### Tìm kiếm 
- Để tìm kiếm camera đã tạo, thực hiện như sau :
  <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/search-camera.png)
  - Bước 1 : Tìm kiếm theo 1 trong các tiêu chí sau :
    - **Tên** : Nhập 1 hoặc nhiều ký tự trong tên để tìm kiếm.
    - **Biển số** : Chọn 1 trong những biển số trong droplist.
    - **Loại camera** : Chọn 1 trong 2 loại camera đã từng chọn.
  - Bước 2 : Nhấn **Tìm kiếm** để hiển thị tất cả những tiêu chí muốn xem.
  - Nhấn **Đặt lại** để xóa dữ liệu, đưa về chế độ mặc định ban đầu.

### Thêm camera
- Để thêm camera, trước tiên phải có điểm để thêm camera, mỗi kênh camera là 1 điểm.
- Hãy liên hệ nhà phân phối để thêm điểm camera.
- Sau khi có điểm, thực hiện thêm camera như sau :

#### Đầu ghi SM400 Basic

  - Bước 1 :  Click vào **<span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Tạo camera**.
- Bước 2 : Sẽ xuất hiện hộp thoại như dưới đây. Nhập/chọn thông tin vào trong ô.

    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/add-camera.png)
- Biển số : Chọn 1 trong những biển số trong droplist để thêm camera
    - **Tên** : Nhập tên vị trí camera bạn muốn lắp đặt.
    - **Loại camera** : **Basic** ( thường ). Chỉ chụp ảnh.
    - **Camera Id** :  Dây nối camera cắm vào cổng của kênh nào thì chọn kênh đó. 
      - Vị trí kênh lắp ở đầu ghi, **AV1  <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  AV4**. (Đối với đầu ghi 8 kênh thì <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  **AV8** ). 
      - Tương ứng từ **CH1 <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) CH8**
      -  Chỉ được tạo 1 kênh duy nhất. 
  - **Vị trí** : Đối với các xe truyền dữ liệu lên Bộ Giao thông vận tải bắt buộc phải lắp camera tại 3 vị trí sau :
      - **Lái xe** : Vị trí nhìn thấy người lái xe, tài xế.
      - **Cửa** :  Vị trí  hành khách đi lên -  xuống xe.
      - **Hành khách** : Vị trí bao quát hết các hành khách đang trên xe.

  - **Mô tả** : Có thể nhập thêm thông tin về camera, vị trí lắp đặt,...
  - **Nhân bản** : Nếu muốn tạo nhiều kênh cùng 1 lúc thì chọn nhân bản, sao chép bằng đó kênh. Khi nhân bản thành công chỉ cần chọn lại số kênh. Chỉ áp dụng khi thiết bị đó chưa tạo camera nào.    
- Bước 3 :  Click **Thêm** để lưu camera.

#### Đầu ghi SM400 Livestream (MDVR)

 - Bước 1: Click vào **<span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Tạo camera**
- Bước 2 : Sẽ xuất hiện hộp thoại như dưới đây. Nhập/chọn thông tin vào trong ô.
    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/add-camera-mdvr.png)
  - **Biển số** : Chọn 1 trong những biển số trong droplist để thêm camera
  - **Tên** : Nhập tên vị trí camera bạn muốn lắp đặt.
  - **Loại camera** : **MDVR**. Ngoài chụp ảnh ra còn có thêm tính năng quay video.
  - **MDVR Id** : Nhập mã của camera. ID ghi trên thiết bị SM400.
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
    - **Mô tả** : Có thể nhập thêm thông tin về camera, vị trí lắp đặt,...
  - **Nhân bản** : Nếu muốn tạo nhiều kênh cùng 1 lúc thì chọn nhân bản, sao chép bằng đó kênh. Chỉ áp dụng khi thiết bị đó chưa tạo camera nào.

- Bước 3 : Click **Thêm** để lưu camera.


### Sửa camera 
 - Bước 1: Click vào **<span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-edit.svg) Sửa** kênh camera đó.
- Bước 2 : Sẽ xuất hiện hộp thoại như dưới đây. Sửa thông tin nếu có thay đổi.
    <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/edit-camera.png)
- Bước 3 : Click **Lưu thay đổi** để lưu thông tin vừa sửa.

### Xóa
- CLick  vào icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) **> Xóa** của kênh camera đó, sẽ xuất hiện một hộp thoại như hình dưới đây:

  <span style="display:block;text-align:left">![delete device](/docs/assets/images/web-interface/livestream/list-camera-delete.png)

  Nếu:
  - Chọn **Xác nhận**: Sẽ xóa thiết bị đó.
  - Chọn **Hủy**: Sẽ hủy thao tác xóa.

### Xuất báo cáo

* Khi tìm kiếm ra kết quả, click vào 

    - <span class="icon-left svg-filter-circlegreen2">![Ok](/docs/assets/images/web-interface/icon/SVG/file-excel1.svg) **XLSX** : Tải xuống dạng Excel của trang hiện tại.

    - <span class="icon-left svg-filter-circlered">![Ok](/docs/assets/images/web-interface/icon/SVG/file-pdf1.svg) **PDF** : Tải xuống dạng PDF của trang hiện tại
   
    - <span class="icon-left svg-filter-circlegreen2">![Ok](/docs/assets/images/web-interface/icon/SVG/file-excel1.svg) **Tải xuống tất cả XLSX** : Tải xuống dạng Excel tất cả các trang.
    - <span class="icon-left svg-filter-circlered">![Ok](/docs/assets/images/web-interface/icon/SVG/file-pdf1.svg) **Tải xuống tất cả PDF** : Tải xuống tất cả  PDF tất cả các trang.

    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/livestream/list-camera-export.png)


### Các tiện ích trên góc phải 

- Click vào icon  <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-reset.svg) để làm mới dữ liệu.

- Click vào <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/column-height.svg) để chỉnh sửa chiều cao của hàng theo mức **Nhỏ** <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) **Lớn** 

  - **Nhỏ** : Chiều cao của từng hàng sẽ nhỏ lại.
  - **Trung bình** : Chiều cao của hàng sẽ rộng ra cách chữ 1 chút.
  - **Lớn** : Chiều cao của hàng sẽ rộng hơn loại Trung bình thêm 1 chút.

<span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/livestream/list-camera-export-1.png)

- Dạng bảng :  Click vào <span class="icon-left ">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-gear.svg) để hiển thị dữ liệu dạng bảng.

    - Bật / tắt <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square1.svg) hiển thị bảng / cột theo ý bạn muốn.
    
    - Nếu bỏ tick ẩn đi 1 hoặc nhiểu cột. <br>
    - Khi Nhấn **Đặt lại** sẽ chọn lại về mặc định hiển thị tất cả/