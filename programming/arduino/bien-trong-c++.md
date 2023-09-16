# Biến trong C++

Biến là các "thùng chứa" được dùng để lưu trữ dữ liệu.&#x20;

Trong C++, mỗi biến sẽ có các kiểu dữ liệu khác nhau và xác định. Điều đó có nghĩa rằng khi tạo một biến thì bạn phải cung cấp cho nó kiểu giá trị nhất định. Điều này khác với các ngôn ngữ bậc cao như Python khi bạn có thể tạo biến mà không cần phải xác định kiểu dữ liệu cho trước (đây là một thói quen xấu khi lập trình nhưng sẽ thuận lợi cho người mới vì không phải ghi nhớ các từ khoá và kiểu dữ liệu).

## Tạo một biến

Để tạo một biến thì bạn cần chỉ định một kiểu dữ liệu và giá trị của nó:&#x20;

```cpp
int a = 1;     // kiểu_dữ_liệu tên_biến = giá_trị_của_biến;
```

Trong đó **kiểu dữ liệu** là một trong các kiểu dữ liệu trong C++ (ví dụ như `int` là kiểu số nguyên), và **tên biến** là tên của biến đó (ví dụ như biến có tên là `a`). **Dấu bằng** có tác dụng xếp giá trị của biến đó bằng một giá trị.&#x20;

Ngoài ra bạn có thể tạo ra một biến mà không có giá trị, và xếp giá trị cho chúng sau:&#x20;

```cpp
int myNum;      //tạo biến kiểu nguyên myNum mà không có giá trị nào cả.
myNum = 15;     //myNum bây giờ đã có giá trị là 15
```

Và bạn cũng có thể thay đổi giá trị của biến bằng cách ghi đè:

```cpp
int myNum = 15;  // myNum có giá trị là 15
myNum = 10;  // Bây giờ myNum có giá trị là 10
```

Ngoài ra bạn cũng có thể tạo ra nhiều biến với cùng một kiểu dữ liệu như sau:

```cpp
int x = 5, y = 6, z = 50; 
// Tạo ra biến nguyên x,y,z với giá trị tương ứng là 5,6 và 50.
```

Và cũng có điều tương tự nếu bạn muốn gắn 1 giá trị cho nhiều biến cùng một lúc như sau:

```cpp
int x, y, z; // Tạo biến nguyên x,y,z
x = y = z = 50; // Cả 3 biến x,y,z đều có giá trị là 50
```

## Các kiểu dữ liệu

Trong C++ có rất nhiều các kiểu dữ liệu, bao gồm các kiểu dữ liệu được định sẵn. Ngoài ra bạn cũng có thể tạo ra kiểu dữ liệu của mình.&#x20;

{% hint style="info" %}
Trong bài tiếp theo bạn sẽ được biết về các kiểu dữ liệu định sẵn, bao gồm các kiểu dữ liệu cơ bản và phổ biến nhất. Xem thêm tại [kieu-du-lieu.md](kieu-du-lieu.md "mention").
{% endhint %}

## Tên biến

Tất cả các biến trong C++ đều **phải** được định nghĩa với tên **khác nhau.**

Các tên biến đó cũng có thể được hiểu là định danh. Tên biến có thể đơn giản như x,y hoặc là tên dễ xác định hơn như userName, gradeNum,...

{% hint style="warning" %}
Bạn nên đặt tên biến sao cho dễ hiệu nhất mà không làm cho tên biến quá dài và khó nhớ:

```cpp
string userEmail = "thaimeo200389@gmail.com" // Tên biến ngắn, dễ hiểu.
// Ngắn, nhưng gây khó hiểu vì không biết m ở đây là gì.
string m = "thaimeo200389@gmail.com" 
/* Tên biến dễ hiểu nhưng quá dài khiến cho việc truy xuất biến mất 
 thời gian hơn */
string userEmailAddress = "thaimeo200389@gmail.com" 
```
{% endhint %}

{% hint style="info" %}
Quy tắc đặt tên biến thông dụng là:

* Đặt tên biến sao cho có ý nghĩa và miêu tả được mục đích sử dụng của biến.
* Tên biến có thể có chữ hoa, chữ thường, chữ số và dấu gạch dưới.
* Tên biến bắt buộc phải bắt đầu bằng một chữ cái hoặc dấu gạch dưới.
* Tên biến có phân biệt chữ hoa và chữ thường (`username` và `userName` là 2 biến khác nhau)&#x20;
* Tên biến không thể chứa khoảng trắng hoặc các ký tự đặc biệt như !,%,#,...
* Tên biến không thể trùng với các từ khoá được sử dụng trong C++ (tên biến không thể là int, float,...)&#x20;
* Đặt tên biến theo kiểu camelCase hoặc PascalCase.
* Đối với biến toàn cục (global) thì nên thêm tiền tố g\_ hoặc một cách khác để phân biệt được biến nội bộ với biến toàn cục.&#x20;
* Đối với các hằng số, sử dụng chữ hoa và dấu gạch dưới để phân cách các từ, ví dụ:  `const unsigned int MAX_PWM = 4096`.
{% endhint %}

## Hằng số

Khi bạn không muốn người khác (hoặc chính bản thân bạn) thay đổi giá trị của một biến nào đó, hãy dùng `const` trước kiểu dữ liệu của tên biến đó.&#x20;

{% hint style="info" %}
`const` ở đây có nghĩa là constant hay còn gọi là hằng số - biến đó sẽ là chỉ đọc và không bao giờ thay đổi.&#x20;
{% endhint %}

Bạn luôn nên định nghĩa một biến là hằng số nếu bạn muốn tạo một biến có giá trị cố định và không bao giờ thay đổi, điều này sẽ khiến cho bạn hoặc người khác không vô tình làm thay đổi giá trị đó.

```cpp
const int PI = 3.14;  // Biến PI sẽ luôn có giá trị là 3.14
PI = 9.8;  // error: assignment of read-only variable 'PI' 
```
