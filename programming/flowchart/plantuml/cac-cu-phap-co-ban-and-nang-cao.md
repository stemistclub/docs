# Các cú pháp cơ bản & nâng cao

## 1. Các cú pháp cơ bản

### a) Câu trúc đơn giản

Mỗi flowchart trong PlantUML bắt đầu và kết thúc bằng các từ khóa **`@startuml`** và **`@enduml`**.

```plant-uml
@startuml
start
:Action 1;
:Action 2;
stop
@enduml
```

* **`start`**: Ký hiệu bắt đầu quy trình.
* **`:Action;`**: Mỗi bước trong quy trình được biểu diễn bằng ký tự `:` theo sau là mô tả hành động. Ký hiệu này tạo ra một hình chữ nhật trong Flowchart.
* **`stop`**: Ký hiệu kết thúc quy trình.

### b) Ký hiệu điều kiện (Decision)

Ký hiệu điều kiện trong Flowchart được biểu diễn bằng hình thoi, dùng để tạo các nhánh quyết định.

```plant-uml
@startuml
start
:Check Condition;
if (Condition?) then (Yes)
  :Action if Yes;
else (No)
  :Action if No;
endif
stop
@enduml
```

* **`if (Condition?) then (Yes)`**: Tạo một nhánh quyết định với câu hỏi điều kiện.
* **`else (No)`**: Định nghĩa nhánh khác nếu điều kiện không thỏa mãn.
* **`endif`**: Kết thúc khối điều kiện.

### c) Vòng lặp (Loop)

Vòng lặp có thể được tạo bằng cách sử dụng các khối **`repeat ... repeat while`** hoặc **`while ... endwhile`**.

```plant-uml
@startuml
start
repeat
  :Action in Loop;
repeat while (Condition?)
:Continue;
stop
@enduml
```

* **`repeat ... repeat while`**: Tạo một vòng lặp kiểm tra điều kiện ở cuối.
* **`while (Condition?)`**: Tạo một vòng lặp kiểm tra điều kiện ở đầu.
* **`endwhile`**: Kết thúc khối vòng lặp **`while`**.

## 2. Các cú pháp nâng cao

### a) Ký hiệu đầu vào/ra (Input/Ouput)

Hình bình hành biểu diễn thao tác nhập hoặc xuất dữ liệu.

```plant-uml
@startuml
start
:Input data;
:Process data;
:Output result;
stop
@enduml
```

**`:Input data;`** và **`:Output result;`**: Ký hiệu này tạo ra hình hình bình hành để biểu diễn các thao tác nhập và xuất dữ liệu.

### b) Hình thoi với điều kiện phức tạp

Ta có thể sử dụng các biểu thức điều kiện phức tạp để mô tả các quyết định phức tạp hơn.

```plant-uml
@startuml
start
if (Condition A?) then (Yes)
  if (Sub-Condition 1?) then (True)
    :Sub-Action 1;
  else (False)
    :Sub-Action 2;
  endif
else (No)
  :Action B;
endif
stop
@enduml
```

**Điều kiện lồng nhau**: Cho phép chúng ta xây dựng các quyết định phức tạp với nhiều nhánh con bên trong.

### c) Chia quy trình thành các giai đoạn khác nhau (Different Phases)

Ta có thể chia quy trình thành các giai đoạn khác nhau sử dụng ký hiệu **`partition`**.

```plant-uml
@startuml
partition "Phase 1" {
  :Step 1;
  :Step 2;
}
partition "Phase 2" {
  :Step 3;
  :Step 4;
}
@enduml
```

**`partition "Phase Name"`**: Phân chia Flowchart thành các phần khác nhau theo giai đoạn.

### d) Ghi chú và chú thích (Notes or Comments)

Chúng ta nên thêm ghi chú vào Flowchart để giải thích hoặc thêm thông tin chi tiết.

```plant-uml
@startuml
start
:Action 1;
note right
  This is a note for Action 1
end note
:Action 2;
note left
  This is another note for Action 2
end note
stop
@enduml
```

**`note left`** và **`note right`**: Thêm ghi chú vào bên trái hoặc phải của một bước.

### e) Các ký hiệu khác của mũi tên và nét đoạn thẳng

Ta có thể tùy chỉnh hướng của mũi tên và kiểu đường nét giữa các bước trong Flowchart.

```plant-uml
@startuml
start
:Action 1;
-> :Step 1;        // Mũi tên đơn
--> :Step 2;       // Mũi tên nét đứt
- :Step 3;         // Đường nét không mũi tên
stop
@enduml
```

* **`->`**: Mũi tên đơn.
* **`-->`**: Mũi tên nét đứt.
* **`-`**: Đường nét không mũi tên.

### f) Kết hợp nhiều ký hiệu và điều kiện

```plant-uml
@startuml
start
partition "User Input" {
  :Input Username;
  :Input Password;
}
partition "System Processing" {
  :Verify Credentials;
  if (Valid?) then (Yes)
    :Grant Access;
  else (No)
    :Deny Access;
  endif
}
stop
@enduml
```
