# Mảng và lòng lặp

## Vòng lặp trong mảng

Chúng ta có thể áp dụng vòng lặp vào trong mảng.

Trong ví dụ dưới đây sẽ hiển thị tất cả các giá trị bên trong mảng:

```cpp
int arrNum[5] = {3,5,2,6,2}
for (i = 0; i < 5; i++) {
    Serial.print(arrNum[i]);
}
```

Output:

```
35262
```

## Vòng lặp for-each:

Ngoài ra cũng có một loại vòng lặp được gọi là vòng lặp "for-each", được giới thiệu vào C++ version 11. Và được thiết kế để dành cho việc truy suất các giá trị bên trong mảng:&#x20;

```cpp
for (kiểu tên biến : tên mảng) {
  // nội dung.
}
```

Ví dụ dưới đây có tác dụng giống với ví dụ ở trên những sử dụng vòng lặp for-each:

```cpp
int arrNum[5] = {3,5,2,6,2}
for (int i : arrNum) {
    Serial.print(i);
}
```

