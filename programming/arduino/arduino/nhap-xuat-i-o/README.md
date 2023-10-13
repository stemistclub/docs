# Nhập / Xuất (I/O)

Khi chúng ta viết một chương trình thì việc lấy dữ liệu từ một thiết bị và sau đó dựa vào kết quả mà thiết bị đó thu được qua các điều kiện xác định để thực hiện một hành động nào đó.&#x20;

Trong ví dụ dưới đây sử dụng một bút bấm và đèn LED. Ta có thể viết hàm điều kiện để kiểm tra xem mỗi khi nút được bấm thì đèn LED sẽ sáng lên và tắt đi khi nút được thả ra.&#x20;

```cpp
int buttonState = digitalRead(buttonPin);   //đọc và lưu giá trị đọc được từ nút bấm

if(buttonState == HIGH){        //kiểm tra nếu điều kiện là đúng (nút được bấm)
    digitalWrite(LED, HIGH);    //bật sáng LED
} else {
    digitalWrite(LED, LOW);     //tắt LED
}
```
