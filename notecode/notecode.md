_float: inline-start;_ : cho khối đó nằm cạnh 1 khối đã có sẵn (xem ví dụ ở file chocackhoinamcanhnhau)
_đơn vị vh_ : là thuộc tính làm 1 đơn vị chiếm full màn hình đang nhìn từ trên xuống dưới hoặc từ trái qua phải nếu được set.
_text-align: `center`;_ : căn giữa chữ của 1 khối hoặc thẻ nào đó.
                   `left`: căn trái chữ
                   `right`: căn phải chữ
- _flex-direction: row_;/*hiển thị của flex mặc định là ngang(row), có thể chỉnh lại là dọc(column) */
- _align-items: stretch_; /*align-items mặc định là stretch, tác dụng của dòng này là kéo các cột cao bằng nhau khi dùng flex.
    nếu flex set là row thì làm các cột có chiều cao bằng nhau.
    nếu flex set là column thì làm cho các cột có chiều rộng bằng nhau.
    (dòng này có thể hiểu nôm na là ví dụ nếu có 3 cột có nội dung giống nhau nhưng có 1 cột có nội dung ít hơn 2 khối còn lại thì chiều cao/độ rộng của cột đó vẫn sẽ bằng với chiều cao/độ rộng của cột còn lại(cột ở đây tạm hiểu là chiều cao/độ rộng của khối)) */
- _align-items_ : `flex-start`/`flex-end`/`center`/`baseline` (ba thuộc tính khác của align-items.
`flex-start` sẽ căn đẩy các khối lên trên.
`flex-end` sẽ đẩy các khối dịch xuống.
`center` căn giữa.
`baseline` căn theo chân chữ của dòng chữ đầu tiên
còn khối nào đủ to, không nhỏ hơn so với các khối khác thì nhìn vào vẫn sẽ y nguyên như vậy)
_justify-content: `center`;_ toàn bộ phần tử bên trong 1 khối sẽ nằm giữa
                          `flex-end` toàn bộ phần tử bên trong 1 khối sẽ nằm phải
                          `flex-start` toàn bộ phần tử bên trong 1 khối sẽ nằm trái
                          `space-between` chia đầu cuối: nếu bên trong 1 khối vẫn còn dư chỗ trống do rộng rộng khối đó lớn thì sẽ đẩy các phần tử bên trong chia đều ra 2 phía và chỉ chừa lại 1 khoảng trống ở giữa.
                          `space-around` chia đều 2 bên sao cho bên trái, phải, ở giữa đều có khoảng trống, nhưng khoảng trống ở giữa sẽ lớn hơn khoảng trống 2 bên
                          `space-evenly` chia đều khoảng trống sao cho cả ba khoảng trống trái,phải,giữa đều bằng nhau.
xem ví dụ ở folder (cho các phần tử bên trong 1 khối nằm đều về phía nào)
