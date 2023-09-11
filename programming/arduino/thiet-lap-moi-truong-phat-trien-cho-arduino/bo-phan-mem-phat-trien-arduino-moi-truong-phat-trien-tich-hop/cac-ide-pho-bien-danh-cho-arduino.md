# Các IDE phổ biến dành cho Arduino

Như phần trước đã đề cập đến Arduino IDE, vốn là phần mềm được phát triển và hỗ trợ chính thức từ Arduino nhưng đây không phải là IDE duy nhất và "tốt nhất".&#x20;

Không có một IDE nào có thể được cho là "tốt nhất" bởi nó hoàn toàn phụ thuộc vào nhu cầu sử dụng của mỗi người. Trong phần này ta sẽ xem xét thêm một IDE phổ biến dành cho người dùng có kinh nghiệm từ trước đó là PlatformIO - một IDE mà bản thân mình - người viết đã sử dụng ngay từ ngày đầu sử dụng Arduino.&#x20;

Về chung, cả 2 IDE đều phổ biến dành cho hệ thống nhúng và chúng đều có điểm mạnh và điểm yếu riêng.

## Arduino IDE

Arduino IDE là một phần mềm đơn giản và dễ sử dụng được thiết kế dành riêng cho nền tảng Arduino. Nó cung cấp một giao diện trực quan để viết và nạp chương trình vào mạch điều khiển và nó thích hợp với những dự án đơn giản và cho người dùng mới làm quen với hệ thống nhúng.

### Ưu điểm&#x20;

* Đơn giản và dễ sử dụng
* Được thiết kế để dành riêng cho nền tảng Arduino
* Có cộng đồng lớn
* Hỗ trợ nhiều thư viện và mạch khác nhau

### Ngược điểm&#x20;

* Không có nhiều tính năng như nhiều IDE khác
* Có thể gặp vấn đề khi sử dụng với những dự án có quy mô lớn hơn
* Không sử dụng tốt với nền tảng ngoài Arduino

## PlatformIO IDE

Mặt khác, PlatformIO lại là một phần mềm mạnh mẽ và nhiều tính năng hơn. Nó hỗ trợ một lượng rất lớn các nền tảng hệ thông nhúng khác nhau, và cung cấp một lượng lớn các công cụ về quản lí thư viện, CI, Unit Testing và Debugging. PlatformIO IDE phù hợp với các dự án lớn hơn và dành cho người đã có kinh nghiệm cần những tính năng nâng cao.&#x20;

### Ưu điểm

* Mạnh mẽ và nhiều tính năng hơn Arduino IDE
* Hỗ trợ lượng lớn các nền tảng nhúng, bao gồm Arduino, ESP8266, ESP32, STM32 và Raspberry Pi
* Được xây dụng trên Visual Studio Code, nên tính mở rộng rất lớn và tuỳ biến cao.
* Hỗ trợ Debugging, Unit Testing và CI.&#x20;

### Ngược điểm

* Phức tạp hơn so với Arduino IDE.
* Không được hỗ trợ trực tiếp từ Arduino.

## Nên chọn cái nào ?

Nếu bạn là người mới, chưa biết nhiều về lập trình hoặc làm việc cho một dự án nhỏ, thì Arduino IDE là một lựa chọn đáng để cân nhắc. Nó dễ để học và sử dụng hơn, và có cộng đồng rất lớn người dùng có thể hỗ trợ bạn khi gặp vấn đề.

Nhưng nếu bạn đang làm việc trong một dự án lớn hơn và cần nhiều tính năng nâng cao, thì PlatformIO lại là một lựa chọn tốt hơn bởi sự mạnh mẽ và linh động của nó. Tuy nhiên nó cũng phức tạp và khó làm quen hơn.

Cuối cùng, lựa chọn tốt nhất sẽ phụ thuộc vào nhu cầu của bạn. Đối với thành viên của Stemist MSE, các thành viên sẽ được làm quen với Arduino IDE trước, và sẽ được giới thiệu về PlatformIO sau khi đã có kinh nghiệm.
