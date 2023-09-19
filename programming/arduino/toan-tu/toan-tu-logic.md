# Toán tử logic

Giống với toán tử so sánh, toán tử logic là toàn tử sẽ trả về giá trị kiểu Boolean. Nhưng toán tử logic là loại toán tử dùng để xử lí trạng thái của các điều kiện con hay điều kiện logic.

Trong ví dụ sau, chương trình sẽ trả về `0` (False) nếu cả 2 điều kiện ở dưới không thoả mãn, và trả về `1` (True) nếu chỉ 1 trong 2 điều kiện bất kỳ thoả mãn:&#x20;

<pre class="language-cpp"><code class="lang-cpp">int x = 5;
int y = 3;
<strong>bool result x > 3 || x &#x3C; 4; // True vì x > 3. 
</strong></code></pre>

Sau đây là các toán tử logic thường dùng:

<table><thead><tr><th width="162" align="center">Toán tử</th><th width="108" align="center">Tên</th><th width="170" align="center">Biểu thức</th><th align="center">Ý nghĩa</th></tr></thead><tbody><tr><td align="center">&#x26;&#x26;</td><td align="center">AND</td><td align="center">X &#x26;&#x26; Y</td><td align="center">true nếu cả X và Y đều đúng</td></tr><tr><td align="center">||</td><td align="center">OR</td><td align="center">X || Y</td><td align="center">true nếu ít nhất một trong hai vế X hoặc Y đúng</td></tr><tr><td align="center">!</td><td align="center">NOT</td><td align="center">! X</td><td align="center">true nếu X sai và false nếu X đúng</td></tr></tbody></table>
