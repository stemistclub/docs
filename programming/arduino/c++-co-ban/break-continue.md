# Break / Continue

## Định nghĩa

### Break

Như các bạn có thể đã gặp từ khoá `break` ở bài [switch.md](switch.md "mention"), từ khoá `break` ở đây có tác dụng thoát khỏi một hàm điều kiện.&#x20;

Cụ thể hơn, chúng ta hãy xem lại ví dụ trong bài [switch.md](switch.md "mention"):&#x20;

```cpp
switch (case label) {
    case case1:
    // nội dung 1
    break;
    case case2:
    // nội dung 2
    break;
    case case3:
    // nội dung 3
    break;
    case default:
    // nội dung mặc định
    break;
}
```

Trong ví dụ trên khi nội dung của một **case** đã thực thi, lúc này khi gặp từ khoá `break` hàm switch sẽ thoát ra ngay lập tức và tiếp tục làm việc.

Ngoài ra `break` có thể giúp chúng ta thoát khỏi một **vòng lặp**.&#x20;

Ở ví dụ dưới đây **vòng lặp for** sẽ kết thúc khi `i` chạy đến 4:

```cpp
for (int i = 0; i < 10; i++) {
  if (i == 4) {
    break;
  }
  Serial.print(i); //output: 4
} 
```

### Continue

Từ khoá `continue` có tác dụng bỏ qua một lượt chạy đó nhưng vẫn tiếp tục vòng lặp.

Ở ví dụ dưới đây **vòng lặp for** khi giá trị i bằng 4 thì sẽ bỏ qua lượt chạy đó nhưng vòng lặp vẫn tiếp tục dẫn đến kết quả :

```
for (int i = 0; i < 10; i++) {
  if (i == 4) {
    continue;
  }
  Serial.print(i);
} 
```

Output:

```
012356789
```
