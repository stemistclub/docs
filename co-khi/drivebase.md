# DRIVEBASE

## **A. Thế nào là Drivebase**

* Như các bạn đã biết, để một con robot di chuyển được chúng ta cần một bộ phận chứa những động cơ gắn bánh với chức năng di chuyển. Vì vậy DriveBase được coi là nền tảng của mọi con bot.
* Không chỉ thế, tất cả các bộ phận khác của một con bot đều gắn với drivebase nên nó cũng chính là thành phần quan trọng nhất của một con bot hoàn thiện.
* Drivebase thường có dạng một khung hình vuông hoặc hình chữ nhật được ghép bởi các thanh nhôm định hình và có những thiết kế đặc thù cho từng loại drivebase khác nhau.

<figure><img src="https://lh5.googleusercontent.com/6KE7kZ2hDDqJ2NI4OBnPKlP-FcrUy7InNP9XkAMmuP1ffxp8P-OUo2f1v3zFYub6YLHSdoDpOXwZtgBukwlZMCqL1CWUz9jDq_1Me_-g_AJezSV49aiu2OlvqUATJYguHBrmjhYgXs7eNK7Eti-qg3o" alt=""><figcaption><p><mark style="color:blue;">1.1, Type of Drivebase: Tank</mark></p></figcaption></figure>

{% embed url="https://www.youtube.com/watch?v=FLnUZBHBczM" %}
<mark style="color:blue;">1.2, Type of Drivebase: Swerve</mark>
{% endembed %}

<figure><img src="https://lh5.googleusercontent.com/fpUC2_P06URBkpDqH7Y3-kkhRTolEN7FkyLkLUfsPrMGbgEtddoIbBQhcj2FW4_4TQ_fChZNNPQ-qBTk3MrnEH7TUiERW3vaMs7-OIqX_IOetgdT0NGlOSLHRn6YSeVFCFFib2N97fDxwZ-fouhgRCs" alt=""><figcaption><p><mark style="color:blue;">1.3, Type of Drivebase: VRC Drivebase</mark></p></figcaption></figure>

### **B. Một số loại Drivebase phổ biến**&#x20;

1. **VRC Drivebase**&#x20;

* Đây là một loại drivebase khá phổ biến ở các giải thi đấu ở Việt Nam.
* Bao gồm: 2 bánh phay nhôm, 2 bánh đa hướng và 2 động cơ 300 (VRC)&#x20;
* Nguyên lý hoạt động: Động cơ dẫn động thẳng vào bánh phay nhôm và đây là dẫn động chính của loại drivebase này. Hai bánh đa hướng có vai trò điều hướng&#x20;
* Điểm mạnh: Dễ thực hiện lắp ráp, linh kiện đơn giản
* Điểm yếu: Di chuyển đa hướng khó linh hoạt, bị trơn trượt trên sàn
*

    <figure><img src="https://lh5.googleusercontent.com/fpUC2_P06URBkpDqH7Y3-kkhRTolEN7FkyLkLUfsPrMGbgEtddoIbBQhcj2FW4_4TQ_fChZNNPQ-qBTk3MrnEH7TUiERW3vaMs7-OIqX_IOetgdT0NGlOSLHRn6YSeVFCFFib2N97fDxwZ-fouhgRCs" alt=""><figcaption><p><mark style="color:blue;"><strong>II.1, Type of Drivebase: VRC Drivebase</strong></mark></p></figcaption></figure>

2. **Drivebase Tank**

* Còn đây là loại drivebase dành cho các đội mới của các giải robotics quốc tế (FGC, FRC, FTC, …)
* Bao gồm: 4 bánh phay nhôm, 2 động cơ DC, nhông xích
* Nguyên lý hoạt động: Động cơ gắn với trục dẫn động trực tiếp vào bánh xe ở cuối bot và truyền động qua xích đến bánh xe ở đầu. Hai bên bánh xe chạy riêng biệt nhau
* Điểm mạnh: Ma sát tốt nên khả năng bám trên mặt đường tốt, có thể rẽ được sang các hướng khác nhau. Truyền động bằng xích nên khá chắc chắn, đảm bảo tốc độ các bánh bằng nhau.
* Điểm yếu: Việc di chuyển đa hướng vẫn có một số bất tiện, chưa được linh hoạt.

3. **Drivebase Mecanum**

* Bao gồm: 4 bánh mecanum, 4 động cơ DC
* Nguyên lý hoạt động: Loại drivebase này hữu dụng hơn loại trên về mặt di chuyển trên mặt đất, tuy chỉ có 4 bánh mecanum nhưng loại này vô cùng linh hoạt trong việc di chuyển đa hướng (đi ngang, đi chéo mọi hướng). Hộp số được lắp đặt trực tiếp vào 4 bánh, mỗi hộp số 1 motor.
* Điểm mạnh: Di chuyển đa hướng dễ dàng, không gặp khó khăn khi phải chuyển hướng trong diện tích hẹp. Di chuyển trơn tru, ma sát ít.
* Điểm yếu: Bot không có độ bám quá tốt. Tốn động cơ&#x20;

<figure><img src="https://lh6.googleusercontent.com/-fL9vBIOLtatebwsy_wdiMsMdEJ6etkuLJuWydYy3bXYYAkzKS16BksTYWJrNH0c_iwUt4Tyjr51sgf0y_IPwIw453baPOPpUkHnYgT88Y4iPll0zudkTZb-Fp5_SqL5FPjRYahOyGMA_uqal52i7VE" alt=""><figcaption></figcaption></figure>

\


4. **Drivebase X**

* Bao gồm 4 bánh omi và 4 động cơ
* Nguyên lý hoạt động: X-Drive là một hệ thống truyền động dựa trên bánh xe omni holonomic. Loại truyền động này bao gồm việc lắp đặt 4 bánh xe omni ở góc của robot với góc 45 độ.
* Điểm mạnh: Khả năng quay và tăng tốc tốt, di chuyển nhanh
*   Điểm yếu: Hệ thống truyền động nên chiếm nhiều không gian

    <figure><img src="https://lh3.googleusercontent.com/7oJr8Jd617pmfF_X-s8P16WybLPay5MDeSQnl4rIDGDvskg5kjAQOQ6iNYA54bd6f0A9dQrAgEScCtHFZqB-TJUPPJ8pq7z9mX72r00fUwltsHtoYyVhKodfkdLAjo3vdI6Wj5S57CBoqKH0B0YTSZk" alt=""><figcaption></figcaption></figure>
