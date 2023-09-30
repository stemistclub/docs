# Nhập xuất Analog

Giống như Digital, ta có thể nhập cũng xuất tín hiệu analog bằng 2 lệnh đơn giản: `analogWrite()` và `analogRead()`.

* `analogWrite(pin, giá trị)` : Xuất ra giá trị analog tại chân pin với giá trị 10-bit (0-1023).
* `analogRead(pin)` : Xuất ra giá trị analog được nhập vào từ thiết bị bên ngoài vào tại chân pin hay nói cách khác thì analogRead sẽ trả về giá trị 0-1023 từ giá trị mà nó đọc được tại chân pin.

