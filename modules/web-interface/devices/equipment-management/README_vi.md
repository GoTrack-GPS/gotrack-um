# Các chức năng khác  
Để thực hiện các chức năng khác của thiết bị, người dùng vào **Quản lý > Thiết bị** 

 <span class="icon-left4">![Manage device ](/docs/assets/images/web-interface/device/manage-device-1.png)
 
### 1. Chuyển/Bán thiết bị
Để chuyển/gán thiết bị sang cho tài khoản khác, có 2 cách
* **Cách 1** 

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/move-device.png)

    - Bước 1: Tick vào thiết bị cần chuyển/bán.
    - Bước 2: Chọn **Chuyển/Bán**.
    - Bước 3: Một hộp thoại xuất hiện. Chọn **tài khoản** để chuyển/bán thiết bị sang đó. **IMEI** là mã số của thiết bị đó.
    - Bước 4: Click vào **Gửi** để chuyển/bán thiết bị.
* **Cách 2** 

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/move-device-2.png)

- Bước 1 : CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Bán** của thiết bị đó.
- Bước 2 : Sau khi  click vào "Bán" xong. Sẽ cập nhật trạng thái hiện tại <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) **Đã bán**. 
  - Thông báo "Thiết bị đã được bán".
* **Cách 3**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/equipment-sale.png)
    

    - Bước 1 : Click vào **Thêm**
    - Bước 2 : Chọn **Bán thiết bị vào tại tài khoản**.
    - Bước 3: Nhập các thông tin trong hộp thoại
        - **Tài khoản** : Chọn tài khoản để bán thiết bị.
        - **Tiền tố tài khoản** : Tương ứng với tài khoản vừa chọn.
        - **Vai trò** : Chọn vai trò tài khoản.
        - **IMEI** : Mã số của thiết bị đó.

    - Bước 4 : Click vào **Gửi** để bán thiết bị.

### 2. Kích hoạt / Vô hiệu hóa thiết bị
- **Kích hoạt tự động**: Thiết bị được tự động kích hoạt sau 8h kể từ khi tạo và lắp xong thiết bị.
- **Kích hoạt thủ công**:
     
    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-interface/device/active-device.png)

    - Bước 1: Chọn thiết bị mà bạn muốn kích hoạt / vô hiệu hóa.
    - Bước 2. Chọn **:point_right: Kích hoạt** / **vô hiệu hóa**. **IMEI** là mã số của thiết bị đó.
    - Bước 3: Một hộp thoại xuất hiện. 
        Cài đặt trạng thái là **kích hoạt** / **vô hiệu hóa**. 
        **IMEI** là mã số của thiết bị đó.

    - Bước 4 : Click vào **Gửi** để kích hoạt / vô hiệu hóa thiết bị.

### 3. Cài đặt trạng thái thiết bị

Để cài đặt trạng thái cho thiết bị, thực hiện các bước sau: 

<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/device-status.png)


- Bước 1: Tick vào thiết bị cần cài đặt trạng thái.
- Bước 2: Chọn **Trạng thái**.
- Bước 3: Một hộp thoại xuất hiện. Chọn trạng thái hiện tại đúng của thiết bị. **IMEI** là mã số của thiết bị đó.
- Bước 4: Click vào **Gửi** để cài đặt trạng thái cho thiết bị.

### 4. Gửi lệnh thiết bị

Để gửi lệnh thiết bị, thực hiện các bước sau: 

<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/send-the-device-command.png)


- Bước 1: Tick vào thiết bị cần gửi lệnh.
- Bước 2: Chọn **Gửi lệnh**.
- Bước 3: Một hộp thoại xuất hiện. **Tên thiết bị, Loại thiết bị** đã tạo. Chọn **loại lệnh** cần yêu cầu thực hiện.
- Bước 4: Click vào **Gửi** để gửi lệnh thiết bị.

