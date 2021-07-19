# Hướng dẫn cấu hình và kiểm tra cơ bản


Một vài lưu ý:
-	Thiết bị hỗ trợ việc đọc/thiết lập cấu hình qua 3 kênh khác nhau: TCP/IP, COM-Terminal, SMS (cấu trúc, mã lệnh là như nhau).

-	Các thông số quan trọng như IP/Port, ID, central phone sẽ được bảo vệ (sau đây sẽ gọi là thiết bị bị khóa) sau khi thiết bị chạy liên tục được 10 ngày, sau khoảng thời gian này việc thay đổi các thông tin được bảo vệ ở trên sẽ bị hạn chế và chỉ được thực hiện qua các số điện thoại trung tâm hoặc qua kênh cấu hình TCP/IP mà thiết bị đang kết nối tới. (Một nội dung ”No Permission@ER#” sẽ được trả về khi chúng ta thay đổi các thông số đang được bảo vệ từ các kênh đã bị hạn chế).

-	Khách hàng/Đại lý nên cho nhà sản xuất biết thông tin về các số điện thoại sẽ là số trung tâm cho riêng mình, để nhà sản xuất thực hiện việc cấu hình này trước lúc bàn giao tới Khách hàng/Đại lý.

-	***Xin Quý Khách hãy [liên hệ](vi/modules/web-interface/contact/) bộ phận hỗ trợ kỹ thuật để nhận được giải đáp và hướng dẫn tốt nhất***.

- **Chữ cái đầu không phân biệt chữ hoa/chữ thường và chữ cái còn lại viết thường**. . 

###  Bảng tổng hợp chi tiết các loại lệnh

Bạn tham khảo <a href="/mindmaster/gpstracker-param-setting.pdf" target="_blank"> tại đây</a> để xem hoặc tải file. 

### 1. Thiết lập và kiểm tra thông số cơ bản

#### 1.1. Thông số IP/Port


<table>
  <tr>
        <td colspan="3"> * Để cài đặt có hiệu lực,vui lòng gửi lệnh  <b>reset#</b></td>
    </tr> 
    <tr>
        <td rowspan="2"><b>Cấu trúc</b></td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>server,data,< ip/domain>,< port number>#</td>
        <td class="text-bold">server,data#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td><b>Gửi</b></td>
        <td>server,data,125.212.235.145,13030#</td>
        <td class="text-bold">server,data#</td>  
    </tr> 
    <tr>
        <td><b>Nhận</b></td>
        <td>server,data,125.212.235.145,13030#@OK#</td>
        <td>server,data,125.212.235.145,13030@OK#</td>  
    </tr> 
</table>



> Lưu ý: đối với lệnh thiết lập cho thông số này để thực hiện được thành công cần như sau: <br> 
Thiết bị chưa bị khóa cấu hình (để kiểm tra,xem mục [2.10](vi/modules/integrated-devices/smc/s400/sms-command/#unlock) ). <br>
Nếu cấu hình đã bị khóa,số điện thoại thực hiện thiết lập phải là số điện thoại trung tâm. (để kiểm tra/thiết lập,xem mục [1.9](vi/modules/integrated-devices/smc/s400/sms-command/#sensor)). <br>
Thực hiện việc thiết lập qua gửi lệnh từ máy chủ mà thiết bị đang kết nối.

#### 1.2. Thông số APN

<table>
    <tr>
        <td colspan="3"> * Để cài đặt có hiệu lực, vui lòng gửi lệnh  <b>reset#</b></td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>apn,< tên apn cần thiết lập># </td>
        <td class="text-bold">apn#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>apn,apn-name#</td>
        <td class="text-bold">apn#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>apn,apn-name#@OK#</td>
        <td>apn,apn-name@OK#</td>  
    </tr> 
</table>


#### 1.3. Thông số APN-ROAMING


<table>
    <tr>
        <td colspan="3"> * Để cài đặt có hiệu lực, vui lòng gửi lệnh  <b>reset#</b></td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>apnex,< tên apn khi chuyển vùng cần thiết lập># </td>
        <td class="text-bold">apnex#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>apnex,e-connect#</td>
        <td class="text-bold">apnex#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>apnex,e-connect#@OK#</td>
        <td>apnex,e-connect@OK#</td>  
    </tr>
</table>

#### 1.4. Tần suất truyền tin

<table>
     <tr>
        <td colspan="3"> * Mặc định là 30,900 <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh  <b>reset#</b></td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>tim,< thời gian truyền khi chạy>,< khi dừng># </td>
        <td class="text-bold">tim#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>tim#,10,900#</td>
        <td class="text-bold">tim#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>tim,10,900#@OK#</td>
        <td>tim,30,900@OK#</td>  
    </tr> 
    
</table>


#### 1.5. Thông số timezone

<table>
 <tr>
        <td colspan="3"> * Mặc định là +7.0 <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh  <b>reset#</b></td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>tzone,< múi giờ định dạng ±HH.hh># </td>
        <td class="text-bold">tzone#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>Múi giờ: 9:30 -> “HH.hh” = 9 + 30/60 = 9.5 <br>
            tzone,9.5#</td>
        <td class="text-bold">tzone#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>tzone,9.5#@OK#</td>
        <td>tzone,9.5@OK#</td>  
    </tr> 
    
</table>

#### 1.6. Thông số vận tốc giới hạn

<table>
    <tr>
        <td colspan="3"> * Mặc định là 120 <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh  <b>reset# </b>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>speedth,< giá trị tốc độ giới hạn># </td>
        <td class="text-bold">speedth#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td> Gửi</td>
        <td>speedth,120#</td>
        <td class="text-bold">speedth#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>speedth,120#@OK#</td>
        <td>speedth,120#@OK#</td>  
    </tr> 
     
</table>

#### 1.7. Thiết lập còi Buzzer

<table>
    <td colspan="3"> * Mặc định là bật <br>
                         * Được cập nhật sau khi phản hồi OK (đối với việc tắt) và lưu sau khi gửi lại lệnh  <b>reset#</b>
        </td>
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>buzzer,< 0/1: disable/enable>#</td>
        <td  class="text-bold">buzzer#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>buzzer,1#</td>
        <td  class="text-bold">buzzer#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>buzzer,1#@OK#</td>
        <td>buzzer,1#@OK#</td>  
    </tr> 
     <tr>
        
    </tr> 
</table>

#### 1.8. Thiết lập tín hiệu vào số (ALT IO)

<table>
    <tr>
        <td colspan="3"> * Mặc định là AIR với ALT0 và SOS với ALT1 <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh  <b>reset#</b>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>- đối với cổng ALT0 <br> altio,0,< acc/air/sos/doo/ben>,< mức tích cực 0/1># <br>
            - đối với cổng ALT1 <br> altio,1,< acc/air/sos/doo/ben>,< mức tích cực 0/1># </td>
        <td  class="text-bold">altio,0# <br>
            <br>
            altio,1#
        </td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>altio,0,air,1#</td>
        <td  class="text-bold">altio,0#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>altio,0,air,1#@OK#</td>
        <td>altio,0,air,1#@OK#</td>  
    </tr> 
     
</table>

<div id="sensor">
</div>

#### 1.9.	Thiết lập cổng truyền thông RS232 (kết nối cảm biến)

##### 1.9.1. Thiết lập kết nối

<table>
    <tr>
        <td colspan="3"> * Mặc định là tắt <br>
                         * Được cập nhật và lưu sau khi gửi lại lệnh   <b>reset#</b>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>- đối với cổng RS232_0 <br> rs232,0,< sensor id>,< baudrate># <br>
             - đối với cổng RS232_1 <br> rs232,1,< sensor id>,< baudrate># <br>
             -  sensor id:<br> 0/1/2 tắt rs232/cảm biến dầu FLS-Omnicom/ cảm biến dầu Soji
        </td>  
        <td class="text-bold">rs232,0# <br>
            <br>  <br> 
            rs232,1#
        </td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi </td>
        <td>rs232,0,2,9600# (thiết lập cho cảm biến dầu Soji)</td>
        <td class="text-bold">rs232,0#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>rs232,0,2,9600#@OK#</td>
        <td>rs232,0,2,9600#@OK#</td>  
    </tr> 
    
</table>

##### 1.9.2. Thiết lập tham số hoạt động

<table>
    <tr>
        <td colspan="3"> * Mặc định là 10s và 5 đơn vị <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh   <b>reset# </b> <br>
                         * Để xem giá trị cảm biến gửi về xem lệnh view,comm# <br>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
       <td>- đối với cổng RS232_0 <br> 
                rs232para,0,< sample time>,< trigger value># <br> 
            - đối với cổng RS232_1 <br>
                rs232para,1,< sample time>,< trigger value># <br>
            <b> sample time </b> : Thời gian đọc cảm biến,đơn vị s,mặc định 10s<br>
            <b> trigger value </b>: giá trị sai khác giữa 2 lần gần nhất để tạo ra 1 sự kiện cập nhật giá trị cảm biến,mặc định là 5
        </td>  
        <td class="text-bold">rs232para,0# <br>
            <br>  <br> 
                            rs232para,1#
        </td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi </td>
        <td>rs232para,0,20,10# <br> 
             <i>(thiết lập tần suất lấy mẫu/đọc cảm biến: 20s và cập nhật giá trị cảm biến khi sai khác từ 10 đơn vị trở lên) </i>
        </td>
        <td class="text-bold">rs232para,0#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>rs232para,0,20,10#@OK#</td>
        <td>rs232para,0,20,10#@OK#</td>  
    </tr> 
    
</table>

##### 1.10.	Bật/tắt tín hiệu ra số (Out0)

<table>
    <tr>
        <td colspan="3"> * Mặc định đầu ra ở trạng thái không tích cực. <br>
                         * Được cập nhật và lưu tức thì
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td>  
    </tr> 
    <tr>
        <td>outputturn,0,< 0/1: tắt / bật> </td>  
        <td  class="text-bold">output,0#</td>  
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi </td>
        <td>outputturn,0,1#</td>
        <td  class="text-bold">output,0#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>outputturn,0,1#@OK#</td>
        <td>output,0,1#@OK#</td>  
    </tr> 
    
</table>

- Ngoài ra,thiết bị còn hỗ trợ tạo ra một xung vuông có Ton,Toff,số chu kỳ điều chỉnh được hoặc một trigger (xung 1 chu kỳ):

  * **Xung** : outputpulse,0,< ton>,< toff>,< số chu kỳ>#
  * **Trigger**: outputtrigger,0,< ton>#

##### 1.11.	Thiết lập số điện thoại trung tâm 

<table>
     <tr>
        <td colspan="3"> * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh   <b>reset# </b>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>centralphone,< n>,< số điện thoại># <br>
            n: 0,1,2 (hỗ trợ cài đặt 3 số trung tâm)
        </td>  
        <td class="text-bold">centralphone,0# <br>
             Hoặc <br>
             centralphone,1# <br>
             Hoặc <br>
             centralphone,2# <br>
        </td>   
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi</td>
        <td>centralphone,0,0986026929#</td>
        <td class="text-bold">centralphone,0#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>centralphone,0,0986026929#@OK#</td>
        <td>centralphone,0,0986026929#@OK#</td>  
    </tr> 
   
</table>

##### 1.12.	Thiết lập lịch khởi động lại

<table>
    <tr>
        <td colspan="3"> * Mặc định chức năng này bị tắt <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh   <b>reset# </b>
        </td>
    </tr> 
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>rebootsch,< n>,< a># <br>
            thực hiện lịch reboot thiết bị sau “n” ngày vào đúng thời điểm lúc “a” giờ <br>
            n=0: chế độ lập lịch này bị tắt 
        </td>  
        <td class="text-bold">rebootsch#</td>   
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi </td>
        <td>rebootsch,1,0#</td>
        <td class="text-bold">rebootsch#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>rebootsch,1,0#@OK#</td>
        <td>rebootsch,1,0#@OK#</td>  
    </tr> 
    
</table>

##### 1.13.	Thiết lập cảm biến rung lắc

<table>
    <tr>
        <td colspan="3"> * Mặc định là bật và độ nhạy là 0.05 <br>
                         * Được cập nhật sau khi phản hồi OK và lưu sau khi gửi lại lệnh   <b>reset# </b>
        </td>
    </tr>
    <tr>
        <td rowspan="2">Cấu trúc</td>
        <td>Ghi</td>
        <td>Đọc</td> 
    </tr> 
    <tr>
        <td>motion,< 0/1: tắt/bật>,< chỉ số độ nhạy là một giá trị nhỏ hơn 1>#</td>  
        <td class="text-bold">motion#</td>   
    </tr> 
     <tr>
        <td colspan="3">Ví dụ</td>
    </tr> 
     <tr>
        <td>Gửi </td>
        <td>motion,1,0.05#</td>
        <td class="text-bold">motion#</td>  
    </tr> 
    <tr>
        <td>Nhận</td>
        <td>motion,1,0.05#@OK#</td>
        <td>motion,1,0.05#@OK#>  
    </tr> 
     
</table>

>	Lưu ý: giá trị thông số độ nhạy càng nhỏ càng nhạy trong việc phát hiện rung lắc và chuyển động. Khách hàng cẩn trong khi thay đổi thông số này.

##### 1.14.	Thiết lập cân bằng tiêu thụ điện năng (điện áp thấp)
-	Nên sử dụng phần mềm cấu hình để thực hiện việc này.

### 2. Kiểm tra trạng thái hoạt động
#### 2.1. Kiểm tra thông tin thiết bị


<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,vehicleinfo#<b></td>
    </tr> 
    <tr>
        <td>Nội dung phản hồi</td>
        <td>
        <b>vehi</b>,< Biển số xe>,< quãng đường: Km>,< tốc độ>,< ngưỡng xác lập chuyển động>,< số lần quá tốc>,< thời gian duy trì trạng thái hiện tại>,< tổng thời gian dừng>,< lọc vận tốc: 0/A or E không dùng/lọc theo tín hiệu ACC hoặc Engine>. <br>
        <b>driv</b>,< ID thẻ>,< tên lái xe>,< GPLX>,< bắt đầu hành trình>,< kết thúc hành trình>,< tg lái xe liên tục>,< tổng thời gian lái xe> <br>
        <b>devi</b>,< tên thiết bị>,< imei>,< hw-rev>,< Manuf-time>,< install-time> .<br>
        <b>pwr</b>,< điện áp nguồn ngoài>,< điện áp nguồn dự phòng>
        </td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td>view,vehicleinfo,<br>
          <b>vehi</b>,xxX-abc.de,0,0/10,0,9585,161,0 <br>
          <b>driv</b>,1dd46392500104e0 <br>
           ,LX_1dd46,gplx_1dd46,000000,000000,0,0 <br>
          <b>devi</b>,,S200,868183033819694,S2xx v1.0a,201020,201020 <br>
          <b>pwr</b>,19.39,0.00 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.2. Kiểm tra tổng quan

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,overview#</b></td>
    </tr> 
    <tr>
        <td>Nội dung phản hồi</td>
        <td>
        <b>< device name></b>,< imei>,< phiên bản fw>,< 0/1: thiết bị chưa khóa/đã khóa>,< số ngày thiết bị đã hoạt động>,< thời điểm khởi độngDDMMYYhhmmss>,< Nhiệt độ chip xử lý><br>
        <b>nw</b>,< 0/1: chưa có/đã có GPRS>,< độ mạnh sóng,lớn nhất: 31> <br>
        <b>gps</b>,< 0/4/6: trạng thái OK/ERROR/đang ngủ>,< 0/1: không/có chốt vị trí>,< số vệ tinh><br>
        <b>sv</b>,< server ip>,< server port>,< 0/1: chưa/đã kết nối><br>
        <b>pw</b>,< chế độ: 0:normal/1:sleeping>,< điện áp nguồn ngoài>,< điện áp nguồn dự phòng>,< chế độ sạc>,< trạng thái sạc><br>
        <b>ti</b>,< ddmmyy>-< hh:mm:ss>
        </td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td>view,overview,<br>
          <b>S200</b>,868183033877510,1.000.01.000000.201201,0,240,021220094301,34.3C <br>
            <b>nw</b>,1,20 <br>
            <b>gps</b>,0,1,6 <br>
            <b>sv</b>,125.212.235.145,13030,1 <br>
            <b>pw</b>,0,12.17,0.00,2,0 <br>
            <b>ti</b>,7.00,041220-11:13:08 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.3. Kiểm tra trạng thái ngoại vi

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,comm#</b></td>
    </tr> 
    <tr>
        <td>Nội dung phản hồi</td>
        <td>
        <b>led</b>,< state>,< trạng thái 4 led chỉ thị,tính từ trái qua phải: “Lái xe” – “Bộ nhớ” – “Mạng di động” – “GPS”> <br>
        <b>gps</b>,< state>,< 0-Không tốt,1-Tốt>, <số vệ tinh> <br>
        <b>cell</b>,< state>,1,1,1,1,1,< độ mạnh sóng>,< trạng thái kết nối sv/trạng thái đăng nhập server: 0-không tốt,1-Tốt> <br>
        <b>buz</b>,< state>,< 0/1: không bip/đang phát kêu bip> <br>
        <b>rfid</b>,< state>,< ID thẻ> <br>
        <b>Acce</b>,< state>,< trục x>,< trục y>,< trục z>,< trục xyz> <br> 
        <b>rs0</b>,< state>,< sensor id>,< state>,< giá trị số đọc từ cảm biến> <br>
        <b>rs1</b>,< state>,< sensor id>,< state>,<giá trị số đọc từ cảm biến> <br>
        <b>acc</b>,< state>,< mức tích cực> <br>
        <b>eng </b>,< state>,< mức tích cực> <br>
        <b>AIR</b>,< state>,1,+,< mức tích cực> <br>
        <b>SOS</b>,< state>,3,+,< mức tích cực> <br>
        <b>DO</b>, < state>,< mức tích cực>  <br>
        <i>state </i>: <br>
        &emsp;&emsp;&emsp;&emsp;-	7: bị tắt/Không sử dụng <br>
        &emsp;&emsp;&emsp;&emsp;-	6: bị reset <br>
        &emsp;&emsp;&emsp;&emsp;-	5: dừng tạm thời <br>
        &emsp;&emsp;&emsp;&emsp;-	4: không kết nối được với bộ xử lý <br>
        &emsp;&emsp;&emsp;&emsp;-	3: lỗi gói tin <br>
        &emsp;&emsp;&emsp;&emsp;-	2: lỗi checksum <br>
        &emsp;&emsp;&emsp;&emsp;-	1: đang ngủ <br>
        &emsp;&emsp;&emsp;&emsp;-	0: Tốt <br>
        <i>Mức tích cực </i>: 0-Tắt/Đóng,1-Bật/Mở <br>
        <i>Trạng thái led </i> : 0-Tắt,1-Sáng không chớp,2-Lóe sáng nhanh (Chớp nhanh),3-Lóe sáng lâu (chớp chậm).
        </td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td>view,comm,<br>
          <b>led</b>,,0,0133<br>
            <b>gps</b>,0,1,5 <br>
            <b>cell</b>,0,1,1,1,1,1,20,1/1 <br>
            <b>buz</b>,0,0 <br>
            <b>rfid</b>,0,3030303030303030 <br>
            <b>Acce</b>,0,0.00,-0.02,1.00,1.00 <br>
            <b>rs0</b>,0,2,4,0 <br>
            <b>acc</b>,0,0 <br>
            <b>eng</b>,0,0 <br>
            <b>AIR</b>,0,1,+,0 <br>
            <b>SOS</b>,0,3,+,0 <br>
            <b>DO</b>,0,0 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.4.	Kiểm tra thông tin kết nối mạng di động


<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,network#</b></td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td>view,network,<br>
            <b>reg</b>,1,1,1,1,1 <br>
            <b> cid</b>,89840480000616669331 <br>
            <b>nw</b>,0,0,"Mobifone",20 <br>
            <b>cb</b>,EGSM_MODE,ALL_BAND,20 <br>
            <b>apn</b>,m-wap,e-connect <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.5. Kiểm tra trạng thái kết nối máy chủ 

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,serverconn#</b></td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td> 
            view,serverconn,10.82.117.62[0] <br>
            0.asia.pool.ntp.org:123,0,105311,LOST <br>
            27.72.57.208:5555,1,104609,LOST <br>
            125.212.235.145:13030,*,102409,OK <br>
            ota.gotrack.vn:8086,0,,LOST <br>
            ota.gotrack.vn:1111,0,,LOST <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.6. Kiểm tra lưu lượng tiêu thụ

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view, idatameter# </b><br>
        (Lưu lượng được tính từ 00h)
        </td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td> 
            view, idatameter,<br>
            <b>Send/Rev </b>: 30.98/0.64KB <br>
            0:112412,112418,48B,0P,112417,48B,7P <br>
            1:112240,112245,12B,0P,112246,37B,18P <br>
            2:102409,102414,38B,0P,112749,50B,697P <br>
            3:,,0B,0P,,0B,0P <br>
            4:,,0B,0P,,0B,0P <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.7. Kiểm tra thông tin bộ nhớ và lưu trữ 

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view, diskinfo# </b></td>
    </tr> 
    <tr>
        <td>Nội dung phản hồi</td>
        <td>view, diskinfo,<br>
        <b>disk</b>,< 0: tốt>,< dung lượng KB còn trống/tổng> <br>
        <b>dat</b>,< tên file dữ liệu>,< dung lượng KB>,< 1: đã bật chế độ log> <br>
        <b>bak</b>,< thông tin truyền log: số byte đã truyền/tổn số>,< dung lượng Byte của file > <br>
        <b>> TCP-Stream</b>
         < Số bản tin của FIFO>,< dung lượng BYTE và địa chỉ của FIFO> <br>
        Q_NO_PROTEC <br>
        < số bản tin đã truyền/tổng số bản tin trong FIFO>:<số BYTE còn lại của FIFO>
        @OK#
    </td>
    </tr> 
      <tr>
        <td>Ví dụ</td>
        <td>view, diskinfo, <br>
        <b>disk </b>,0,2800.0/7640.0 <br>
            <b>dat </b>,201204.TXT,95065,0x1 <br>
            <b>bak</b>,0/0,0 <br>
            <b>>TCP-Stream</b> <br> 
            120Msg,4096B@0x200032f8 <br>
            Q_NO_PROTEC <br>
            0/0:4096 <br>
            @OK#
    </td>
    <tr>
        <td colspan="2"> 
            * Log (hay còn gọi là dữ liệu lịch sử) bị đọng sẽ thể hiện ở bak và < số bản tin đã truyền/tổng số bản tin trong FIFO>. Thực hiện kiểm tra khi không thấy thiết bị cập nhật dữ liệu mới <br>
            *  Xóa log để cập nhật ngay dữ liệu mới xử dụng lệnh <b> fsmclean,log# </b>
        </td>
    </tr> 
</table>

#### 2.8. Kiểm tra trạng thái nguồn điện của xe 

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view, powerinfo#</b></td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td> 
            view, powerinfo, <br>
            <b>Main </b>,12.18,1(12.40-36.00) <br>
             <b>Bak </b>,0.00,0%,1(3.20-4.20) <br>
             <b>SW </b>,0/1,505000/10,180000/3 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.9. Lấy vị trí của xe hiện tại

<table>
    <tr>
        <td>Lệnh</td>
        <td><b>view,map#</b></td>
    </tr> 
    <tr>
        <td>Ví dụ</td>
        <td> 
            view,map,http://maps.google.com/maps?q=N%2020%2059.618626%20E%20105%2047.236412 <br>
            @OK#     
        </td>
    </tr> 
</table>

<div id="unlock">
</div>

#### 2.10.	Trạng thái bảo vệ cấu hình

<table>
    <tr>
        <td>Lệnh</td>
        <td colspan="2"><b>lockerstat#</b></td>
    </tr> 
    <tr>
        <td rowspan="2">Ví dụ</td>
        <td>lockerstat, 0@OK# </td>
        <td>Cấu hình chưa được bảo vệ</td>
    </tr> 
    <tr>
        <td>lockerstat, 1@OK#</td>
        <td>Cấu hình đã được bảo vệ (thiết bị đã bị khóa)</td>
    </tr> 
</table>

### 3. Các lệnh xử lý khác

#### 3.1. Xóa log

* Fsmclean,log#

#### 3.2. Khởi động lại thiết bị

* reset#

#### 3.3. Truyền bản tin tức thì

* Pack,< packet-name: location/status/sensor/heartbeat>#
* VD: Pack,location#

#### 3.4. Lấy số điện thoại trên thiết bị

* Cellularsms,< sdt nhận sms từ thiết bị>,< nội dung sms mà thiết bị sẽ gửi>#
Cellularsms,0986026929,xin chao#
