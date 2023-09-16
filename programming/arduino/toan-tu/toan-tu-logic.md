# Toán tử logic

Với toán tử nó sẽ trả về giá trị true (1) và false (0)

{% hint style="info" %}
Thường được sử dụng trong câu điều kiện if else
{% endhint %}

>

Sau đây là tổng quan:&#x20;

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Tổng quan. Cre by w3school.com</p></figcaption></figure>



* Toán tử Logic && (toán tử và ): đây là toán tử giúp thực hiện động thời 2 nhiệm vụ

```cpp
// sử dụng để làm điều kiện
x > 5 && x < 10
// Khi nhập giá trị vào nếu x thuộc {6,7,8,9} thì sẽ return True
// Khi giá trị nằm ngoài khoảng đó thì return false
int x; cin >> x;
if(x > 5 && x < 10){ // nếu x thoả mãn đồng thời 2 điều kiện thì in ra x
    cout << x;
}
```

* Toán tử Logic || (toán tử hoặc): thay vì thoả mãn cả 2 điều kiện thì nếu x mà thoả mãn 1 trong 2 thì đều đc chấp nhận

```cpp
int x; cin >> x;
if (x > 5 || x < 3){ // nếu x > 5 hoặc x < 3 thì điều kiện thoả mãn vd: 10 hoặc 1
    cout << x;
}
```

* Toán tử Logic !(toán tử ngược hoặc khác): để sử dụng trong các trường hợp kết quả mong muốn phải khác.

```cpp
// 
int i = 8;
if (i != 9) cout << i; // kiểm tra nếu i khác 9 thì sẽ in ra. ở đây 8 khác 9 nên sẽ đc in
```

{% hint style="info" %}
Khi sử dụng ! đồng nghĩa với việc giá trị false thì mới chạy
{% endhint %}
