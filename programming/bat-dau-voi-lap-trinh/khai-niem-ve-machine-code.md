---
description: Phần này nếu bạn cảm thấy không có hứng thú thì hoàn toàn có thể bỏ qua
---

# Khái niệm về machine code

Đối với máy tính điện tử ngày nay đều sử dụng mã mãy hay machine code dưới dạng nhị phân (Binary), là dạng mà chỉ có 2 trạng thái là Bật hoặc Tắt (0 và 1), điều này bắt nguồn từ việc bản chất cấu tạo của một CPU (Bộ vi xử lí trung tâm) được tạo nên từ các bóng bán dẫn (Transitiors).

Chính vì vậy machine code không có nghĩa là mã nhị phân, lấy ví dụ là máy tính lượng tử - một dạng máy tính mà có thể biểu diễn nhiều hơn 2 trạng thái là 0 và 1. Đây là điều cần lưu ý, nó sẽ không giúp ích gì cho chúng ta trong việc lập trình, nhưng nếu sau này ai muốn theo khoa học máy tính, thì đây là thứ không được nhằm lẫn.&#x20;

## Mã máy hay machine code là gì ?

Mã máy là ngôn ngữ lập trình cấp thấp nhất mà máy tính có thể hiểu trực tiếp. Nó là một chuỗi các số nhị phân (0 và 1) đại diện cho các hướng dẫn (instructions) mà máy tính phải thực hiện.

Đây là một ví dụ của một dãy hướng dẫn bằng mã máy để thêm 2 số:&#x20;

```
0000 0000 0000 0010 0000 0000 1000 1000
```

Nhìn vào dãy hướng dẫn trên, nếu không đề cập trước rằng đây là dãy hướng dẫn để thêm 2 số thì không ai có thể hiểu được rằng dãy này dùng để làm gì hay nó thực hiện hành động gì, chính vì vậy mã máy cực kỳ khó để có thể hiểu và viết.&#x20;

## Phương thức lập trình

Do việc sử dụng mã máy để viết chương trình là rất khó nên mọi người thường sẽ sử dụng ngôn ngữ lập trình bậc cao hơn, với sự trợ giúp của trình biên dịch, hoặc trình thông dịch đối với ngôn ngữ bậc cao (high-level) để giúp chuyển ngôn ngữ mà con người có thể hiểu được (Python, C/C++,...) sang mã máy để máy có thể hiểu được.

Trong trang tiếp theo, chúng ta sẽ không đi sâu về cách chương trình hoạt động với mã máy bởi rằng nó không hữu ích trong việc chúng ta viết chương trình đơn giản mà ta sẽ phân biệt giữa ngôn ngữ lập trình bậc thấp sử dụng trình biên dịch (compiler) với ngôn ngữ bậc cao sử dụng trình thông dịch (interpreter).&#x20;
