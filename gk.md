# Phần 1 Phần lý thuyết
<details>
  <summary><code><img width="1158" height="101" alt="image" src="https://github.com/user-attachments/assets/2b339f56-52d6-4559-8a92-93231b1255f3" />
</code></summary>

- Để giải quyết một bài toán trên máy tính điện tử ta phải thực hiện một số bước, trong đó có một
bước quan trọng là tìm ra giải thuật.
- Giải thuật (còn gọi là thuật toán) là một hệ thống chặt chẽ và rõ ràng các quy tắc nhằm xác định
một dãy các thao tác trên những đối tượng, sao cho sau một số bước hữu hạn thực hiện các thao
tác đó ta thu được kết quả mong muốn.
- Nhưng giải thuật chỉ phản ánh các phép xử lý, còn đối tượng để xử lý trên máy tính điện tử chính
là dữ liệu (data), chúng biểu diễn các thông tin cần thiết cho bài toán như: các dữ liệu vào, các kết
quả trung gian, các dữ liệu ra... .
- Không thể nói tới giải thuật mà không nghĩ tới giải thuật đó được tác động trên dữ liệu nào. Còn
khi xét tới dữ liệu thì cũng phải hiểu dữ liệu ấy cần được tác động bởi giải thuật gì để đưa tới kết
quả mong muốn.
- Với một cấu trúc dữ liệu đã chọn ta sẽ có giải thuật xử lý tương ứng. Cấu trúc dữ liệu thay đổi thì
giải thuật cũng thay đổi theo.
- Bản thân các phần tử của dữ liệu thường có mối quan hệ với nhau, ngoài ra nếu biết tổ chức
chúng theo các cấu trúc dữ liệu thích hợp thì việc thực hiện các phép xử lý trên các dữ liệu sẽ
càng thuận lợi hơn, đạt hiệu quả cao hơn.
- Như vậy, giữa cấu trúc dữ liệu và giải thuật có mối quan hệ mật thiết. Có thể coi chúng như hình
với bóng, không thể nói tới cái này mà không nhắc tới cái kia.
- Chính điều đó đã dẫn tới việc, cần nghiên cứu các cấu trúc dữ liệu (data structures) đi đôi với việc
xác lập các giải thuật xử lý trên các cấu trúc ấy.
VD:
- Giả sử ta có một danh sách các trường đại học trên cả nước (danh sách chưa được sắp xếp). Ta
cần viết một chương trình tìm kiếm theo tên trường.
- Một cách đơn giản là cứ duyệt tuần tự các Tên trường trong danh sách cho tới khi tìm thấy (tìm
kiếm tuần tự). Cách tìm kiếm tuần tự này rõ ràng chỉ chấp nhận được khi danh sách ngắn, còn
danh sách dài thì rất mất thời gian. Thời gian tìm kiếm được đánh giá trong trường hợp này là
O(n), với n là số trường đại học (n là độ lớn dữ liệu vào).
- Nếu ta biết tổ chức lại danh sách bằng cách sắp xếp theo thứ tự từ điển của Tên trường, thì có thể
áp dụng một giải thuật tìm kiếm khác tốt hơn, tương tự như ta vẫn thường làm khi tra từ điển (còn
gọi là Tìm kiếm nhị phân). Tìm kiếm nhị phân có thời gian tìm kiếm được đánh giá là O(Log2n).
- Rõ ràng Tìm kiếm nhị phân nhanh hơn rất nhiều Tìm kiếm tuần tự, nhưng không thể áp dụng
được với dữ liệu chưa được sắp xếp. 
</details>




<details>
  <summary><code><img width="1160" height="103" alt="image" src="https://github.com/user-attachments/assets/5a052e04-7c80-40aa-9d23-5524c61bfbe4" />
</code></summary>

- Đối với các bài toán phi số, đi đôi với các cấu trúc dữ liệu mới cũng xuất hiện các phép toán mới
tác động trên các cấu trúc ấy. Thông thường có các phép toán như: Phép tạo lập hoặc huỷ bỏ một
cấu trúc, phép truy nhập vào từng phần tử của cấu trúc, phép bổ sung hoặc loại bỏ một phần tử
trên cấu trúc ...
- Các phép toán đó sẽ có những tác dụng khác nhau đối với từng cấu trúc. Có phép toán hữu hiệu
đối với cấu trúc này nhưng lại tỏ ra không hữu hiệu trên các cấu trúc khác.
- Vì vậy, khi chọn một cấu trúc dữ liệu ta phải nghĩ ngay tới các phép toán tác động trên cấu trúc
ấy. Và ngược lại, nói tới phép toán thì lại phải chú ý tới phép đó được tác động trên cấu trúc dữ
liệu nào. Cho nên người ta thường quan niệm: nói tới cấu trúc dữ liệu là bao hàm luôn cả phép
toán tác động trên các cấu trúc ấy.
</details>



