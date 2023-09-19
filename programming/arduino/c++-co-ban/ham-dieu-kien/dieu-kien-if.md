# Điều kiện if

## Định nghĩa&#x20;

Hàm điều kiện `if` được dùng để định nghĩa các hàm được nằm bên trong nó được khởi động khi điều kiện trong hàm được thoả mãn. Điều kiện của hàm được giới hạn bằng dấu ngoặc đơn `()` và nội dung hàm được giới hạn bằng dấu ngoặc nhọn `{}`

```cpp
int a = 9;
if ( a % 3 == 0 ) {
    // Nội dung bên trong này sẽ được thực thi nếu điều kiện của hàm là True.
    Serial.println("Số vừa nhập chia hết cho 3");
}
```

Trong ví dụ trên, ta đặt biến nguyên `a` có giá trị là 9. Và trong hàm điều kiện `if` ở phần điều kiện nếu biến `a` chia hết cho 3 (chia cho 3 dư 0) thì nội dung bên trong hàm là hiển thị : "Số vừa nhập chia hết cho 3" ra Serial.&#x20;

Về logic, vì 9 chia cho 3 dư 0 cho nên điều kiện `a % 3 == 0` sẽ trả về giá trị là True. Vì vậy nội dung nằm bên trong hàm sẽ được thực thi. Ví dụ trên sử dụng toán tử so sánh bằng `==`

## Cấu trúc

```cpp
if (điều kiện) {
    // nội dung hàm sẽ được thực thi nếu điều kiện được thoả mãn
}
```
