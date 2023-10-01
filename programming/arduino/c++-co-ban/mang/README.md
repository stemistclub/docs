# Mảng

## Định nghĩa&#x20;

**Mảng (Array)** được dùng để lưu trữ nhiều giá trị trên cùng một biến thay vì phải tạo nhiều biến khác nhau với tên khác nhau.&#x20;

### Khởi tạo mảng

Để khởi tạo biến, ta tạo biến như bình thường đó là viết **kiểu biến** và **tên** nhưng kèm với đó là **đôi ngoặc vuông** `[]` và định số phần tử bên trong mảng.&#x20;

```cpp
int senInp[5];
```

Chúng ta vừa tạo ra một mảng số **nguyên** có tên là `senInp` với **5** phần tử bên trong nó.&#x20;

### Gán giá trị cho mảng

Để có thể gán giá trị cho mảng ta có thể dùng các khởi tạo mảng với các giá trị được phân cách nhau bằng dấu `,` và nằm bên trong ngoặc nhọn `{}`.&#x20;

```cpp
int senInp[5] = {1,1,0,0,1}; 
```

hoặc là bằng cách gắn ở vị trí cụ thể:&#x20;

```cpp
int senInp[5];
senInp[2] = 0;
```

{% hint style="danger" %}
Chú ý số đếm của mảng sẽ bắt đầu từ 0. Nói cách khác là số đầu tiên có vị trí là 0, số thứ hai có vị trí là 1,...&#x20;

```cpp
int senInp[5] = {1,1,0,0,1}; 
Serial.print(senInp[0]); // output: 1
Serial.print(senInp[2]); // output: 0
```
{% endhint %}

### Truy cập mảng

Để truy cập mảng, bạn chỉ cần đưa ra tên mảng cùng với vị trí cần truy cập, và từ đó bạn cũng có thể đọc giá trị hoặc thay đổi nó.

```cpp
int senInp[5] = {1,1,0,0,1}; // tạo mảng. Chú ý giá trị ở vị trí 2 lúc này là 0
Serial.print(senInp[0]); //output: 1
senInp[2] = 1;         // thay đổi giá trị mảng senInp ở vị trí 2 với giá trị 1.
Serial.print(senInp[2]); // output: 1 thay vì 0
```

