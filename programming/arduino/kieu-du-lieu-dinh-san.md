# Kiểu dữ liệu định sẵn

Mỗi dữ liệu khi lưu trữ đều có kiểu dữ liệu riêng của nó, sau đây là các biến phổ biến:&#x20;

### Số nguyên

Là kiểu dữ liệu dùng để lưu trữ số nguyên (bao gồm cả số dương và số âm). Sau dây là một trong những kiểu dữ liệu số nguyên thông dụng:

<table data-full-width="false"><thead><tr><th>Kiểu dữ liệu</th><th>Kích cỡ (bytes)</th><th>Vùng</th></tr></thead><tbody><tr><td><code>short int</code></td><td>2</td><td>-32,768 to 32,767</td></tr><tr><td><code>unsigned short int</code></td><td>2</td><td>0 to 65,535</td></tr><tr><td><code>unsigned int</code></td><td>4</td><td>0 to 4,294,967,295</td></tr><tr><td><code>int</code></td><td>4</td><td>-2,147,483,648 to 2,147,483,647</td></tr><tr><td><code>long int</code></td><td>4</td><td>-2,147,483,648 to 2,147,483,647</td></tr><tr><td><code>unsigned long int</code></td><td>4</td><td>0 to 4,294,967,295</td></tr><tr><td><code>long long int</code></td><td>8</td><td>-(2^63) to (2^63)-1</td></tr><tr><td><code>unsigned long long int</code></td><td>8</td><td>0 to 18,446,744,073,709,551,615</td></tr></tbody></table>

Mặc dù các kiểu dữ liệu định sẵn ở trên chưa phải là đầy đủ nhất, nhưng bạn không cần quan tâm đến các kiểu dữ liệu ở trên mà chỉ tập trung duy nhất vào kiểu dữ liệu `int` nếu bạn muốn biểu diễn một số nguyên. Các kiểu dữ liệu khác sẽ hữu ích trong tương lai nhưng về cơ bản bạn chỉ cần quan tâm đến `int`.

### Số thực&#x20;

Là kiểu dữ liệu dùng để lưu trữ các số thập phân (ví dụ như -1.5, 3.14).&#x20;

| Kiểu dữ liệu  | Kích cỡ (bytes) | Vùng                       |
| ------------- | --------------- | -------------------------- |
| `float`       | 4               | -3.4×10^38 to 3.4×10^38    |
| `double`      | 8               | -1.7×10^308 to1.7×10^308   |
| `long double` | 12              | -1.1×10^4932 to1.1×10^4932 |

* **Độ chính xác** của số thực là số chữ số nằm sau dấu . mà kiểu dữ liệu đó có thể lưu trữ được.
* `float` có thể lưu trữ được đến 6 hoặc 7 chữ số.
* `double` thì lại có thể lưu trữ được đến 15 chữ số.&#x20;
* Với các phép tính toán, bạn nên dùng `double` để đảm bảo về độ chính xác.