Để tìm hiểu thêm chi tiết, bạn tham khảo [tại đây](vi/modules/web-interface/devices/send-the-device-command/#command)  <div id="command"> 

### 5. CCID
- Kiểm tra SIM đang lắp trên thiết bị có phải SIM hợp lệ hay không.
- CCID Origin là SIM được gắn kèm khi xuất kho và có thể cập nhật khi có yêu cầu thay đổi.
- CCID là SIM hiện tại đang được gắn với thiết bị.
- SIM hợp lệ là SIM có CCID bằng CCID Origin.
- SIM không hợp lệ là trường có CCID không bằng CCID Origin + phải bật kiểm tra CCID + CCID phải do GoTrack cũng cấp và tồn tại trong hệ thông quán lý SIM.

#### 5.1. Đồng bộ CCID
- **Cách 1**
  - Là **cập nhật CCID Origin = CCID**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/ccid-sync.png)

  - Bước 1 : Tick chọn **IMEI** cần đồng bộ CCID.
  - Bước 2 : Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Đồng bộ CCID**.
  - Bước 3 : **Kiểm tra IMEI**.
  - Bước 4 : Nhấn **Gửi** để đồng bộ CCID.
- **Cách 2**
    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/syn-ccid.png)
  - CLick  vào icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Đồng bộ CCID** của thiết bị đó.

#### 5.2. Cập nhật kiểm tra CCID
- Là **cho phép bật / tắt kiểm tra SIM**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/update-ccid-check.png)
  - Bước 1 : Tick chọn **IMEI** cần cập nhật kiểm tra CCID.
  - Bước 2 : Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Cập nhật kiểm tra CCID**.
  - Bước 3 : 
    - **Trạng thái** : Kích hoạt/Không kích hoạt để bật/tắt SIM.
    - **IMEI** Thiết bị cần kiểm tra.
  - Bước 4 : Nhấn **Gửi** để cập nhật kiểm tra CCID.


#### 5.3. Cập nhật CCID: 
- Cho phép cập nhật CCID thủ công.

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/update-ccid.png)
  - Bước 1 : Tick chọn **IMEI** cần cập nhật CCID.
  - Bước 2 : Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Cập nhật CCID**.
  - Bước 3 : 
    - **IMEI** Thiết bị cần kiểm tra.
    - **CCID** là là mã số in trên thẻ SIM. SIM hiện tại đang được gắn với thiết bị

  - Bước 4 : Nhấn **Gửi** để cập nhật CCID.

### 6. Thêm
#### 6.1. Đặt lại vị trí
- Nếu vị trí của thiết bị chưa có thì có thể cấu hình nhanh ở đây.
  <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/reset-location.png)

  - Bước 1 : **Chọn thiết bị** cần thiết lập vị trí
  - Bước 2 : Vào **Thêm > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Đặt lại vị trí**.
  - Bước 3 : Hộp thoại mở ra. Nhập thông tin vào form :
    - **Vĩ độ** là giá trị xác định vị trí của một điểm nào đó trên bề mặt Trái đất và kể cả các hành tinh khác, ở phía bắc hay phía nam của xích đạo. 
    -  **Kinh độ** là giá trị tọa độ địa lý theo hướng đông sang tây.  
    - Bạn có thể vào Bản đồ của Google để lấy tọa độ chính xác.
  > Lưu ý : Chỉ nhập được tọa độ là số nguyên.
  - Bước 4 : Nhấn **Gửi** để đặt lại vị trí.

#### 6.2. Đổi  IMEI
- Khi xe của khách hàng đổi sang thiết bị mới, muốn đổi lại IMEI trên hệ thống để hiển thị dữ liệu theo IMEI mới thì thực hiện như sau :
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/change-imei.png)
  - Bước 1 : **Chọn thiết bị** cần phải chuyển đổi IMEI.
  - Bước 2 : Click vào **Thêm > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Đổi IMEI**.
  - Bước 3 : Xuất hiện hộp thoại. Điền thông tin vào form.
    - **IMEI mới** : Nhập IMEI mới mà đã có sẵn trong kho.
  - Bước 3 : Nhấn **Lưu thay đổi** để đổi IMEI.

#### 6.3. Đặt lại mặc định
- Khi muốn lưu lại dữ liệu mới từ đầu/gặp vấn đề gì đó cần phải đặt lại mặc định thì thực hiện như sau :
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/device/reset-to-defaults.png)
  - Bước 1 : **Chọn thiết bị** cần đặt lại mặc định
  - Bước 2 : Click vào **Thêm > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Đặt lại mặc định**.
  - Bước 3 : Xuất hiện hộp thoại. Điền thông tin vào form.
    - **IMEI** : Nhập IMEI mà đã có sẵn trong kho/thêm IMEI cần đặt lại mặc định và kiểm tra lại IMEI đó.
  - Bước 3 : Nhấn **Gửi** để đổi IMEI.







