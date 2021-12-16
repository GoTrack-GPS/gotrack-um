# Corridor
- **Corridor** là tạo đường cảnh báo vượt quá tốc độ giới hạn khi đi vào/ra đường theo lộ trình đã tạo.
- Số lần vượt quá tốc độ giới hạn tính từ 2 gói tin trở lên. Và từ thời gian  bắt đầu vượt quá tốc độ cảnh báo đến thời gian mà có tốc độ dưới mức cảnh báo.
- Để vào corridor, thực hiện như sau :
  - Vào **Quản lý > Cấu hình > Corridor**.

    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/corridor-in.jpg)

### Thêm
- Để tạo mới corridor, thực hiện như sau :

    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-add.jpg)

  - Bước 1 : Nhấn vào **Thêm corridor**.
  - Bước 2 : Xuất  hiện hộp thoại như trong ảnh :
    - **Tên** : Tên corridor ngắn gọn, dễ hiểu với đường bạn muốn vẽ.
    - **Bán kính** : Bán kính đường corridor.
    - **Tốc độ giới hạn (km/h)** : Tốc độ cho phéo tối đa mà xe có thể chạy khi đi qua đoạn đường đó.
    - **Số điểm đánh dấu** : Sự tự động hiển thị khi bạn vẽ đường cảnh báo trên Bản đồ.
    - **Màu viền/màu nền** : Có thể chọn màu khác tùy theo sở thích của bạn. 
    - **Độ mờ viền/độ mờ nền** : Có thể sửa tăng giảm tùy theo góc nhìn của bạn.
    - **Mô tả** : Nhập địa chỉ cụ thể của đoạn đường đó. Hoặc là mô tả chi tiết  thông tin từ lối vào- lối ra của đoạn đường đó đi qua nơi nào,...
    - **Trạng thái** : Bật/tắt kích hoạt corridor đang tạo.
  - Bước 3 : Click vào **đoạn icon trên Bản đồ** để thêm, sửa, xóa điểm tạo thành đường đi. Phóng to/thu nhỏ, di chuyển đến đường cần vẽ cảnh báo vượt quá tốc độ.
    - **Chấm các điểm theo lộ trình** đường đi muốn tạo cảnh báo.
    - **Click vào điểm cuối** lần nữa khi muốn dừng vẽ 1 đoạn đường.
    - Click giữ chuột trái vào chấm tròn trắng  để kéo, di chuyển đến đúng đường đi. 
    - Click vào điểm xám nhạt sẽ tự động sinh ra 1 điểm nữa.
    - Với đường đi thẳng, chỉ cần chấm ở 2 đầu đoạn đường đó.
    - Vẽ dùng càng ít điểm mà vẫn đúng lộ trình càng tốt.
- Bước 4 : Nhấn button **Thêm** để tạo corridor.

### Sửa 
- Để sửa corridor, thực hiện theo các bước sau :

    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-edit.jpg)

  - Bước 1 : Click vào **Sửa** corridor đó.
  - Bước 2 : Sửa các thông tin (nếu có) như tốc độ, đường đi,...
  - Bước 3 : Nhấn button **Lưu thay đổi** để lưu lại thông tin vừa sửa.

### Trạng thái kích hoạt

- Để thay đổi trạng thái kích hoạt mà không cần phải vào Sửa corridor, thực hiện như sau : 

  <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-chage-status.jpg)
  
  - CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Thay đổi trạng thái**.
  - Trạng thái sẽ thay đổi từ : 
    - **Kích hoạt <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) Không kích hoạt** :Corridor dừng hoạt động.
    - **Không  kích hoạt <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) Kích hoạt** : Corridor tiếp tục hoạt động.

### Xóa 

- Bước 1 : CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Xóa** của corridor đó, sẽ xuất hiện một hộp thoại như hình dưới đây:

    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-delete.jpg)

- Bước 2 : Nếu:
  - Chọn **OK**: Sẽ xóa corridor đó.
  - Chọn **Hủy**: Sẽ hủy corridor xóa.


### Xuất báo cáo

* Khi tìm kiếm ra kết quả, click vào **Tải xuống** để xuất dữ liệu
 
    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-dowload.jpg)
  
  - <span class="icon-left svg-filter-circlegreen2">![Ok](/docs/assets/images/web-interface/icon/SVG/file-excel1.svg) **XLSX** : Tải xuống dạng Excel của trang hiện tại.

  - <span class="icon-left svg-filter-circlered">![Ok](/docs/assets/images/web-interface/icon/SVG/file-pdf1.svg) **PDF** : Tải xuống dạng PDF của trang hiện tại.

  - <span class="icon-left svg-filter-circlegreen2">![Ok](/docs/assets/images/web-interface/icon/SVG/file-excel1.svg) **Tải xuống tất cả XLSX** : Tải xuống dạng Excel tất cả các trang.
  
  - <span class="icon-left svg-filter-circlered">![Ok](/docs/assets/images/web-interface/icon/SVG/file-pdf1.svg) **Tải xuống tất cả PDF** : Tải xuống tất cả  PDF tất cả các trang.

- Click vào <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-reset.svg) để làm mới danh sách.
      
- Click vào <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/column-height.svg) để chỉnh sửa chiều cao của hàng theo mức **Nhỏ** <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) **Lớn** 

  - **Nhỏ** : Chiều cao của từng hàng sẽ nhỏ lại.
  - **Trung bình** : Chiều cao của hàng sẽ rộng ra cách chữ 1 chút.
  - **Lớn** : Chiều cao của hàng sẽ rộng hơn loại Trung bình thêm 1 chút.
- Dạng bảng :  Click vào <span class="icon-left ">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-gear.svg) để hiển thị dữ liệu dạng bảng.
    
    <span style="display:block;text-align:left">![Interface Web](/docs/assets/images/web-interface/map/manage-corridor-dowload-2.jpg)
    
    - Bật / tắt <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square1.svg) hiển thị bảng / cột theo ý bạn muốn.
    
    - Nếu bỏ tick ẩn đi 1 hoặc nhiểu cột. <br>
    Khi Nhấn **Đặt lại** sẽ chọn lại về mặc định hiển thị tất cả.
    
- Ngoài ra, bạn có thể tạo mới và quản lý corridor [tại đây](vi/modules/web-interface/tracking/map-corridor/#map-corridor)
