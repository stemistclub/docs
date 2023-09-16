# Cấu trúc một chương trình Arduino

## Ví dụ

Trước khi tìm hiểu cấu trúc của một chương trình Arduino, chúng ta hãy xem qua một ví dụ về chương trình mẫu như sau:

```cpp
#include <Arduino.h>

// put function declarations here:
int myFunction(int, int);

void setup() {
  // put your setup code here, to run once:
  int result = myFunction(2, 3);
}

void loop() {
  // put your main code here, to run repeatedly:
}

// put function definitions here:
int myFunction(int x, int y) {
  return x + y;
}
```

Ở dòng đầu tiên, `#include <Arduino.h>` chính là các file header. Các file header này giúp cho chương trình của chúng ta được mở rộng thêm. Trong trường hợp này là sẽ thêm các hàm dùng cho Arduino.

Chương trình này bao gồm 2 hàm bắt buộc đó là `setup()` và `loop()` , ngoài ra còn có thêm hàm tự định nghĩa (trong trường hợp này là hàm `myFunction()` .&#x20;

Bạn cũng sẽ thấy đường rằng các đoạn mã xử lí đều được nằm trong một hàm và gói gọn bằng dấu ngoặc `{}`. Tất cả các câu lệch ở trong dấu ngoặc đó sẽ được thực thi khi hàm đó được gọi. Ngoài ra các câu lệch đều có dấu `;` ở cuối dòng, đây là cách để giúp cho trình biên dịch biết rằng đó là điểm kết thúc của một câu lệch.

Chương trình này sẽ tạo ra một hàm tự định nghĩa đó là hàm `myFunction()` với kiểu giá trị trả về là kiểu số nguyên (`int`), nhận vào hai giá trị nguyên đầu vào là `x` và `y`, rồi sau đó tiến hành trả kết quả của hàm là tổng của chúng. Và cuối cùng là khi Arduino khởi động hàm `setup()` lần đầu tiên, sẽ lưu biến kiểu số nguyên `result` với giá trị là kết quả của hàm `myFunction().`

{% hint style="info" %}
Đừng lo nếu bạn không hiểu đoạn vừa rồi, đó chỉ là cách diễn giải cách chương trình trên hoạt động. Trong tương lại bạn hoàn toàn có thể đọc được code mà không cần phải đọc giải thích.
{% endhint %}

## Hai hàm bắt buộc

Trong Arduino bắt buộc phải có sự tồn tại của hai hàm sau, đó chính là hàm `setup()` và `loop()`

* Hàm `setup()` chỉ được thực thi tự động một lần duy nhất, đó là khi mạch được khởi động. Với hàm này ta thường dùng để định nghĩa như là kiểu đầu vào / ra của chân tín hiệu, khởi tạo giao tiếp serial với tốc độ (baudrate) chỉ định hoặc khởi tạo hàm thiết lập của một thư viện.
* Hàm `loop()` là nơi mà chương trình chính của chúng ta sẽ được chạy như là một vòng lặp (lặp đi lặp lại cho đến khi nào mạch tắt nguồn), ví dụ như bật/tắt led sau 2 giây (2000 miliseconds), quay servo khi cảm biến được kích hoạt,...
* Trong [#vi-du](cau-truc-mot-chuong-trinh-arduino.md#vi-du "mention") bạn sẽ thấy rằng trước hai hàm bắt buộc vừa kể trên có cụm từ `void` ở phía trước. `void` ở đây có nghĩa là hàm này sẽ không trả về một giá trị nào cả.

{% hint style="info" %}
Những hàm trên là những hàm bắt buộc phải có trong chương trình Arduino, nhưng chúng ta luôn có thể tạo ra những hàm mới ví dụ như hàm `myFunction()` ,điều này hữu ích khi ta viết những chương trình phức tạp.&#x20;
{% endhint %}

## Quy trình chạy của Arduino

Quy trình chạy của Arduino như các ngôn ngữ lập trình khác sẽ dịch và chạy chương trình từ trên xuống dưới của source code. Và giả sử chương trình đã được biên dịch và khởi động, chúng sẽ gọi hàm setup() đầu tiên và chỉ một lần duy nhất, sau đó là hàm loop() và sẽ chạy trong vòng lặp không ngừng.

Và bởi vì chương trình cũng được biên dịch từ trên xuống, nên nếu bạn viết như sau, trình biên dịch sẽ báo lỗi:

```cpp
#include <Arduino.h>

void setup() {
  // put your setup code here, to run once:
  int result = myFunction(2, 3);
}

void loop() {
  // put your main code here, to run repeatedly:
}

// put function definitions here:
int myFunction(int x, int y) {
  return x + y;
}
```

```
Compiler:
src\main.cpp: In function 'void setup()':
src\main.cpp:5:16: error: 'myFunction' was not declared in this scope
```

Do khi chương trình dịch đến dòng `int result = myFunction(2, 3);`trình biên dịch sẽ nhận ra rằng nó không tìm thấy hàm nào có tên là `myFunction()` dẫn đến việc trình biên dịch sẽ để lại lỗi như trên bất chấp ở các dòng dưới hàm `myFunction()` đã được định nghĩa.&#x20;

Giải pháp cho vấn đề này đó là định nghĩa trước về hàm:

```cpp
#include <Arduino.h>

// put function declarations here:
int myFunction(int, int);

void setup() {
  // put your setup code here, to run once:
  int result = myFunction(2, 3);
}
```

Cho dù hàm không có nội dung bên trong hàm, mà nội dung hàm chỉ được định nghĩa ở cuối chương trình, nhưng khi biên dịch thì trình biên dịch sẽ tự ghi đè nội dung của hàm.&#x20;
