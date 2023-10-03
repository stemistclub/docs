# Switch

## Định nghĩa

**Switch** so sánh một **biến (hoặc biểu thức)** với một giá trị. Mỗi giá trị đó là một **case label (nhãn trường hợp)** trong khối. Trong khối switch còn có thể có một **default label (nhãn mặc định)** có thể có hoặc không. Trong mỗi label còn chứa các khối code tương ứng.

<pre class="language-cpp"><code class="lang-cpp">switch (case label) {
    case case1:
    // nội dung 1
    break;
<strong>    case case2:
</strong>    // nội dung 2
    break;
    case case3:
    // nội dung 3
    break;
    case default:
    // nội dung mặc định
    break;
}
</code></pre>

Trong đó:

* **case label** sẽ là điều kiện được đưa ra tham chiếu.
* **case1,case2,...** là giá trị mà khi điều kiện được đưa ra tham chiếu đạt một giá trị của chúng.

Trong khối code switch còn có thể có một **default label (nhãn mặc định)** có thể có hoặc không. Trong mỗi label còn chứa các khối code tương ứng. Và khối **default label** này sẽ được thực thi khi không có một điều kiện tham chiếu nào trước đó thoả mãn. Đối với quy tắc tổng quát thì nội dung trong khối mặc định sẽ được thực thi khi **case label** không đạt bất cứ giá trị nào trong **case1,case2 và case3**.

{% hint style="info" %}
Trong ví dụ trên bạn thấy rằng có từ khoá `break;` được đặt sau mỗi trường hợp, điều này sẽ được đề cập ở bài [break-continue.md](break-continue.md "mention").
{% endhint %}
