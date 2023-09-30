# Hàm (Function)

## Định nghĩa

**Hàm (function)** là một đoạn chương trình có tên, đầu vào và đầu ra. **Hàm** có chức năng giải quyết một số vấn đề chuyên biệt cho chương trình chính.

Hàm có thể được gọi nhiều lần với các tham số khác nhau và là một đơn vị độc lập của chương trình, không cho phép xây dựng một hàm bên trong một hàm khác.

Cách xây dựng hàm:

```cpp
<kiểu hàm> <tên hàm> (tham số) {
    <nội dung hàm> 
    return <giá trị trả về>;
}
```

## Ví dụ:

```cpp
float doSum(float a,float b) {
    float sum = a + b;
    return sum;
}
```

Trong ví dụ trên, hàm được định nghĩa có tên là `doSum` với kiểu hàm là `float` (số thực) với tham số là 2 giá trị thực `a` và `b`. Khi phân tích nội dung hàm thì ta dễ thấy rằng biến thực `sum` được gán giá trị là toán tử tổng của `a` và `b`. Sau đó hàm kết thúc với giá trị được trả về là giá trị của biến `sum`.
