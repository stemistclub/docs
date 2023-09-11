# Cài đặt trình điều khiển (driver) dành cho USB to Serial

Đối với máy tính sau khi cắm usb từ mạch điều khiển thì hệ thống thường sẽ tự động cài đặt driver để hoạt động với mạch. Trong trường hợp driver không tự động cài đặt và bạn không thể sử dụng với mạch thì bạn hãy xác định chip USB to Serial trên mạch và tìm trên internet driver tương thích.

Trong hầu hết trường hợp điều này chỉ xảy ra trên nền tảng Windows. Trên macOS Monterey trở lên (theo như phiên bản mình sử dụng) thì chưa xảy ra vấn đề gì và chỉ Plug n Play (cắm và sử dụng được ngay), và trên Linux mình chỉ cần thêm udev rules [tại đây](https://docs.platformio.org/en/stable/core/installation/udev-rules.html)

Để kiểm tra xem thiết bị của bạn đã được nhận diện hay chưa, hãy thực hiện các bước sau:

### Đối với Windows

1. Chuột phải vào Start, hoặc bấm Windows + X, hoặc mở Search và mở Device Manager.
2. Trên Device Manager, bạn hãy tìm và mở rộng mục Port (COM\&LPT).
3. Nếu máy của bạn đã nhận thiết bị thành công, ở dưới mục Port sẽ có hiện thiết bị ví dụ như: Silicon Labs CP210x USB to UART Bridge (COM 3).
4. Nếu máy của bạn không hiển thị, và có thêm phần Unknown Device, bạn hãy thử cài đặt đúng driver cho thiết bị
5. Nếu máy của bạn không hiển thị và cũng không có phần Unknown Device, bạn hãy kiểm tra cáp kết nối

### Đối với Linux

1. Mở terminal và nhập lệnh lsusb, nếu có thiết bị nào hiển thị dưới dạng ttyUSB hoặc ttyACM thì khả năng cao là đã nhận thành công
2. Nếu không hiển thị thì bạn hãy thử cài udev rules ở trên và khởi động lại máy

### Đối với macOS

Bạn hãy thử sử dụng Arduino IDE hoặc PlatformIO để kiểm tra xem có nhận thiết bị hay không và cài thêm trình điều khiển nếu cần thiết.
