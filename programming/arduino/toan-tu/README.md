# Toán tử

Toán tử là một biểu tượng hoạt động trên giá trị để thực hiện các phép tính logic và toán học cụ thể. Chúng tạo thành nền tảng của bất cứ ngôn ngữ lập trình nào.&#x20;

Trong C++, chúng ta có sẵn các toán tử để cung cấp chức năng cần thiết.

Trong ví dụ dưới đây sử dụng toán tử cộng `+` để cộng 2 giá trị vào với nhau:

```cpp
int x = 100 + 50; 
```

Mặc dù toán tử cộng `+` thường được dùng để cộng 2 giá trị vào nhau, toán tử cộng cũng có thể cộng giá trị với một biến, hoặc một biến với một biến hay là cộng nhiều giá trị vào với nhau:&#x20;

```cpp
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400) 
int sum4 = sum1 + sum2 + sum3 // 1350 (150 + 400 + 800)
```

Toán tử trong C++ được chia thành các nhóm toán tử sau:&#x20;

* [toan-tu-so-hoc.md](toan-tu-so-hoc.md "mention")
* [toan-tu-gan.md](toan-tu-gan.md "mention")
* [toan-tu-so-sanh.md](toan-tu-so-sanh.md "mention")
* [toan-tu-logic.md](toan-tu-logic.md "mention")

{% hint style="warning" %}
Bởi toán tử là một trong những nền tảng quan trọng trong lập trình, nên bạn cần phải hiểu rõ tất cả các toán tử.&#x20;
{% endhint %}

{% hint style="info" %}
Tuy nhiên đối với những người chưa có kinh nghiệm về lập trình từ trước, việc "học" các toán tử này sẽ thấy khó khăn, điều này có thể giải quyết bằng cách tạo "liên hệ" với nó. Ví dụ như `=` là gắn, vậy nếu muốn so sánh xem biến a có giá trí bằng 2 hay không thì ta phải dùng `==`. Từ `==` mà muốn kiểm tra khác 2 thì ta thay `==` thành `!=`,... &#x20;

Nếu bạn vẫn gặp khó khăn, hãy cứ xem đây là nơi tổng hợp các toán tử mà bạn cần để có thể tra cứu lại. Theo thời gian bạn sẽ quen với điều đó và dần không cần đến tài liệu này nữa.
{% endhint %}