<details>
  <summary><code><img width="1166" height="102" alt="image" src="https://github.com/user-attachments/assets/6c6757b2-1995-448b-b6a0-fa5336068506" />
</code></summary>

- Các cách biểu diễn một cấu trúc dữ liệu trong bộ nhớ máy tính điện tử được gọi là cấu trúc lưu trữ
(storage structures).
- Đó chính là cách cài đặt cấu trúc ấy trên máy tính điện tử, và trên cơ sở cấu trúc lưu trữ này mà
thực hiện các phép xử lý.
- Ta cần phân biệt giữa cấu trúc dữ liệu và cấu trúc lưu trữ tương ứng. Có thể có nhiều cấu trúc lưu
trữ khác nhau cho cùng một cấu trúc dữ liệu, cũng như có thể có những cấu trúc dữ liệu khác
nhau mà được thể hiện trong bộ nhớ bởi cùng một kiểu cấu trúc lưu trữ.
VD: Cấu trúc lưu trữ mảng và cấu trúc lưu trữ móc nối đều có thể được dùng để cài đặt cấu trúc
dữ liệu cây. Mặt khác, các cấu trúc dữ liệu như: danh sách, ngăn xếp và cây đều có thể cài đặt trên
máy thông qua cấu trúc lưu trữ móc nối.
</details>


<details>
  <summary><code><img width="1169" height="106" alt="image" src="https://github.com/user-attachments/assets/58536883-de2d-4856-95fe-734240e11cc1" />
</code></summary>

- Trong các ngôn ngữ lập trình bậc cao, các dữ liệu được phân thành các kiểu dữ liệu.
- Kiểu dữ liệu của một biến được xác định bởi một tập các giá trị mà biến đó có thể nhận và các
phép toán có thể thực hiện trên các giá trị đó.
- Ví dụ, kiểu dữ liệu “int” trong ngôn ngữ C có miền giá trị từ: -32768 đến 32767, các phép toán có
thể thực hiện trên các giá trị này là: các phép toán số học, các phép toán thao tác bit, các phép
toán logic và các phép toán so sánh.
Ví dụ:
- Ngôn ngữ C có các kiểu dữ liệu cơ bản sau:
- Các kiểu ký tự ( char, signed char, unsigned char )
- Các kiểu nguyên (int, unsigned int, long int, unsigned long int)
- Các kiểu thực (float, double, long double)
- Kiểu liệt kê (enum)
- Gọi là các kiểu dữ liệu cơ bản, vì các dữ liệu của các kiểu này sẽ được sử dụng như là các thành
phần cơ sở để kiến tạo nên các dữ liệu có cấu trúc phức tạp.
- Các kiểu dữ liệu đã cài đặt sẵn (build-in types) mà ngôn ngữ lập trình cung cấp thường không đủ
cho người sử dụng.
- Trong nhiều ứng dụng, người lập trình cần phải tiến hành các thao tác trên các dữ liệu phức hợp.
- Vì vậy, mỗi ngôn ngữ lập trình cung cấp cho người sử dụng một số quy tắc cú pháp để tạo ra các
kiểu dữ liệu mới từ các kiểu cơ bản hoặc các kiểu khác đã được xây dựng.
- Chẳng hạn, ngôn ngữ C cung cấp cho người lập trình các quy tắc để xác định các kiểu dữ liệu
mới như: kiểu mảng, kiểu cấu trúc (struct), kiểu móc nối, ...
- Các kiểu dữ liệu được tạo thành từ nhiều kiểu dữ liệu khác (các kiểu này có thể là kiểu cơ bản
hoặc kiểu dữ liệu đã được xây dựng) được gọi là kiểu dữ liệu có cấu trúc.
- Các dữ liệu thuộc kiểu dữ liệu có cấu trúc được gọi là các cấu trúc dữ liệu.
- Ví dụ, các mảng, các cấu trúc, các danh sách móc nối ... trong ngôn ngữ C, là các cấu trúc dữ
liệu.
- Từ các kiểu cơ bản, bằng cách sử dụng các qui tắc cú pháp để kiến tạo các kiểu dữ liệu, người lập
trình có thể xây dựng nên các kiểu dữ liệu mới thích hợp cho từng vấn đề.
- Các kiểu dữ liệu mà người lập trình xây dựng nên được gọi là các kiểu dữ liệu được xác định bởi
người sử dụng (user-defined data types).

