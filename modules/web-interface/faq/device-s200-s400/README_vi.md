# Thiết bị S200/S400

### Câu 1

* Q : Chúng tôi muốn kết nối thiết bị tới máy chủ của chúng thôi có IP/port là: 115.14123.160/16868 và tần suất truyền dữ liệu là 10s khi xe chạy thì thực hiện như thế nào?

* A : Chúng ta có thể thực hiện việc thay đổi các thông số này qua SMS, như sau:
    - [Tham khảo 1.1](vi/modules/integrated-devices/smc/s200/sms-command/#ip)  và soạn lệnh: server,data,125.212.235.144,13030# gửi tới số điện thoại trong thiết bị
    - [Tham khảo 1.3](vi/modules/integrated-devices/smc/s200/sms-command/#apn-roaming)  soạn lệnh tim,10,900# gửi tới số điện thoại của thiết bị
    -	Để thiết bị lưu và cập nhật cấu hình mới, soạn lệnh reset# gửi tới số điện thoại trong thiết bị. Sau đó thiết bị sẽ cần thời gian để khởi động lại.

### Câu 2

* Q : Xe của chúng tôi có chạy qua ranh giới 2 quốc gia, sim điện thoại của chúng tôi đã đăng ký chuyển vùng quốc tế, nhưng khi qua biên giới nước bạn thì không còn gửi dữ liệu về nữa. Vậy chúng tôi phải xử lý, khắc phục như thế nào

* A : Đối với trường hợp này, rất có thể Quý Khách chưa thực hiện việc cấu hình bổ sung thông tin APN, Quý khách cần liên lạc với tổng đài hoặc nhà cung cấp dịch vụ viễn thông đang sử dụng để hỏi về APN mỗi khi SIM thực hiện ROAMING bên nước bạn. Sau khi có thông tin này, chúng ta thực hiện theo lệnh ở mục [1.13](vi/modules/integrated-devices/smc/s200/sms-command/#ring).

### Câu 3

* Q : Tôi muốn tắt tiếng kêu của còi, bởi vì Khách hàng thuê xe thấy phiền khi nghe thấy nó

* A : Chúng ta có thể tham khảo lệnh [1.7](vi/modules/integrated-devices/smc/s200/sms-command/#bip), Quý Khách soạn một SMS như sau: buzzer,0# sau đó gửi tới số điện thoại trong thiết bị.

### Câu 4

* Q : Tại sao tôi khi tôi thay đổi cấu hình chỉ chạy được một thời gian lại thấy quay lại cấu hình cũ?

* A : Để đảm bảo cấu hình được lưu trữ và cập nhật, Quý Khách sau khi thực hiện xong việc cấu hình thay đổi các thông tin mong muốn thì nên thực hiện gửi thêm lệnh khởi động lại: reset#

### Câu 5

* Q : Tôi thấy trên phần mềm giám sát, xe của tôi thể hiện trạng thái đang truyền log. Làm thế nào để xe của tôi cập nhật vị trí ngay lập tức.

* A : Thiết bị của Quý Khách vì lý do nào đó mà trước đấy đã mất kết nối với máy chủ một thời gian dài, làm cho dữ liệu hành trình tích lũy trong bộ nhớ và hiện tại đang thực hiện truyền lại dữ liệu này. Nếu dữ liệu đó không quan trọng và có thể xóa được thì chúng ta có thể thực hiện lệnh xóa như sau: fsmclean,log# gửi tới số điện thoại trong thiết bị. (xem thêm [2.7](vi/modules/integrated-devices/smc/s200/sms-command/#log))

### Câu 6

* Q : Tôi thường xuyên đi làm trên đường cao vành đai trên cao, khi xe vừa lên 80Km/h thì thiết bị kêu còi làm sao để khắc phục cho trường hợp này?

* A : Đối với trường hợp của quý Khách, rất có thể thiết bị đang cảnh báo quá tốc độ cho phép, nếu là xe cá nhân Quý Khách có thể thay đổi vận tốc giới hạn cho cảnh báo, ví dụ cung đường đó cho phép tới 90Km/h, quý Khách có thể cấu hình lại bằng cách soạn tin SMS: speedth,90# gửi tới số điện thoại trong thiết bị.

### Câu 7

* Q : Khi lắp xong cảm biến dầu trên cổng rs232_0 ở cổng A tôi muốn kiểm tra trạng thái hoặc giá trị mức dầu tại hiện trường trong trường hợp tôi không thể xem qua máy tính?

* A : Với trường hợp này quý Khách có thể thực hiện như sau, soạn SMS: view,comm# gửi tới số điện thoại của thiết bị. Thiết bị sẽ phản hồi 1 SMS có nội dung minh họa như sau: 
 
    Trong trường hợp không lên mức dầu (từ 1÷4095), Quý khách nên kiểm tra lại:
    -	Cấu hình cổng, loại cảm biến. Tham khảo 1.19
    -	Kiểm tra lại TX, RX của thiết bị và cảm biến có được nối chéo nhau hay không.
