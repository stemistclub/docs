# Pulse-width modulation (PWM)

## Định nghĩa

**PWM** là phương pháp lấy tín hiệu **analog** bằng việc **sử dụng tín hiệu digital** qua việc **lặp đi lặp lại chu kỳ bật/tắt** trong một chu kỳ thời gian.

Thời gian mà tín hiệu bật được gọi là **độ rộng xung (pulse width)**. Thời gian mà tín hiệu bật khi kết thúc một chu kỳ được gọi là **duty cycle**, và duty cycle quyết định đến tín hiệu trả về thực tế.

<figure><img src="../../../../.gitbook/assets/image (37).png" alt=""><figcaption><p>Tần số PWM là 500Hz – 2 giây mỗi chu kỳ</p></figcaption></figure>

Trong ví dụ trên thì ta thấy rằng tín hiệu đang ở mức 0%, 25%(1/4 trong 2 giây chu kỳ), 50% (1/2 trong 2 giây chu kỳ), 75%(3/4 trong 2 giây chu kỳ) và 100%.

## Đối với Arduino

Với Arduino, thì việc sử dụng PWM dễ dàng hơn rất nhiều, chỉ bằng việc sử dụng `analogWrite(pin, dutyCycle)` với `dutyCycle` là giá trị trong khoảng từ `0` đến `255` và `pin`PWM (`~`). Hàm `analogWrite()` cung cấp khả năng tương tác đơn giản với PWM, nhưng hàm này không cho chúng ta kiểm soát về tần số.

{% hint style="info" %}
Mặc dù tên hàm là `analogWrite()`, nhưng thực chất tín hiệu đầu ra vẫn là digital (tín hiệu 0 và 1 như trong ảnh minh hoạ)
{% endhint %}

{% hint style="info" %}
Ta có thể sử dung PWM theo cách thủ công trên gần như mọi pin qua cách liên tiếp bật/tắt trong một khoảng thời gian.
{% endhint %}

## Sử dụng PWM thủ công

<pre class="language-cpp"><code class="lang-cpp"><strong>void setup(){
</strong>    pinMode(13, OUTPUT);
}

void loop(){
    digitalWrite(13, HIGH);
    delayMicroseconds(100); // Khoảng 10% duty cycle @ 1KHz
    digitalWrite(13, LOW);
    delayMicroseconds(1000 - 100);
}
</code></pre>

Ưu điểm của phương pháp này là có thể áp dụng với mọi pin digital và có toàn quyền kiểm soát **duty cycle** và tần số.

**Ngược điểm** lớn nhất đó là mọi ngắt quãng sẽ ảnh hưởng đến bộ đếm thời gian, và từ đó nó gây ra loạn tín hiệu rất lớn nếu ta không loại bộ yếu tố ngắt quãng đấy và rất khó để xác định các hằng số thích hợp cho một chu kỳ và tần số cụ thể trừ khi ta đếm cẩn thận các chu kỳ hoặc điều chỉnh các giá trị trong khi xem máy hiện sóng.

## Ứng dụng

PWM được sử dụng để điều tốc động cơ, bằng chính duty cycle của tín hiệu, ví dụ như 25% duty cycle sẽ cho động cơ chạy 25% vận tốc tối đa của chúng.

Với servo 360 độ thì chúng hoạt động tương tự như động cơ.

Còn đối với servo 180 độ thì PWM được sử dụng để thay đổi góc quay. Với 0% duty cycle là 0 độ và 100% duty cycle ứng với 180 độ. Ngoài ra có một thư viện Servo được tạo ra nhằm giúp chúng ta có thể dễ dàng chỉnh góc quay servo theo ý muốn bằng độ (0-180).

Tuy nhiên do bộ đếm thời gian của thư viện servo, nên khi làm các dự án phức tạp hơn, như làm robot phải xử lí tín hiệu liên tục, thì thư viện này sẽ làm gián đoạn (interupt) việc xử lí tín hiệu, và dẫn đến hậu quả như đề cập ở phần trước rằng nó sẽ gây là loạn tín hiệu, vì thế nên thư viện Servo chỉ nên được sử dụng khi làm các project đơn giản, đối với project yêu cầu xử lí cao hơn thì ta nên sử dụng PWM thủ công.
