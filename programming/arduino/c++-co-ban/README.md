# C++ cơ bản

Hướng dẫn này dành cho những ai chưa có một kiến thức về lập trình, hoặc là đối với C++.

## Tại sao lại cần có hướng dẫn này ở đầu.

Bởi vì trước khi các bạn bắt đầu với Arduino, bạn nên biết ngôn ngữ mà Arduino được chạy trên C++ nhưng được tối giản lại nhằm dễ tiếp cận hơn với người mới.

Khác với các hướng dẫn khác, khi bạn sẽ được viết thử các chương trình cho Arduino trước, sau đó bạn sẽ được giới thiệu dần về những nội dung căn bản của C++ như toán tử, kiểu dữ liệu,... Tài liệu này sẽ cho bạn biết về căn bản của C++ trước, sau khi học được các nội dung cơ bản của C++, bạn sẽ có tư duy về cách một chương trình hoạt động, ngoài ra khi đi sâu vào việc tương tác giữa thiết bị và chương trình, tài liệu sẽ không phải giới thiệu lại các căn bản như "Vì ta muốn dữ liệu được cập nhật liên tục nên ta sẽ sử dụng một vòng lặp. Và vì ta chỉ muốn điều đó xảy ra khi ta kích hoạt chế độ chỉ định nên ta sẽ sử dụng vòng lặp while."&#x20;

{% hint style="warning" %}
Việc bố trí tài liệu theo hướng này được đánh giá là không thân thiện đối với người mới. Nhưng một khi bạn đã hiểu về lập trình, tài liệu này sẽ rất có ích với bạn bởi mọi thứ sẽ rất rõ ràng, không phải tìm hiểu hàm này thông qua một ứng dụng cụ thể...
{% endhint %}

{% hint style="danger" %}
Hướng dẫn trong phần này hướng đến các hàm cốt lõi trong C++ và ứng dụng nó vào lập trình Arduino.

Khác với các hướng dẫn lập trình C++ khi bạn sẽ được biết đến các hàm về đầu vào / đầu ra phổ biến như `cout`, `cin`,... Tài liệu này sẽ chỉ hướng chung là cốt lõi của C++ bởi bản thân các hàm như `cout`,`cin` đều nằm trong thư viện của Standart Input / Output.&#x20;

Trong Arduino có cách giao tiếp có thể coi là "tương tự" CLI đó là Serial, trong phần riêng về Serial bạn sẽ biết rõ hơn về cách giao tiếp Serial.

Trong hướng dẫn này sẽ chứa hàm `Serial.println();` hiện tại bạn chỉ cần biết rằng nội dung của hàm này là sẽ hiển thị ra màn hình Serial. Cụ thể hơn sẽ được nói trong bài Serial.
{% endhint %}

{% hint style="info" %}
Nếu bạn cảm thấy khó khăn mà vẫn muốn học theo cách bố trí trong tài liệu này, bạn chỉ cần đọc đến [ham-dieu-kien](ham-dieu-kien/ "mention"), và sau đó bạn có thể chuyển sang [arduino-co-ban](../arduino-co-ban/ "mention"). Khi bạn đã thuần thục việc sử dụng các hàm cơ bản đã được học trước đó, bạn có thể chuyển qua phần tiếp theo trong [.](./ "mention") như [switch.md](switch.md "mention").
{% endhint %}

{% hint style="info" %}
Nếu bạn thấy phần này khó nhớ, hãy coi đây như là một "từ điển" mà bạn có thể quay lại và tra cứu bất cứ lúc nào. Theo thời gian khi bạn đã thuần thục với chúng thì bạn gần như sẽ không bao giờ phải quay lại phần này.
{% endhint %}
