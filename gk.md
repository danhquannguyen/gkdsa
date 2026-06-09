# Phần 1
<details>
  <summary><code>1. Trình bày mối quan hệ giữa cấu trúc dữ liệu và giải thuật, cho ví dụ minh
hoạ. </code></summary>

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
  <summary><code>2. Để giải quyết một bài toán trên máy tính điện tử ta phải thực hiện một số bước, trong đó có một
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
được với dữ liệu chưa được sắp xếp.</code></summary>

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

# Phần 2 
<details>
  <summary><code>1 Cho cây nhị phân, viết thứ tự các nút được thăm theo các thứ tự: trước, giữa,
sau. Ví dụ: 
  <img width="1000" height="455" alt="image" src="https://github.com/user-attachments/assets/95e1a1d5-0e13-4225-bb8e-9d2272f453fd" /></code></summary>

  Trước: A C G F B E I D H
 
  Giữa: G C F A I E B D H
  
  Sau: G F C I E H D B A
</details>

<details>
  <summary><code>2. Biết thứ tự duyệt cây nhị phân theo thứ tự trước và giữa, hãy dựng lại cây
nhị phân. Ví dụ thứ tự trước là: A B D E H C F I G, thứ tự giữa là: D B H E A F I C
G.</code></summary>

 <img width="1490" height="877" alt="image" src="https://github.com/user-attachments/assets/2d0199f3-03bc-4cfe-99c9-d95d77404040" />


</details>

<details>
  <summary><code>3.  Biết thứ tự duyệt cây nhị phân theo thứ tự giữa và sau, hãy dựng lại cây nhị
phân. Ví dụ thứ tự giữa là: D H B E A F C I G, thứ tự sau là: H D E B F I G C A. </code></summary>

  <img width="1302" height="817" alt="image" src="https://github.com/user-attachments/assets/75f852b9-15f0-4382-9370-2b22bb0c260a" />


</details>

<details>
  <summary><code><img width="532" height="193" alt="image" src="https://github.com/user-attachments/assets/103159c6-3957-4104-a189-f89185bbb962" />
  </code></summary>

  <table border="1" style="border-collapse: collapse; text-align: center; width: 100%;">
  <!-- Hàng tiêu đề 1 -->
  <tr>
    <th rowspan="2" style="background: linear-gradient(to top right, transparent calc(50% - 1px), #000, transparent calc(50% + 1px)); position: relative; width: 80px; height: 50px; padding: 0;">
      <span style="position: absolute; top: 2px; right: 8px; font-weight: normal;">V</span>
      <span style="position: absolute; bottom: 2px; left: 8px; font-weight: normal;">k</span>
    </th>
    <th colspan="2">1</th>
    <th colspan="2">2</th>
    <th colspan="2">3</th>
    <th colspan="2">4</th>
    <th colspan="2">5</th>
    <th colspan="2">6</th>
    <th colspan="2">7</th>
  </tr>
  
  <!-- Hàng dữ liệu 1 (k = 1) -->
  <tr>
    <!-- Hàng trống tương ứng với ô rowspan bên trái -->
  </tr>
  <tr>
    <td><b>1</b></td>
    <td>0</td><td>0</td>
    <td>6</td><td>1</td>
    <td>6</td><td>1</td>
    <td>12</td><td>2</td>
    <td>12</td><td>2</td>
    <td>18</td><td>3</td>
    <td>18</td><td>3</td>
  </tr>
  
  <!-- Hàng dữ liệu 2 (k = 2) -->
  <tr>
    <td><b>2</b></td>
    <td>0</td><td>0</td>
    <td>6</td><td>0</td>
    <td>10</td><td>1</td>
    <td>12</td><td>0</td>
    <td>16</td><td>1</td>
    <td>20</td><td>2</td>
    <td>22</td><td>1</td>
  </tr>
  
  <!-- Hàng dữ liệu 3 (k = 3) -->
  <tr>
    <td><b>3</b></td>
    <td>1</td><td>1</td>
    <td>6</td><td>0</td>
    <td>10</td><td>0</td>
    <td>12</td><td>0</td>
    <td>16</td><td>0</td>
    <td>20</td><td>0</td>
    <td>22</td><td>0</td>
  </tr>
</table>
</details>

