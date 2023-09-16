# Toán tử số học

Toán tử số học hiểu đơn giản là các phép tính toán đơn giản mà chúng ta đã được học ngay từ bậc Tiểu học.&#x20;

<table data-full-width="false"><thead><tr><th width="121">Toán tử</th><th width="134">Định nghĩa</th><th width="315">Giải thích</th><th width="225">Ví dụ</th></tr></thead><tbody><tr><td>+</td><td>Cộng</td><td>Cộng hai số hạng với nhau</td><td>x + y</td></tr><tr><td>-</td><td>Trừ</td><td>Trừ số thứ nhất cho số thứ 2</td><td>x - y</td></tr><tr><td>*</td><td>Nhân</td><td>Nhân 2 số</td><td>x * y</td></tr><tr><td>/</td><td>Chia </td><td>Chia số thứ nhất cho số thứ 2</td><td>x / y</td></tr><tr><td>%</td><td>Chia lấy dư</td><td>Trả về số dư của phép chia </td><td>x % y</td></tr><tr><td>++</td><td>Thăng</td><td>Tăng giá trị của một biến lên 1</td><td>++x</td></tr><tr><td>--</td><td>Giáng</td><td>Giảm giá trị của một biến xuống 1</td><td>--x</td></tr></tbody></table>

Để hiểu sâu hơn, chúng ta cùng xem qua các ví dụ để được cách hoạt động của toán tử số học.&#x20;

* Toán tử: `+` <mark style="color:blue;">(Cộng / Addition)</mark>:&#x20;

```cpp
int a = 10, b = 3;
int sum << a + b; // 13 (Kết quả của a + b)
```

* Toán tử: `-` <mark style="color:blue;">(Trừ / Subtraction)</mark>:&#x20;

```cpp
int a = 10, b = 3;
int sub << a - b: // 7 (Kết quả của a - b)
```

* Toán tử: <mark style="color:blue;">`*`</mark> <mark style="color:blue;"></mark><mark style="color:blue;">(Nhân / Multiplication)</mark>:&#x20;

```cpp
int a = 10, b = 3;
int mul << a * b; // 30 (Kết quả của a * b) 
```

* Toán tử: `/` <mark style="color:blue;">(Chia / Division)</mark>:

```cpp
int a = 10, b = 3;
int divis << a / b; // 3 (Kết quả của a/b nhưng trả về giá trị nguyên)
```

{% hint style="info" %}
Vì chúng ta khai báo biến a và b là số nguyên nên kết quả sẽ chỉ lấy phần nguyên

a / b = 3,333 nhưng khi khai báo là int thì => a / b = 3
{% endhint %}

* Toán tử: `%` <mark style="color:blue;">(Chia lấy dư / Modulus)</mark>:

```cpp
int a = 10, b = 3;
cout << a % b; // 1 (vì 10 / 3 = 3 và dư 1)
```

* Toán tử: `++` <mark style="color:blue;">(Thăng / Increment):</mark>

```cpp
int a = 10, b = 3;
cout << ++a << " " << ++b; // 11 4
```

Toán tử: `--` <mark style="color:blue;">(Giáng / Decrement)</mark>: giảm 1 số.

```cpp
int a = 10, b = 3;
cout << --a <<  " " << --b; // 9 2
```
