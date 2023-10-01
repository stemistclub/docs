# Toán tử so sánh

Toán tử so sánh là các toán tử được dùng để so sánh giữa 2 giá trị với nhau.

Giá trị trả về của toán tử so sánh là kiểu Boolean, có nghĩa là gồm 2 giá trị là True (`1`) hoặc False (`0`) .&#x20;

{% hint style="info" %}
Toán tử so sánh rất quan trọng đối với lập trình, vì nó giúp chúng ta điều hướng và tìm ra giải pháp.
{% endhint %}

Trong ví dụ sau, chúng ta sử dụng toán tử > để tìm xem liệu 5 có lớn hơn 3 hay không:

```
int x = 5;
int y = 3;
bool result = x > y; // Trả về 1 (True) vì 5 > 3.
```

<table data-full-width="false"><thead><tr><th>Toán tử</th><th>Định nghĩa</th><th>Ví dụ</th></tr></thead><tbody><tr><td>==</td><td>Bằng</td><td>x = y</td></tr><tr><td>!=</td><td>Không bằng</td><td>x != y</td></tr><tr><td>></td><td>Lớn hơn </td><td>x > y</td></tr><tr><td>&#x3C;</td><td>Nhỏ hơn</td><td>x &#x3C; y</td></tr><tr><td>>=</td><td>Lớn hơn hoặc bằng</td><td>x >= y</td></tr><tr><td>&#x3C;=</td><td>Nhỏ hơn hoặc bằng</td><td>x &#x3C;= y</td></tr></tbody></table>

{% hint style="info" %}
Đây là các toán tử rất quen thuộc với các bạn vì các toán tử này bạn đều đã được gặp trong chương trình Toán THCS.
{% endhint %}

{% hint style="danger" %}
**Không bao giờ so sánh** **hai giá trị dấu chấm động bằng nhau hay không**. Hầu như luôn luôn có sự khác biệt nhỏ giữa hai số chấm động. Cách phổ biến để so sánh 2 số chấm động là tính khoảng cách giữa 2 số đó, nếu khoảng cách đó là rất nhỏ thì ta cho là bằng nhau. Giá trị dùng để so sánh với khoảng cách đó thường được gọi là **epsilon**.
{% endhint %}
