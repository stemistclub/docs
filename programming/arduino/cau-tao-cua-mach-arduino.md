# Cấu tạo của mạch Arduino

<figure><img src="../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption><p>Cấu tạo của mạch Arduino Uno R3 - arduino.cc</p></figcaption></figure>

1. Vi điều khiển (Microcontroller) là nơi điều khiển tất cả các hoạt động của mạch, đóng vai trò là "bộ não" xử lí mọi tín hiệu và điều khiển chúng.
2. Cổng USB (USB Port) là cổng USB Type B, có tác dụng giao tiếp qua phương thức Serial giữa máy tính với mạch điều khiển.
3. Chip chuyển đổi tín hiệu từ Serial qua USB: Chip này đóng vai trò là đầu nối giữa tín hiệu Serial từ vi điều khiển sang USB để máy tính có thể giao tiếp.
   * Mặc dù trong mạch Arduino Uno R3 được tích hợp sẵn chip chuyển đổi và cổng USB, có một số mạch điều khiển không có hai bộ phận trên, và vì chúng chỉ có tác dụng tạo phương thức giao tiếp giữa máy tính và vi điều khiển nên không nhất thiết phải tồn tại hai bộ phận trên thì mạch điều khiển mới có thể hoạt động.
   * Vi điều khiển có thể được tái lập trình với một bộ chuyển đổi tín hiệu USB sang Serial ngoài với sự trợ giúp của 2 chân digital là 0 -> RX và 1 -> TX.
4. Chân Digital: Là các chân giao tiếp dưới dạng tín hiệu Digital, với chân có dấu (\~) là các chân có hỗ trợ băm xung PWM (Pulse-Width Modulation) và chân RX, TX như đã được nhắc ở phần trên.&#x20;
5. Chân Analog:  là các chân tín hiệu Analog ở dạng 10bit (0-1023)
6. 5V/3.3V: là những chân được dùng để cấp thêm nguồn cho thiết bị ngoài.
7. GND: hay còn được gọi là âm hoặc nối đất, được dùng để kết thúc một vòng mạch điện kín, có điện mức là 0V.
8. VIN: hay còn được gọi là Voltage In, là chân dùng để kết nối nguồn bên ngoài vào bên trong mạch Arduino.

Dựa vào các mạch Arduino khác nhau mà sẽ có các bộ phận khác nhau, nhưng hầu hết các bộ phận kể trên đều có mặt ở mọi mạch nhúng Arduino.