- Như vậy, một cấu trúc dữ liệu là một dữ liệu phức hợp, gồm nhiều thành phần dữ liệu, mỗi thành
phần hoặc là dữ liệu cơ sở (số nguyên, số thực, ký tự,... ) hoặc là một cấu trúc dữ liệu đã được
xây dựng.
- Các thành phần dữ liệu tạo nên một cấu trúc dữ liệu được liên kết với nhau theo một cách nào đó.
- Trong các ngôn ngữ lập trình như: Pascal, C/C+ +, có ba phương pháp để liên kết các dữ liệu:
1. Liên kết các dữ liệu cùng kiểu tạo thành mảng dữ liệu.
2. Liên kết các dữ liệu (không nhất thiết cùng kiểu) tạo thành cấu trúc (struct) trong C/C+ +,
hoặc bản ghi (record) trong Pascal.
3. Sử dụng con trỏ để liên kết dữ liệu. Chẳng hạn, sử dụng con trỏ ta có thể tạo nên các danh
sách móc nối, hoặc sử dụng con trỏ để biểu diễn cây...

</details>



<details>
  <summary><code><img width="1118" height="51" alt="image" src="https://github.com/user-attachments/assets/4b8d08d9-cb3d-49ed-9e35-eba856ac16de" />
</code></summary>

- Với một bài toán, không phải chỉ có một giải thuật. Chọn một giải thuật để đưa tới kết quả nhanh là một đòi hỏi thực tế. Nhưng căn cứ vào đâu để có thể nói được giải thuật này nhanh hơn giải thuật kia?
- Có thể thấy ngay: thời gian thực hiện một giải thuật (hay chương trình thể hiện giải thuật đó) phụ thuộc vào rất nhiều yếu tố. Một yếu tố cần chú ý trước tiên đó là kích thước của dữ liệu đưa vào.
- Chẳng hạn thời gian sắp xếp một dãy số phải chịu ảnh hưởng của số lượng các số thuộc dãy số đó.
- Nếu gọi $n$ là số lượng này (kích thước của dữ liệu vào) thì thời gian thực hiện $T$ của một giải thuật phải được biểu diễn như một hàm của $n$: $T(n)$.
- Các kiểu lệnh và tốc độ xử lý của máy tính, ngôn ngữ viết chương trình và chương trình dịch ngôn ngữ ấy đều ảnh hưởng tới thời gian thực hiện, nhưng những yếu tố này không đồng đều với mọi loại máy trên đó cài đặt giải thuật, vì vậy không thể dựa vào chúng khi xác lập $T(n)$.
- Điều đó cũng có nghĩa là $T(n)$ không thể được biểu diễn thành đơn vị thời gian bằng giây, bằng phút... được.
- Tuy nhiên, không phải vì thế mà ta không thể so sánh được các giải thuật về mặt tốc độ.

  <img width="527" height="112" alt="image" src="https://github.com/user-attachments/assets/64fe09df-07ef-4175-8181-3bf53d49a184" />

- Nhận thấy, khi $n$ đủ lớn thì các hệ số $c$ và $k$ không còn ý nghĩa khi so sánh $T_1(n)$ và $T_2(n)$.
- Và như vậy thì nếu nói thời gian thực hiện giải thuật $T(n)$ tỉ lệ với $n^2$ hay tỉ lệ với $n$ cũng cho ta ý niệm về tốc độ thực hiện giải thuật đó khi n khá lớn (với $n$ nhỏ thì việc xét $T(n)$ không có ý nghĩa).
- Cách đánh giá thời gian thực hiện giải thuật độc lập với máy tính và các yếu tố liên quan tới máy như vậy sẽ dẫn tới khái niệm về **“cấp độ lớn của thời gian thực hiện giải thuật”** hay còn gọi là **“độ phức tạp tính toán của giải thuật”**.
- Nếu thời gian thực hiện một giải thuật là $T(n) = c \cdot n^2$ (với $c$ là hằng số) thì ta nói: độ phức tạp tính toán của giải thuật này có cấp là $n^2$ (hay cấp độ lớn của thời gian thực hiện giải thuật là $n^2$) và ta ký hiệu: $T(n) = O(n^2)$ *(ký hiệu chữ O lớn)*.

<br>

- Định nghĩa O lớn
- Một cách tổng quát có thể định nghĩa: Một hàm $f(n)$ được xác định là $O(g(n))$ và được gọi là có cấp $g(n)$ nếu tồn tại các hằng số $c$ và $n_0$ sao cho: 
  $$f(n) \le c \cdot g(n) \text{ khi } n \ge n_0$$
  nghĩa là $f(n)$ bị chặn trên bởi một hằng số $c$ nhân với $g(n)$, với mọi giá trị của $n$ từ một thời điểm $n_0$ nào đó.
