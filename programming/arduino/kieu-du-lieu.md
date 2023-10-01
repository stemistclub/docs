# Kiểu dữ liệu định sẵn

Mỗi dữ liệu khi lưu trữ đều có kiểu dữ liệu riêng của nó, sau đây là các kiểu dữ liệu phổ biến:&#x20;

```cpp
int myNum = 5;               // Số nguyên
float myFloatNum = 5.99;     // Số thực
double myDoubleNum = 9.98;   // Số thực
bool myBoolean = true;       // Boolean
char myLetter = 'D';         // Ký tự
string myText = "Hello";     // Kiểu sâu
```

### Số nguyên

Là kiểu dữ liệu dùng để lưu trữ số nguyên (bao gồm cả số dương và số âm). Sau dây là một trong những kiểu dữ liệu số nguyên thông dụng:

<table data-full-width="false"><thead><tr><th>Kiểu dữ liệu</th><th>Kích cỡ (bytes)</th><th>Vùng</th></tr></thead><tbody><tr><td><code>short int</code></td><td>2</td><td>-32,768 to 32,767</td></tr><tr><td><code>unsigned short int</code></td><td>2</td><td>0 to 65,535</td></tr><tr><td><code>unsigned int</code></td><td>4</td><td>0 to 4,294,967,295</td></tr><tr><td><code>int</code></td><td>4</td><td>-2,147,483,648 to 2,147,483,647</td></tr><tr><td><code>long int</code></td><td>4</td><td>-2,147,483,648 to 2,147,483,647</td></tr><tr><td><code>unsigned long int</code></td><td>4</td><td>0 to 4,294,967,295</td></tr><tr><td><code>long long int</code></td><td>8</td><td>-(2^63) to (2^63)-1</td></tr><tr><td><code>unsigned long long int</code></td><td>8</td><td>0 to 18,446,744,073,709,551,615</td></tr></tbody></table>

Mặc dù các kiểu dữ liệu định sẵn ở trên chưa phải là đầy đủ nhất, nhưng bạn không cần quan tâm đến các kiểu dữ liệu ở trên mà chỉ tập trung duy nhất vào kiểu dữ liệu `int` nếu bạn muốn biểu diễn một số nguyên. Các kiểu dữ liệu khác sẽ hữu ích trong tương lai nhưng về cơ bản bạn chỉ cần quan tâm đến `int`.

### Số chấm động.&#x20;

Là kiểu dữ liệu dùng để lưu trữ các số thập phân (ví dụ như -1.5, 3.14).&#x20;

| Kiểu dữ liệu  | Kích cỡ (bytes) | Vùng                       |
| ------------- | --------------- | -------------------------- |
| `float`       | 4               | -3.4×10^38 to 3.4×10^38    |
| `double`      | 8               | -1.7×10^308 to1.7×10^308   |
| `long double` | 12              | -1.1×10^4932 to1.1×10^4932 |

* **Độ chính xác** của số chấm động là số chữ số nằm sau dấu . mà kiểu dữ liệu đó có thể lưu trữ được.
* `float` có thể lưu trữ được đến 6 hoặc 7 chữ số.
* `double` thì lại có thể lưu trữ được đến 15 chữ số.&#x20;
* Với các phép tính toán, bạn nên dùng `double` để đảm bảo về độ chính xác.

### Boolean, ký tự và kiểu sâu.

#### Boolean

* Là kiểu dữ liệu được định nghĩa bằng từ khoá `bool` và chỉ có thể nhận được hai giá trị duy nhất đó là `True` hoặc `False`.&#x20;
* Khi Boolean được trả về sẽ trả về `True` = `1` hoặc `False` = `0`.
* Kiểu ký tự `bool` có kích cỡ là 1 byte.

{% hint style="info" %}
Kiểu Boolean thường hay được sử dụng để làm điều kiện kiểm tra, và sẽ được nhắc đến trong hàm điều kiện.
{% endhint %}

#### Ký tự

Kiểu dữ liệu `char` được dùng để lưu trữ duy nhất 1 ký tự. Và được bao quanh bởi dấu nháy đơn (Ví dụ như `'A'` hoặc `'x'` ).

Kiểu ký tự `char` có kích cỡ là 1 byte.

#### Kiểu sâu

Kiểu `string` được dùng để lưu trữ một dãy các ký tự. Và được bao quanh bởi dấu nháy kép (Ví dự như `"Stemist Club"` hay `"Chao"` )

Trong C, kiểu sâu thậm chí không tồn tại, và các để có được dạng kiểu sâu này đó chính là việc dùng mảng với kiểu char. Trong C++, để dùng string ta cần thêm thư viện `<string>`. Nhưng trong Arduino đã có kiểu dữ sâu sẵn đó là `String` (với chữ S viết hoa). Nó hoạt động tương tự như kiểu sâu trong C++, là mảng chứa các ký tự khác nhau, điều này sẽ được đề cập rõ hơn ở phần Mảng.&#x20;

{% hint style="info" %}
Đây là kiến thức cơ bản và là nền tảng để bắt đầu với lập trình, tuy nhiên hiện tại bạn chỉ cần ghi nhớ như sau:

* Nếu bạn chỉ cần làm việc với số nguyên, hãy dùng `int`.
* Nếu bạn cần làm chức năng cần sử dụng đến số thập phân hoặc tính toán, dùng `float` hoặc `double`.
* Nếu bạn chỉ cần làm việc với một ký tự duy nhất, dùng `char`.
* Nếu bạn chỉ cần làm việc với một dãy chữ như một từ hoặc 1 câu văn, dùng `string`.

Ngoài các kiểu dữ liệu định sẵn ra, bạn có thể tự tạo ra một kiểu dữ liệu mà bạn tự định nghĩa. Tuy nhiên điều này sẽ không được đề cập trong tài liệu này.
{% endhint %}

