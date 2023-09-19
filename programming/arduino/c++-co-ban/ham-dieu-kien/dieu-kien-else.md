# Điều kiện else

## Định nghĩa

Hàm điều kiện else được sử dụng để định nghĩa các hàm bên trong nó được thực thi nếu điều kiện của hàm điều kiện đó không thoả mãn (`False`).

```cpp
int a = 10;
if ( a % 3 == 0 ) {
    // Nội dung bên trong này sẽ được thực thi nếu điều kiện của hàm là True.
    Serial.println("Số vừa nhập chia hết cho 3");
} else {
    // Nội dung hàm bên trong này sẽ được thực thi nếu điều kiện của hàm là False.
    Serial.println("Số vừa nhập không chia hết cho 3");
}
```

Ví dụ trên hoạt động tương tự như ví dụ ở phần trước, nhưng lần này đã có thêm điều kiện `else` và biến `a` lúc này có giá trị là 10. Nếu biến `a` không chia hết cho 3 đồng nghĩa với việc điều kiện `a % 3 == 0` trả về `False`. Lúc này nội dung trong hàm `else` sẽ được thực thi do không có điều kiện `if` nào thoả mãn.&#x20;

## Cấu trúc

```cpp
if (điều kiện) {
    // nội dung hàm sẽ được thực thi nếu điều kiện được thoả mãn
} else {
    // nội dung hàm sẽ được thực thi nếu điều kiện không được thoả mãn
}
```