- Thông thường ta chọn $g(n)$ là các hàm đơn giản để biểu diễn độ phức tạp tính toán của giải thuật như: $\log_2 n$, $n$, $n\log_2 n$, $n^2$, $n^3$, $2^n$, $n!$, $n^n$.
- Các hàm như $2^n$, $n!$, $n^n$ được gọi là **hàm loại mũ**. Một giải thuật mà thời gian thực hiện của nó có cấp là các hàm loại mũ thì tốc độ rất chậm.
- Các hàm như $\log_2 n$, $n$, $n\log_2 n$, $n^2$, $n^3$ được gọi là **hàm loại đa thức**. Giải thuật với thời gian thực hiện có cấp hàm đa thức thì thường chấp nhận được.


</details>


<details>
  <summary><code><img width="1178" height="146" alt="image" src="https://github.com/user-attachments/assets/0a39c54b-254f-4c7a-814f-37b090cb16bc" />
</code></summary>

- Xác định độ phức tạp tính toán của một giải thuật bất kỳ có thể dẫn tới những bài toán phức tạp. Tuy nhiên các kỹ thuật đưa ra trong mục này cho phép đánh giá được thời gian chạy của hầu hết các giải thuật mà ta gặp trong thực tế.

- **Quy tắc tổng**: Giả sử $T_1(n)$ và $T_2(n)$ là thời gian thực hiện của hai đoạn chương trình $P_1$ và $P_2$ mà $T_1(n) = O(f(n))$ và $T_2(n) = O(g(n))$, thì thời gian thực hiện $P_1$ rồi $P_2$ tiếp theo sẽ là: 
  $$T_1(n) + T_2(n) = O(\max(f(n), g(n)))$$
  *Ví dụ*: Trong một chương trình có 3 bước thực hiện mà thời gian thực hiện từng bước lần lượt là $O(n^2)$, $O(n^3)$ và $O(n\log_2 n)$ thì thời gian thực hiện 2 bước đầu là: $O(\max(n^2, n^3)) = O(n^3)$. Thời gian thực hiện cả chương trình sẽ là: $O(\max(n^3, n\log_2 n)) = O(n^3)$.

- Một ứng dụng khác của quy tắc này là nếu $g(n) \le f(n)$ với mọi $n \ge n_0$ thì $O(f(n) + g(n))$ cũng là $O(f(n))$. Chẳng hạn: $O(n^4 + n^2) = O(n^4)$ và $O(n + \log_2 n) = O(n)$.

- **Các câu lệnh lặp**: Gồm `for`, `while`, `do-while`.
- Để đánh giá thời gian thực hiện một câu lệnh lặp, trước hết ta cần đánh giá số tối đa các lần lặp, giả sử đó là $L(n)$.
- Sau đó đánh giá thời gian chạy của mỗi lần lặp. Chú ý rằng thời gian thực hiện `<phần thân>` của một lệnh lặp ở các lần lặp khác nhau có thể khác nhau, giả sử thời gian thực hiện `<phần thân>` lệnh lặp ở lần thứ $i$ ($i=1, 2, ..., L(n)$) là $T_i(n)$.
- Mỗi lần lặp, chúng ta cần kiểm tra `<điều kiện>` lặp, giả sử thời gian kiểm tra là $T_0(n)$. Như vậy thời gian chạy của lệnh lặp là tổng thời gian của các lần kiểm tra và thực thi thân vòng lặp.

  <img width="184" height="66" alt="image" src="https://github.com/user-attachments/assets/2765ae77-3a12-4014-85cc-02fe6fe00cc6" />

- Công đoạn khó nhất trong đánh giá thời gian chạy của một lệnh lặp là đánh giá số lần lặp.
- Trong nhiều lệnh lặp, đặc biệt là trong các lệnh lặp `for`, ta có thể thấy ngay số lần lặp tối đa là bao nhiêu.
- Nhưng cũng không ít các lệnh lặp, từ điều kiện lặp để suy ra số tối đa các lần lặp, ta cần phải tiến hành các suy diễn không đơn giản.
- **Trường hợp hay gặp**: Kiểm tra `<điều kiện>` lặp (thông thường là đánh giá một biểu thức) chỉ cần thời gian $O(1)$, thời gian thực hiện `<phần thân>` của các lần lặp là như nhau và giả sử ta đánh giá được là $O(f(n))$. Khi đó, nếu đánh giá được số lần lặp là $O(g(n))$, thì thời gian chạy của lệnh lặp là:
  $$O(g(n) \cdot f(n))$$

  *Ví dụ*: Giả sử ta có mảng $A$ các số thực cỡ $n$ và ta cần tìm xem trong mảng có chứa số thực $x$ không. Điều đó có thể thực hiện bởi giải thuật tìm kiếm tuần tự như sau:
  ```c
  (1) i = 0;
  (2) while (i < n && x != A[i])
  (3)     i++;
  ```
  Lệnh gán (1) có thời gian chạy là $O(1)$. Lệnh lặp (2)-(3) có số tối đa các lần lặp là $n$ (đó là trường hợp $x$ chỉ xuất hiện ở thành phần cuối cùng của mảng $A[n-1]$ hoặc $x$ không có trong mảng). Thân của lệnh lặp là lệnh (3) có thời gian chạy $O(1)$. Do đó, lệnh lặp có thời gian chạy là $O(n)$. Giải thuật gồm lệnh gán và lệnh lặp với thời gian là $O(1)$ và $O(n)$, nên tổng thời gian chạy của nó là $O(n)$.

