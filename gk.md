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
</details>


<details>
  <summary><code><img width="1169" height="106" alt="image" src="https://github.com/user-attachments/assets/58536883-de2d-4856-95fe-734240e11cc1" />
</code></summary>

</details>



<details>
  <summary><code><img width="1118" height="51" alt="image" src="https://github.com/user-attachments/assets/4b8d08d9-cb3d-49ed-9e35-eba856ac16de" />
</code></summary>
</details>


<details>
  <summary><code><img width="1178" height="146" alt="image" src="https://github.com/user-attachments/assets/0a39c54b-254f-4c7a-814f-37b090cb16bc" />
</code></sumamry>
</details>


<details>
  <summary><code><img width="1186" height="114" alt="image" src="https://github.com/user-attachments/assets/d6e00437-8dbf-49aa-aec1-7208c9fd2d50" />
</code></summary>
</details>



<details>
  <summary><code><img width="1199" height="160" alt="image" src="https://github.com/user-attachments/assets/6ebbaaee-7ef2-40be-ad8c-42e8cb83ac28" />
</code></summary>
</details>



<details>
  <summary><code><img width="1077" height="73" alt="image" src="https://github.com/user-attachments/assets/37b9e308-def8-49aa-9c22-577523935668" />
</code></summary>
</details>


<details>
  <summary><code><img width="1141" height="76" alt="image" src="https://github.com/user-attachments/assets/1d257353-9cd0-4959-a89c-fddde5ebb4ae" />
</code></summary>
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
</details>



<details>
  <summary><code><img width="1153" height="254" alt="image" src="https://github.com/user-attachments/assets/8cece176-415d-4bcb-97c6-92aa36ea439a" />
</code></summary>
</details>



<details>
  <summary><code><img width="1170" height="212" alt="image" src="https://github.com/user-attachments/assets/68a21569-07b1-4858-8d4c-e2aad08163a3" />
</code></summary>
</details>



<details>
  <summary><code></code><img width="1188" height="254" alt="image" src="https://github.com/user-attachments/assets/8ad569c1-f3e9-4ba2-bf17-20744edc8269" />
</summary>
</details>



<details>
  <summary><code></code><img width="1196" height="255" alt="image" src="https://github.com/user-attachments/assets/9870a90a-dea9-40c7-bfb9-7608380637c9" />
</summary>
</details>



<details>
  <summary><code><img width="1177" height="131" alt="image" src="https://github.com/user-attachments/assets/bc42b71a-92e4-4c1f-9a03-7690cdefa820" />
</code></summary>
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
