# Vòng lặp for

## Định nghĩa

**Vòng lặp for** được sử dụng khi bạn muốn một vòng lặp được chạy lặp lại một số lần nhất định.

```cpp
for (điều kiện khởi tạo, điều kiện thực thi, điều kiện kết thúc) {
    // nội dung
}
```

Nguyên lý hoạt động có thể được hiểu theo cách đơn giản sau:

* **Điều kiện khởi tạo** sẽ được thực thi 1 lần duy nhất, đó là khi hàm được gọi.
* **Điều kiện thực thi** sẽ thực thi nội dung bên trong khi điều kiện thực thi đó thoả mãn.&#x20;
* **Điều kiện kết thúc** sẽ được thực thi mỗi khi nội dung bên trong kết thúc.
  * Phần này thường có mục đích **tăng hoặc giảm giá trị các biến vòng lặp**. Sau khi thực thi xong, vòng lặp **quay lại kiểm tra điều kiện lặp ở bước 2**.

## Ví dụ

```cpp
for (int count = 0; count < 10; ++count) {
    Serial.print(count);
    //output: 0123456789
}
```

Trong ví dụ trên, biến nguyên `count` được tạo với giá trị là `0`, sau đó vì biến count thoả mãn điều kiện **nhỏ hơn 10** nên nội dung bên trong hàm sẽ được thực thi để hiển thị ra giá trị của biến `count`. Sau khi nội dung bên trong đã kết thúc, **điều kiện kết thúc** được thực thi đó là cộng thêm một vào giá trị của biến `count`.&#x20;

Sau đó biến count sẽ có giá trị là 0 + 1 = 1 và thoả mãn điều kiện **nhỏ hơn 10** nên vẫn sẽ tiếp tục thực thi. Cho đến khi `count = 10` và **không còn thoả mãn** điều kiện thực thi thì **vòng lặp kết thúc**.&#x20;