- **Phép toán tích cực**: Dựa vào quy tắc tổng khi đánh giá thời gian thực hiện giải thuật, ta chỉ cần chú ý tới các bước tương ứng với một phép toán mà ta gọi là **phép toán tích cực** (*active operation*). Đó là phép toán thuộc giải thuật mà thời gian thực hiện nó không ít hơn thời gian thực hiện các phép khác, hay nói một cách khác: số lần thực hiện nó không kém gì các phép khác.
- Có những giải thuật có thể có nhiều hơn một phép toán tích cực.

<img width="790" height="279" alt="image" src="https://github.com/user-attachments/assets/7879a692-d5a7-46f7-8466-2adfb8925870" />


</details>


<details>
  <summary><code><img width="1186" height="114" alt="image" src="https://github.com/user-attachments/assets/d6e00437-8dbf-49aa-aec1-7208c9fd2d50" />
</code></summary>

Ý tưởng chung của phương pháp chia để trị là:
- Chia vấn đề cần giải thành một số vấn đề con cùng dạng với vấn đề đã cho,
chỉ khác là cỡ của chúng nhỏ hơn.
- Mỗi vấn đề con được giải quyết độc lập. Sau đó, ta kết hợp nghiệm của các
vấn đề con để nhận được nghiệm của vấn đề đã cho.
- Nếu vấn đề con là đủ nhỏ có thể dễ dàng tính được nghiệm, thì ta giải quyết
nó, nếu không thì vấn đề con được giải quyết bằng cách áp dụng đệ quy thủ tục trên
(tức là lại tiếp tục chia nó thành các vấn đề con nhỏ hơn,…). Do đó, các giải thuật
được thiết kế bằng phương pháp chia để trị sẽ là các giải thuật đệ quy.

<br>

Hàm mô tả ý tưởng của phương pháp chia để trị:

```c
DivideConquer (A, x) // tìm nghiệm x của bài toán A
{
    if (A đủ nhỏ)
        Solve (A);
    else
    {
        Chia bài toán A thành các bài toán con: A1, A2, …, Am;
        for (i = 1; i <= m; i++)
            DivideConquer (Ai, xi);
            
        Kết hợp các nghiệm xi của các bài toán con Ai (i = 1, …, m) 
        để nhận được nghiệm x của bài toán A;
    }
}
```
</details>



<details>
  <summary><code><img width="1199" height="160" alt="image" src="https://github.com/user-attachments/assets/6ebbaaee-7ef2-40be-ad8c-42e8cb83ac28" />
</code></summary>

- Phương pháp quy hoạch động:

  - Phương pháp quy hoạch động giải quyết bài toán bằng cách chia nó thành các bài toán con.
  - Tính nghiệm của các bài toán con từ quy mô nhỏ nhất đến lớn nhất.
  - Ghi lại các kết quả đã tính được vào một bảng lưu trữ (thường là mảng một hoặc hai chiều).
  - Khi tính nghiệm của bài toán lớn hơn, thuật toán chỉ việc tra cứu lại các kết quả trong bảng mà không cần phải tính toán lại nhiều lần.

- Áp dụng giải bài toán “Sắp xếp các đồ vật vào ba lô”
  - <img width="487" height="934" alt="image" src="https://github.com/user-attachments/assets/e28ca581-abd9-4390-8ffc-951b6740520d" />

  - <img width="479" height="378" alt="image" src="https://github.com/user-attachments/assets/bf275336-c48c-4670-aa24-8e5cd1d63e90" />

  - <img width="496" height="546" alt="image" src="https://github.com/user-attachments/assets/3654e86c-12a8-493a-8241-2464b29dbbf8" />


</details>



<details>
  <summary><code><img width="1077" height="73" alt="image" src="https://github.com/user-attachments/assets/37b9e308-def8-49aa-9c22-577523935668" />
</code></summary>

```c
Backtrack(j) // Tìm thành phần thứ j của vector nghiệm
{
    for (mỗi xj ∈ Aj)
    {
        if (xj thoả mãn các mối quan hệ ràng buộc với các thành phần đã chọn)
        {
            Lưu lại tình trạng khi chọn xj;
            if (tìm được một nghiệm mới)
                In nghiệm;
            else
                Backtrack(j + 1);
            Phục hồi lại tình trạng trước khi chọn xj; // thể hiện sự quay lui
        }
    }
}
```
</details>


