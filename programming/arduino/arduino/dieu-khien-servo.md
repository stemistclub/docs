# Điều khiển Servo

## Servo là gì ?

Định nghĩa Servo hay DC Servo đã được nhắc đến trong [co-cau-chap-hanh-actuator.md](../../../co-cau-chap-hanh-actuator.md "mention"). Nếu bạn muốn hiểu rõ hoặc chưa biết Servo là gì, bạn hãy vào [#dong-co-dc-servo-thuong-goi-tat-la-dong-co-servo](../../../co-cau-chap-hanh-actuator.md#dong-co-dc-servo-thuong-goi-tat-la-dong-co-servo "mention") để tìm hiểu thêm.

## Điều khiển Servo bằng thư viện Servo

Bản chất để điều khiển Servo, ta cần sử dụng PWM để có thể giúp Servo xác định được góc cần xoay (đối với servo 180 độ) hoặc tốc độ / chiều xoay.

Để điều khiển servo đơn giản, ta có thể sử dụng thư viện Servo ([Arduino Reference](https://www.arduino.cc/reference/en/libraries/servo/?utm\_source=platformio\&utm\_medium=piohome)) ([PlatformIO](https://registry.platformio.org/libraries/arduino-libraries/Servo)).

### Đối với Servo 180 độ

Để điều khiển Servo 180 độ, ta đưa góc muốn xoay vào thư viện và thư viện sẽ thực hiện các công việc còn lại.

<pre class="language-cpp"><code class="lang-cpp">#include &#x3C;Arduino.h>
<strong>#include &#x3C;Servo.h>
</strong>
// Điều khiển servo 180, quay liên tục từ góc 0 đến 180 độ và ngược lại.

Servo myservo;
int pos = 0; // lưu vị trí của servo

void setup() {
  myservo.attach(9);  // kết nối servo vào chân 9
}

void loop() {
  for (pos=0; pos&#x3C;=180; pos++) { // từ 0 đến 180 độ
      myservo.write(pos);
      delay(15);
  }

  // Đảo ngược quá trình từ 180 đến 0 độ
  for (pos=180; pos>=0; pos--) {
      myservo.write(pos);
      delay(15);
  }
}
</code></pre>

### Đối với Servo 360 độ

Đối với servo 360, chúng ta không thể chỉ định góc muốn xoay mà chỉ có thể thay đổi tốc độ và chiều giống như động cơ DC. Quy ước:

* Góc 0 độ : Servo xoay ngược chiều kim đồng hồ, tốc độ lớn nhất.
* Góc 90 độ : Servo đứng yên.
* Góc 180 độ: Servo xoay theo chiều kim đồng hồ, tốc độ lớn nhất.

<pre class="language-cpp"><code class="lang-cpp">#include &#x3C;Arduino.h>
#include &#x3C;Servo.h>

Servo myservo;
int pos = 0; // lưu vị trí của servo

void setup() {
  myservo.attach(9);  // kết nối servo vào chân 9
}
<strong>
</strong><strong>void loop() {
</strong>  // Servo quay về vị trí tối đa ở góc 180 độ trong 1 giây
  myservo.write(180);
  delay(1000);
  // Servo ở trạng thái đứng yên trong 1 giây
  myservo.write(90);
  delay(1000);
  // Servo quay về vị trí tối đa ở góc 0 độ trong 1 giây
  myservo.write(0);
  delay(1000);
  // Servo ở trạng thái đứng yên trong 1 giây
  myservo.write(90);
  delay(1000);
}
</code></pre>

## Điều khiển Servo thủ công.

