# SHOOTER

## **A. Thế nào là Shooter**

* Đôi khi trong các cuộc thi robot, chúng ta sẽ có nhiệm vụ phải dịch chuyển các gamepiece từ một nơi thấp đến một nơi cao hơn. Khi đó chúng ta có các cách như: sử dụng cần cẩu, dùng ròng rọc, dùng băng truyền... Những cách này có thể áp dụng với hầu hết các vật thể. Nhưng khi vật thể có dạng cầu như các trái bóng, chúng ta có thể lựa chọn cách đó là sử dụng việc bắn. Cho dù là bắn tumlum hay bắn gongang, chúng ta đều cần một bộ phận rất đặc biệt, gọi là Shooter hay có thể gọi là Bộ bắn.
* Đây là video minh họa về các robot sử dụng Shooter&#x20;

{% embed url="https://www.youtube.com/watch?pp=ygUIZmdjIDIwMjI=&v=_v-kmPPhYeE" %}

{% embed url="https://www.youtube.com/watch?pp=ygUIZmdjIDIwMjI=&v=tHJYL7B_P1U" %}

## B.  Các cơ cấu Shooter  thường sử dụng

### 1.  Cơ cấu 1: Bắn bóng đà bằng 2 bánh đà xoay ngược chiều nhau

* **Nguyên lí hoạt động:** Hệ thống bắn này bao gồm một cặp bánh xe xoay ngược chiều nhau. Bất cứ khi nào bóng được dưa vào khoảng trống giữa hai bánh xe nó sẽ được tăng tốc bởi sự ma sát giữa hai bánh xe và trái bóng. Từ đó trái bóng sẽ được cung cấp một phần động lượng từ hai bánh đà đang quay và phóng lên không trung.
* **Ưu điểm:** Có tốc độ bắn bóng nhanh và mạnh, đường bóng bắn ra ổn định bóng không bị có độ xoáy quá lớn khi bị bắn ra bởi hai bánh đà, có thể điều chỉnh được hướng bóng bay ra bằng cách thay đổi tốc độ tương đối giữa hai bên bánh đà.
* **Nhược điểm:** Yêu cầu độ chính xác và sự ổn định về cơ khí phải cao, khoảng cách giữa hai bánh đà phải phù hợp với từng loại bóng khác nhau, hệ thống bắn to cồng kềnh, sự sai lệch về vị trí giữa hai trái bóng liên tiếp được bắn ra phụ thuộc vào vận tốc của bánh đà và cách trái bóng tiếp xúc với hai bánh đà như nào khi được đưa vào khoảng trống, cần nhiều năng lượng để vận hành.



<div data-full-width="true">

<figure><img src="../.gitbook/assets/2 bánh đà.PNG" alt=""><figcaption><p>Ảnh đơn giản về cơ chế bắn 2 bánh đà.</p></figcaption></figure>

</div>

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption><p>Ảnh thực thế bot dùng cơ chế bắn hai bánh đà.</p></figcaption></figure>



### 2. Cơ cấu 2: Bắn bóng bằng hệ thống một bánh đà.

* **Nguyên lý hoạt động:** Hệ thống bắn bóng này bao gồm một bánh đà ở trung tâm hoặc một loạt các bánh đà được xếp ở cùng một phía quay cùng chiều nhau với tốc độ rất cao, khi bóng được đưa vào khoảng trống giữa bánh xe đang quay và tường chắn động lượng từ bánh xe được truyền qua bóng bằng lực ma sát từ đó cung cấp cho bóng một vận tốc để bắn ra.
* **Ưu điểm:** Có cấu tạo đơn giản và dễ dàng hơn trong việc thiêt kế và gia công cơ khí hơn so với hệ thống bắn bằng hai bánh đà, cần ít năng lượng để vận hành hơn cơ cấu bắn bóng bằng hai bánh đà.
* **Nhược điểm:** Không đảm bảo tính ổn định trong vận hành vì cơ cấu một bánh đà không có khả năng tự điều chỉnh nên việc đảm bảo tính ổn định khó hơn khi so sánh với các cơ cấu bắn bóng khác, cơ cấu này không cho phép thay đổi góc bắn bóng một cách dễ dàng việc thay đổi góc bắn đỏi hỏi phải di chuyển toàn bộ cơ cấu.
* Hệ thống bắn 1 bánh đà cơ bản được FGC giới thiệu:

{% embed url="https://www.youtube.com/watch?v=An3xoJgk2uI" %}
FIRST Global: Hướng dẫn cơ chế bắn 1 bánh đà.
{% endembed %}

###

<figure><img src="../.gitbook/assets/1 bánh đà.PNG" alt=""><figcaption><p>Ảnh đơn giản cơ chế bắn 1 bánh đà</p></figcaption></figure>

### 3. Cơ cấu 3: Cơ cấu bắn bóng bằng sự đàn hồi của lò xo hoặc dây cao su.

* Nguyên lý hoạt động: Là phương pháp tạo ra sự đàn hồi trong các vật liệu như cao su, lò xo để tạo ra lực bật trở lại tận dụng lực đàn hồi trở lại đó của vật liệu để bắn bóng đi.
* Ưu điểm: Có cấu tạo đơn giản dễ dàng thiết kế lắp ráp và bảo trì, độ chính xác khi bắn cao, không bị ảnh hưởng bởi chất liệu làm nên quả bóng, bắn được nhiều loại bóng, tiêu tốn ít năng lượng.&#x20;
* Nhược điểm: Tốc độ bắn bóng ra chậm, không thay đổi được độ mạnh, yếu của bóng bắn ra làm giảm tính linh hoạt.

<figure><img src="../.gitbook/assets/đàn hồi của cao su.PNG" alt=""><figcaption></figcaption></figure>
