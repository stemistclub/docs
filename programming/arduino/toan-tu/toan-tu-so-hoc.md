# Toán tử số học

Toán tử số học hiểu đơn giản là các phép tính toán đơn giản mà chúng ta đã được học từ bé tới giờ, khi học C++ nó được mở rộng thêm 1 vài thứ hay ho giúp ích cho chúng ta rất nhiều.

**TỔNG QUAN:**

<figure><img src="../../../.gitbook/assets/Screenshot 2023-09-16 140409.png" alt=""><figcaption></figcaption></figure>

Để hiểu sâu hơn , chúng ta cùng xem qua các ví dụ để biêt đc cách hoạt động của toán tử số học.&#x20;



* Toán tử: <mark style="color:blue;">+ (cộng / addition)</mark>:&#x20;

```cpp
int a = 10, b = 3;
cout << a + b;
// trên màn hình sẽ in ra: 13 (Kết quả của a + b)
```

* Toán tử: <mark style="color:blue;">- (trừ / Subtraction )</mark>:&#x20;

```cpp
int a = 10, b = 3;
cout << a - b:
// trên màn hình sẽ in ra: 7 (kết quả của a - b)
```

* Toán tử: <mark style="color:blue;">\* (nhân / Multiplication)</mark>:&#x20;

```cpp
int a = 10, b = 3;
cout << a * b;
// trên màn hình sẽ in ra: 30 (kết quả của a * b)
```

* Toán tử: <mark style="color:blue;">/ (chia / Division)</mark>:

```cpp
int a = 10, b = 3;
cout << a / b;
// trên màn hình sẽ in ra: 3 
```

{% hint style="info" %}
Lưu ý: vì chúng ta khai báo a và b là số nguyên nên kết quả sẽ chỉ lấy phần nguyên

a / b = 3,333 nhưng khi khai báo là int thì => a / b = 3
{% endhint %}

* Toán tử: <mark style="color:blue;">% (chia lấy dư / Modulus)</mark>: đây là phép tính mới, được mô tả là lấy số dư của phép tính chia

```cpp
int a = 10, b = 3;
cout << a % b;
// kết quả sẽ in ra là: 1 (vì 10 / 3 = 3 và dư 1)
```

* Toán tử: <mark style="color:blue;">++ (tăng / Increment)</mark> : đơn giản là tăng lên 1 số

```cpp
int a = 10, b = 3;
cout << ++a << " " << ++b;
// màn hình sẽ in ra số: 11 4
```

Toán tử: <mark style="color:blue;">--(giảm / Decrement)</mark>: giảm 1 số

```cpp
int a = 10, b = 3;
cout << --a <<  " " << --b;
// in ra: 9 2
```