<details>
  <summary><code><img width="1141" height="76" alt="image" src="https://github.com/user-attachments/assets/1d257353-9cd0-4959-a89c-fddde5ebb4ae" />
</code></summary>

Hàm mô tả ý tưởng phương pháp nhánh cận được viết như sau:

```c
Branch_Bound(j) // Tìm thành phần thứ j của vector nghiệm
{
    for (mỗi xj ∈ Aj)
    {
        Lưu lại tình trạng khi xét xj;
        if (đã tìm được một nghiệm mới)
        {
            if (giá trị của nghiệm mới tốt hơn nghiệm tối ưu)
                Chọn nghiệm mới này làm nghiệm tối ưu;
        }
        else
        {
            if (giá trị cận f(x1, x2, ..., xj) tốt hơn giá trị của nghiệm tối ưu)
                Branch_Bound(j + 1); // gọi đệ quy để tìm xj+1
        }
        Phục hồi lại tình trạng trước khi xét xj; // thể hiện sự quay lui
    }
}
```
</details>


---
<br>

# Phần 2 Phần bài tập
<details>
  <summary><code><img width="1000" height="455" alt="image" src="https://github.com/user-attachments/assets/95e1a1d5-0e13-4225-bb8e-9d2272f453fd" /></code></summary></code></summary>

  <br>
  
  Trước: A C G F B E I D H
 
  Giữa: G C F A I E B D H
  
  Sau: G F C I E H D B A
</details>

<details>
  <summary><code><img width="1209" height="147" alt="image" src="https://github.com/user-attachments/assets/7a9813d4-d304-4bfe-9f38-0e8ea785433a" />
</code></summary>

   <img width="1490" height="877" alt="image" src="https://github.com/user-attachments/assets/2d0199f3-03bc-4cfe-99c9-d95d77404040" />

</details>

<details>
  <summary><code><img width="1190" height="111" alt="image" src="https://github.com/user-attachments/assets/3155b537-50c2-4f0e-8186-a5c017e526b6" />
</code></summary>

  <img width="1302" height="817" alt="image" src="https://github.com/user-attachments/assets/75f852b9-15f0-4382-9370-2b22bb0c260a" />


</details>

<details>
  <summary><code><img width="532" height="193" alt="image" src="https://github.com/user-attachments/assets/103159c6-3957-4104-a189-f89185bbb962" />
</code></summary>

  <img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/b337e282-91f0-438b-92d2-b56dd404a460" />

</details>


<details>
  <summary><code><img width="1201" height="451" alt="image" src="https://github.com/user-attachments/assets/d7194505-0b01-4529-a65f-16f359127d55" />
</code></summary>

  <img width="1920" height="2560" alt="image" src="https://github.com/user-attachments/assets/e328f927-a842-4f0a-b26d-11597c676a8a" />



</details>


---

<br>


# Phần 3 Phần giải thuật

<details>
  <summary><code><img width="1152" height="299" alt="image" src="https://github.com/user-attachments/assets/fd34e9c3-860d-4e03-8f59-2902f5689764" />
</code></summary>

  ```c
  DOUBLE_IN (Pdau, Pcuoi, Q, X){
    P = malloc();
    P->DATA = X;
    P->P_R = P->P_L = NULL;
    if (Pcuoi == NULL){
      Pdau=Pcuoi=P;
    }
    else if (Q == Pdau){
      P->P_R = Q;
      Q->P_L = P;
      Pdau = P;
    }
    else {
      P->P_L = Q->P_L;
      P->P_R = Q;
      Q->P_L = P;
      P->P_L->P_R = P;
    }
  }
  ```

</details>



<details>
  <summary><code><img width="1182" height="295" alt="image" src="https://github.com/user-attachments/assets/42ae1128-319a-4817-bef2-30b51d48d027" />
</code></summary>

  ```c
  DOUBLE_DEL (Pdau, Pcuoi, Q){
    if (Pcuoi == NULL){
      printf(“Danh sách rỗng”);
    }
    else if (Pdau == Pcuoi){
      Pdau = Pcuoi = NULL;
    }
    else if (Q == Pdau){
      Pdau = Pdau→P_R;
      Pdau→P_L = NULL;
    }
    else if (Q == Pcuoi){
      Pcuoi = Pcuoi→P_L;
      Pcuoi→P_R = NULL;
    }
    else{
      Q→P_L→P_R = Q→P_R;
      Q→P_R→P_L = Q→P_L;
    }
    free(Q);
  }
  ```

</details>



<details>
  <summary><code><img width="1153" height="254" alt="image" src="https://github.com/user-attachments/assets/8cece176-415d-4bcb-97c6-92aa36ea439a" />
