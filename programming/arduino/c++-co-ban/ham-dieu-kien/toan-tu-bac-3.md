# Toán tử bậc 3

Có một cách khác để biểu diễn hàm `if` ... `else` ... một cách ngắn hơn, nó được gọi là toán tử bậc 3 bởi vì nó chứa đến 3 toán tử.&#x20;

{% hint style="info" %}
Toán tử bậc 3 thường được dùng để thay thế hàm `if`...`else`... đơn giản bằng cách viết ngắn hơn.&#x20;
{% endhint %}

## Cấu trúc

```cpp
biến = (điều kiện) ? điều kiện đúng : điều kiện sai;
```

## Ví dụ

Thay vì viết như thế này:&#x20;

```cpp
int a = 9;
if ( a % 3 == 0 ) {
    // Nội dung bên trong này sẽ được thực thi nếu điều kiện của hàm là True.
    Serial.println("Số vừa nhập chia hết cho 3");
} else {
    // Nội dung hàm bên trong này sẽ được thực thi nếu điều kiện của hàm là False.
    Serial.println("Số vừa nhập không chia hết cho 3");
}
```

Ta có thể viết như thế này

```cpp
int a = 9;
string result = (a % 3 == 0) ? "Số vừa nhập chia hết cho 3" : "Số vừa nhập không chia hết cho 3";
Serial.println (result);
```

