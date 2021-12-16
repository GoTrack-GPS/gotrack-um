
#  Nhắc nhở

- Nhắc nhở là tạo để thông báo về app/web, tự động nhắc nhở gửi về mail cho các thiết bị khi cần bảo dưỡng hoặc 1 sự kiện nào đó liên quan,...
- Bình thường mọi người hay quên, nên hệ thống sẽ giúp bạn nhắc nhở khi đến mức cảnh báo.
- Đầu tiên, bạn nhấn vào **Quản lý > Cảnh báo - Lập lịch > Nhắc nhở**

    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/remind.jpg) 

### Tìm kiếm 


* Bước 1 : Tìm kiếm theo các tiêu chí sau :
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/search-remind.jpg)    
    
    * **Tên** : Nhập 1 hoặc nhiều ký tự có trong tên nhắc nhở mà bạn muốn tìm kiếm.
    * **Biển số** : Chọn 1 hoặc nhiều  biển số muốn xem nhắc nhở đã gán.

* Bước 2 : Nhấn **Tìm kiếm**.
 
    Nếu nhấn **Đặt lại** sẽ trở về mặc định ban đầu.


### Tạo mới 

- Bước 1 : Nhấn vào **Tạo nhắc nhở**.
- Bước 2 : Xuất hiện màn hình thêm mới
  
  <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/add-remind.jpg)
  
  - **Tên** : Nhập tên thông báo nhắc nhở.
  - **Biển số** : Chọn 1 biển số muốn tạo nhắc nhở
  - **Email** : Nhập email vào ô đó để thêm email. Bạn có thể thêm 1 hoặc nhiều email để gửi thông báo nhắc nhở về.
  - **Mô tả** : Nhập mô tả chi tiết cụ thể thêm về nội dung đó,...
  - **Gửi thông báo** : Tick vào ô  để cài đặt bật / tắt Nhận thông báo về mobile app
  - **Tự động lặp lại** : Lặp lại nhắc nhở theo thời gian = số ngày của thông báo trước.
  - K**ích hoạt** : Bật / tắt chế độ nhắc nhở.
  - **Nhắc nhở theo thời gian** :
    - **Lần bảo trì trước** : Nếu bật thời gian kích hoạt thì bắt buộc nhập. 
    - **Lần bảo trì tiếp theo** : Chọn ngày bảo trì tiếp theo đúng với lịch hẹn của bạn.
    - **Thông báo trước** :  Sẽ lấy trong khoảng của  Ngày bảo trì tiếp theo - Ngày hiện tại. 
  - **Nhắc nhở theo số km** :
    - **Lần bảo trì trước** : Khi chọn biển số sẽ tự động hiện ra quãng đường đã chạy.
    - **Lần bảo trì tiếp theo** : Nhập đúng với lịch hẹn bảo dưỡng số km của bạn.
    - **Thông báo trước** : Sẽ lấy trong khoảng Lần bảo trì tiếp theo - Lần bảo trì trước. 
  - **Nhắc nhở theo giờ nổ máy**  : 
    - Để gửi nhắc nhở này về mail. Cần thực hiện **thêm 1 bước** nữa :
      - Vào **Bản đồ > Thông tin > Tab Mở rộng**. 
      <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/remind-by-hour.jpg)
  
      - Chọn **Tín hiệu động cơ : Khóa điện hoặc Động cơ**. Tùy theo thiết bị lắp dây nào.
      - Nhấn **Lưu thay đổi** để hoàn thành thao tác.
    - **Lần bảo trì trước** : Khi chọn biển số sẽ tự động hiện ra giờ nổ máy đã chạy
    - **Lần bảo trì tiếp theo** : Nhập đúng với lịch hẹn của bạn.
    - **Thông báo trước** : Sẽ lấy trong khoảng Lần bảo trì tiếp theo - Lần bảo trì trước. 
- Bước 3 : Nhấn button **Thêm** để tạo nhắc nhở.


### Sửa

- Để sửa nhắc nhở, thực hiện như sau :

  <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/remind-edit.jpg)

  - Bước 1 : Click vào **Sửa** của nhắc nhở đó.
  - Bước 2 : Sửa các thông tin **nếu có thay đổi** về biển số, mail, loại nhắc nhở,...
  - Bước 3 : Nhấn **Lưu thay đổi** để lưu lại các thông tin vừa sửa.

### Trạng thái kích hoạt
- Để thay đổi trạng thái kích hoạt mà không cần phải vào Sửa nhắc nhở, thực hiện như sau : 

  <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/change-status-active.jpg)
  
  - CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Thay đổi trạng thái**.
  - Trạng thái sẽ thay đổi từ : 
    - **Kích hoạt <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) Không kích hoạt** : Nhắc nhở dừng hoạt động.
    - **Không  kích hoạt <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) Kích hoạt** : Nhắc nhở tiếp tục hoạt động đến số liệu/thời gian đã giới hạn trong nhắc nhở.

### Xóa 

- Bước 1 : CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Xóa** của nhắc nhở đó, sẽ xuất hiện một hộp thoại như hình dưới đây:

    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/remind-delete.jpg)

- Bước 2 : Nếu:
  - Chọn **OK**: Sẽ xóa nhắc nhở đó.
  - Chọn **Hủy**: Sẽ hủy thao tác xóa.

### Xuất báo cáo

* Khi tìm kiếm ra kết quả, click vào **Tải xuống** để xuất dữ liệu
 
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/download-remind.jpg)
  
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
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-interface/notification/download-remind-1.jpg)
    
    - Bật / tắt <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square1.svg) hiển thị bảng / cột theo ý bạn muốn.
    
    - Nếu bỏ tick ẩn đi 1 hoặc nhiểu cột. <br>
    Khi Nhấn **Đặt lại** sẽ chọn lại về mặc định hiển thị tất cả