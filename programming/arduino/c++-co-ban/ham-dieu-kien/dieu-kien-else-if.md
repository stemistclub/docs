# Điều kiện else if

## Định nghĩa

Hàm điều kiện else if được sử dụng để tạo thêm điều kiện mới nếu điều kiện trước nó không thoả mãn.

```cpp
int a = 10;
if ( a % 3 == 0 ) {
    // Nội dung bên trong này sẽ được thực thi nếu điều kiện của hàm là True.
    Serial.println("Số vừa nhập chia hết cho 3");
} else if (a % 5 == 0 ) {
    // Nội dung bên trong này sẽ được thực thi nếu điều kiện của hàm là True.
    Serial.println("Số vừa nhập chia hết cho 5");
} else {
    // Nội dung hàm bên trong này sẽ được thực thi nếu cả 2 điều kiện 
    // của hàm là False.
    Serial.println("Số vừa nhập không chia hết cho 3");
}
```

Cũng giống như các ví dụ trước đó, nhưng bây giờ đã có thêm điều kiện nếu giá trị của biến `a` chia hết cho 5 ( `a` chia cho 5 dư 0 ) thì sẽ hiển thị dòng chữ: "Số vừa nhập chia hết cho 5" trên Serial.

## Cấu trúc

```cpp
if (điều kiện 1) {
  // nội dung trong này sẽ được thực thi nếu điều kiện 1 là True.
} else if (điều kiện 2) {
  // nội dung trong này sẽ được thực thi nếu điều kiện 2 là True.
} else {
  // nội dung trong này sẽ được thực thi nếu cả 2 điều kiện là False.
}
```

