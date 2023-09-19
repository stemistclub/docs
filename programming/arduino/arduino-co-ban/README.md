# Arduino cơ bản

## Cơ chế hoạt động&#x20;

Chương trình Arduino được thiết kế để chạy một chương trình duy nhất trên mạch điều khiển. Chương trình này có thể chạy duy nhất một tác vụ cùng một lúc, hoặc là cùng hàng ngàn tác vụ trong một chu kỳ chạy.&#x20;

Chương trình một khi đã được nạp vào mạch điều khiển sẽ bắt đầu chạy ngay khi nó được bật nguồn. Mỗi chương trình đều có một hàm được gọi là hàm `loop`. Bên trong hàm đó, bạn có thể yêu cầu nó bật đèn led, lấy dữ liệu của cảm biến, và nếu cảm biến gửi về một giá trị nhất định sẽ tắt hoặc nháy đèn led.&#x20;

{% hint style="info" %}
Xem thêm tại [cau-truc-mot-chuong-trinh-arduino.md](../cau-truc-mot-chuong-trinh-arduino.md "mention").
{% endhint %}