</code></summary>

  ```c
  ATTACH (H, M, D){
    T = malloc();
    T→HSO = H;
    T→MU = M;
    if (C == NULL){
      C = T;
    }
    else{
      D→NEXT = T;
    }
    D = T;
  }

  PADD(A, B, C){
    P = A;
    Q = B;
    C = NULL;
    while (P != NULL && Q != NULL){
      if (P→MU == Q→MU){
          H = P→HSO + Q→HSO;
          if (H != 0){
              ATTACH (H, P→MU, D);
              P = P→NEXT;
              Q = Q→NEXT;
          }
      }
      else if (P→MU > Q→MU){
          ATTACH (P→HSO, P→MU, D);
          P = P→NEXT;
      }
      else{
          ATTACH (Q→HSO, Q→MU, D);
          Q = Q→NEXT;
      }
    }
    if (Q == NULL){
        while (P != NULL){
            ATTACH (P→HSO, P→MU, D);
            P = P→NEXT;
        }
    }
    else{
        while (Q != NULL){
            ATTACH (Q→HSO, Q→MU, D);
            Q = Q→NEXT;
        }
    }
    D→NEXT = NULL;
  }
  ```
</details>



<details>
  <summary><code><img width="1170" height="212" alt="image" src="https://github.com/user-attachments/assets/68a21569-07b1-4858-8d4c-e2aad08163a3" />
</code></summary>

  - Ngôn ngữ tựa C:

    ```c
    PUSH (S, T, X){
        if (T >= n-1){
            printf(“Ngăn xếp tràn”);
        }
        else{
            T = T + 1;
            S[T] = X;
        }
    }

    POP (S, T){
        if (T < 0){
            printf(“Ngăn xếp cạn”);
        }
        else{
            T = T – 1;
            return S[T+1];
        }
    }

    DINH_GIA_BIEU_THUC (){
        do{
            Đọc phần tử X tiếp theo trong biểu thức;
            if (X là toán hạng){
                PUSH (S, T, X);
            }
            else{
                Y = POP (S, T);
                Z = POP (S, T);
                W = Z X Y;
                PUSH (S, T, W);
            }
        }while (chưa gặp dấu kết thúc biểu thức);
        R = POP (S, T);
        printf(R);
    ```

- Minh hoạ diễn biến của quá trình đọc biểu thức và sự thay đổi
trong STACK với biểu thức: 8 4 - 6 3 / +


<table width="100%">
  <thead>
    <tr>
      <th align="center" width="35%">Diễn biến đọc biểu thức</th>
      <th align="center" width="20%">Diễn biến STACK</th>
      <th align="center" width="45%">Thực hiện phép toán</th>
    </tr>
  </thead>
  <tbody>
    <!-- HÀNG 1 -->
    <tr>
      <td align="center"><span style="color: red;"><u>8</u> 4 &minus; 6 3 / +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">8</td></tr>
        </table>
      </td>
      <td align="left">Đẩy 8 vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 2 -->
    <tr>
      <td align="center"><span style="color: red;"><u>4</u> &minus; 6 3 / +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">4</td></tr>
          <tr><td width="30px" height="25px">8</td></tr>
        </table>
      </td>
      <td align="left">Đẩy 4 vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 3 -->
    <tr>
      <td align="center"><span style="color: red;"><u>&minus;</u> 6 3 / +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">4</td></tr>
        </table>
      </td>
      <td align="left">Lấy 4 và 8 ra khỏi ngăn xếp, thực hiện: 8 &minus; 4 rồi đẩy kết quả vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 4 -->
    <tr>
      <td align="center"><span style="color: red;"><u>6</u> 3 / +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">6</td></tr>
          <tr><td width="30px" height="25px">4</td></tr>
        </table>
      </td>
      <td align="left">Đẩy 6 vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 5 -->
    <tr>
      <td align="center"><span style="color: red;"><u>3</u> / +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">3</td></tr>
          <tr><td width="30px" height="25px">6</td></tr>
          <tr><td width="30px" height="25px">4</td></tr>
        </table>
      </td>
      <td align="left">Đẩy 3 vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 6 -->
    <tr>
      <td align="center"><span style="color: red;"><u>/</u> +</span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">2</td></tr>
          <tr><td width="30px" height="25px">4</td></tr>
        </table>
      </td>
      <td align="left">Lấy 3 và 6 ra khỏi ngăn xếp, thực hiện: 6 / 3 rồi đẩy kết quả vào ngăn xếp</td>
    </tr>
    <!-- HÀNG 7 -->
    <tr>
      <td align="center"><span style="color: red;"><u>+</u></span></td>
      <td align="center">
        <table border="1" style="border-collapse: collapse; text-align: center; margin: auto;">
          <tr><td width="30px" height="25px">6</td></tr>
        </table>
      </td>
      <td align="left">Lấy 2 và 4 ra khỏi ngăn xếp, thực hiện: 4 + 2 rồi đẩy kết quả vào ngăn xếp</td>
    </tr>
  </tbody>
