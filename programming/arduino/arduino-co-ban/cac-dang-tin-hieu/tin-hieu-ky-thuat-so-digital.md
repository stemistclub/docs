# Tín hiệu kỹ thuật số (Digital)

## Khái niệm

Tín hiệu kỹ thuật số (Digital) là tín hiệu được biểu diễn bởi giá trị cố định, và chỉ có thể biểu diễn một giá trị cố định trong một thời điểm giới hạn (đối lập với Analog khi Analog biểu diễn gần như vô số giá trị).

<figure><img src="../../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

Giá trị digital được biểu diễn ở 2 mức tín hiệu cơ bản, một tín hiệu gần mốc ( gần với mức 0 hay còn gọi là ground), và một mức điện áp định mức ( thường là 5V ). Thường hai giá trị này được gán với số 0 (ground) và số 1 (supply current) giống như dạng mã nhị phân (binary) và với boolean thì là False với True.

Chính bởi vì tín hiệu được biểu diễn với các giá trị cố định này, nên là với một sự thay đổi nhỏ đến tín hiệu đều không làm thay đổi trạng thái của tín hiệu, nhờ vào định mức dữ liệu nhận vào. Và kết quả là tín hiệu digital không bị nhiễu và không ảnh hưởng đến cách hệ thống digital khác (có gây ảnh hưởng đến hệ thống analog nhưng không đáng kể.

{% hint style="info" %}
Digital thực chất là một dạng của Analog.
{% endhint %}

## Ngược điểm

Như đã đề cập ở phần Analog, ta có thể dùng ADC (Analog to Digital Converter) để giải quyết vấn đề mà Analog gặp phải.

Do bản chất của Digital, tín hiệu digital không thể cho độ chính xác như analog, tuy nhiên ta có thể biểu diễn tính hiệu của analog từ digital như hình bên, và đó là cách ADC hoạt động.

<figure><img src="../../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Để ứng dụng vào Arduino như điều khiển servo hay động cơ, thì PWM ra đời và được ứng dụng vào việc truyền tín hiệu dạng analog như điều khiển động cơ,…
