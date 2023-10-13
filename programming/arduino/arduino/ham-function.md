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

## Kiểu hàm

Kiều hàm hỗ trợ tất cả các kiểu dữ liệu trong C++ được sử dụng trong biến, ngoài ra có thêm một ngoại lệ đó chính là `void`. Đồng nghĩa với đó là ngoài void ra thì ta có thể trả về giá trị nguyên, thực, một mảng (array) hay là một chuỗi xâu.

### Từ khoá `void`

`void` là một từ khóa chỉ dùng trong việc khai báo một function. Những function được khai báo với "`void`" sẽ không trả về bất kì dữ liệu nào khi được gọi. Hiểu đơn giản hơn, hàm với kiểu void không cần `return`.

```cpp
void initSensor() {
  pinMode(trigPin1, OUTPUT);
  pinMode(echoPin1, INPUT);
  distance = 0;
}
```