</table>

</details>

</details>



<details>
  <summary><code></code><img width="1188" height="254" alt="image" src="https://github.com/user-attachments/assets/8ad569c1-f3e9-4ba2-bf17-20744edc8269" />
</summary>

  - Ngôn ngữ tựa C

```c
    PUSH (S, T, X)
{
    if (T >= n-1)
        printf(“Ngăn xếp tràn”);
    else
    {
        T = T + 1;
        S[T] = X;
    }
}

POP (S, T)
{
    if (T < 0)
        printf(“Ngăn xếp cạn”);
    else
    {
        T = T – 1;
        return S[T+1];
    }
}

TT_TRUOC_S (T)
{
    if (T == NULL)
    {
        printf(“Cây rỗng”);
        return;
    }
    else
    {
        TOP = -1;
        PUSH (S, TOP, T);
    }
    
    while (TOP > -1)
    {
        P = POP (S, TOP);
        while (P != NULL)
        {
            printf(P → DATA);
            if (P → P_R != NULL)
                PUSH(S, TOP, P → P_R);
            P = P → P_L;
        }
    }
}
```

</details>



<details>
  <summary><code></code><img width="1196" height="255" alt="image" src="https://github.com/user-attachments/assets/9870a90a-dea9-40c7-bfb9-7608380637c9" />
</summary>

- Ngôn ngữ tựa C

```c
PUSH (S, T, X)
{
    if (T >= n-1)
        printf(“Ngăn xếp tràn”);
    else
    {
        T = T + 1;
        S[T] = X;
    }
}

POP (S, T)
{
    if (T < 0)
        printf(“Ngăn xếp cạn”);
    else
    {
        T = T – 1;
        return S[T+1];
    }
}

TT_GIUA_S (T)
{
    if (T == NULL)
    {
        printf(“Cây rỗng”);
        return;
    }
    else
    {
        TOP = -1;
        P = T;
    }
    
    while ((P != NULL) || (TOP > -1))
    {
        while (P != NULL)
        {
            PUSH (S, TOP, P);
            P = P → P_L;
        }
        P = POP (S, TOP);
        printf(P → DATA);
        P = P → P_R;
    }
}
```

</details>



<details>
  <summary><code><img width="1177" height="131" alt="image" src="https://github.com/user-attachments/assets/bc42b71a-92e4-4c1f-9a03-7690cdefa820" />
</code></summary>

- Ngôn ngữ tựa C

```c
In_kqua(x)
{ // Hàm in ra một phương án vị trí các quân hậu (từ cột 1 đến cột 8)
    for (i = 1; i <= 8; i++) 
        printf(x[i]);
    
}

Dat_Hau(j)
{/* Hàm đệ quy quay lui tìm hàng i để đặt quân hậu tại cột j.
    Sử dụng các mảng đánh dấu tình trạng: a (hàng), b (đường chéo xuôi), c (đường chéo ngược)
    để kiểm tra xung khắc dữ liệu trước khi chấp nhận vị trí đặt. */

    for (i = 1; i <= 8; i++) 
    {
        if (a[i] && b[i+j] && c[i-j]) // Kiểm tra nếu hàng i và các đường chéo còn tự do
        {
            x[j] = i; // Ghi nhận lựa chọn đặt quân hậu j ở hàng i
            
            // Lưu lại tình trạng: đánh dấu hàng và các đường chéo đã bị chiếm
            a[i] = b[i+j] = c[i-j] = 0; 
            
            if (j == 8) 
                In_kqua(x); // Nếu đã đặt xong quân hậu ở cột 8 thì in kết quả
            else
                Dat_Hau(j+1); // Gọi đệ quy thử đặt quân hậu tiếp theo ở cột j+1
                
            // Phục hồi lại tình trạng ban đầu (Quay lui) để thử phương án khác
            a[i] = b[i+j] = c[i-j] = 1; 
        }
    }
}

main()
{
    // Khởi tạo trạng thái ban đầu: Tất cả các hàng và đường chéo đều tự do (bằng 1)
    for (i = 1; i <= 8; i++) a[i] = 1;
    for (i = 2; i <= 16; i++) b[i] = 1;
    for (i = -7; i <= 7; i++) c[i] = 1;
    
    Dat_Hau(1); // Bắt đầu tìm kiếm từ quân hậu đầu tiên ở cột 1
}
```

</details>
















---

<br>


<details>
  <summary><code></code></summary>
</details>



<details>
  <summary><code></code></summary>
</details>



<details>
  <summary><code></code></summary>
</details>
