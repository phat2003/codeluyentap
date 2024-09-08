- _padding_: khoảng cách từ viền của khối này tới khối bên trong của khối đó. Không thể dùng số âm , không có giá trị `auto` (có thể hiểu là 1 vật nằm trong cái hộp thì khoảng trống còn lại bên trong cái hộp đó là padding, lưu ý: khi padding lớn hơn width và height thì w,h = 0,hai chỉ số padding và border tăng bao nhiêu thì w và h giảm bấy nhiêu), hiểu ngắn gọn là làm khối to ra và giảm kích thước width, height bên trong nó(hiểu nôm na là 1 hộp gỗ bên trong nó là width và height thì padding làm cho cái vỏ gỗ của hộp to ra về phía trong của hộp khiến cho phần trống bên trong nhỏ đi).
==================
- _margin_: Khoảng cách giữa các khối với nhau,giữa khối này tới khối khác, Có thể dùng số âm, có giá trị `auto`, hiểu ngắn gọn là 1 khối đẩy các khối xung quanh đi
===========================
_float: inline-start;_ : cho khối đó nằm cạnh 1 khối đã có sẵn (xem ví dụ ở file chocackhoinamcanhnhau)
============================
_đơn vị vh_ : là thuộc tính làm 1 đơn vị chiếm full màn hình đang nhìn từ trên xuống dưới hoặc từ trái qua phải nếu được set.
==============================
- _overflow: hidden;_ những thứ tràn ra ngoài khối sẽ bị ẩn đi (ví dụ như chữ nằm trên 1 hàng nhưng số lượng chữ vượt quá độ rộng cố định của 1 khối thì chữ nào bị tràn ra sẽ bị ẩn đi.)
=====================================================
=====flex====
- _flex-direction: row_;/*hiển thị của flex mặc định là ngang(row), có thể chỉnh lại là dọc(column) */
- _align-items: stretch_; /*align-items mặc định là stretch, tác dụng của dòng này là kéo các cột cao bằng nhau khi dùng flex.
    nếu flex set là row thì làm các cột có chiều cao bằng nhau.
    nếu flex set là column thì làm cho các cột có chiều rộng bằng nhau.
    (dòng này có thể hiểu nôm na là ví dụ nếu có 3 cột có nội dung giống nhau nhưng có 1 cột có nội dung ít hơn 2 khối còn lại thì chiều cao/độ rộng của cột đó vẫn sẽ bằng với chiều cao/độ rộng của cột còn lại(cột ở đây tạm hiểu là chiều cao/độ rộng của khối)) */
=====================================================================
- _align-items_ : `flex-start`/`flex-end`/`center`/`baseline` (ba thuộc tính khác của align-items.
`flex-start` sẽ căn đẩy các khối lên trên.
`flex-end` sẽ đẩy các khối dịch xuống.
`center` căn giữa.
`baseline` căn theo chân chữ của dòng chữ đầu tiên
còn khối nào đủ to, không nhỏ hơn so với các khối khác thì nhìn vào vẫn sẽ y nguyên như vậy)
=======================================================
_justify-content: `center`;_ toàn bộ phần tử bên trong 1 khối sẽ nằm giữa
                          `flex-end` toàn bộ phần tử bên trong 1 khối sẽ nằm phải
                          `flex-start` toàn bộ phần tử bên trong 1 khối sẽ nằm trái
                          `space-between` chia đầu cuối: nếu bên trong 1 khối vẫn còn dư chỗ trống do rộng rộng khối đó lớn thì sẽ đẩy các phần tử bên trong chia đều ra 2 phía và chỉ chừa lại 1 khoảng trống ở giữa.
                          `space-around` chia đều 2 bên sao cho bên trái, phải, ở giữa đều có khoảng trống, nhưng khoảng trống ở giữa sẽ lớn hơn khoảng trống 2 bên
                          `space-evenly` chia đều khoảng trống sao cho cả ba khoảng trống trái,phải,giữa đều bằng nhau.
xem ví dụ ở folder (cho các phần tử bên trong 1 khối nằm đều về phía nào)
========================================================
- _display: `-webkit-box`;_ : combo webkit này là để hiển thị 
    _-webkit-line-clamp: `2`;_ vị trí dòng số mấy sẽ hiển thị dấu ba chấm
    _-webkit-box-orient: `vertical`;_
    _overflow: `hidden`;_ : ẩn các thành phần bị tràn ra ngoài của 1 khối.
    _text-overflow: `ellipsis`;_ : cho các chữ nào quá dài và không đủ chỗ để hiển thị hết tất cả thì sẽ hiện dấu ba chấm.
    _word-break: `break-word`;_ chỗ này không đủ chỗ thì nó sẽ xuống dòng nhưng không xuống dòng theo chỗ không đủ mà sẽ xuống dòng theo từ không đủ.
(nguyên 1 combo display: `-webkit-box` trên thì chỉ cần cài evondev snippets nhập text-truncate và enter là ra).
============================================
- _gap_ : giống margin là tạo khoảng cách giữa các phần tử với nhau nhưng gap nếu set ở lớp nào thì sẽ tự chèn 1 khoảng trống vào giữa toàn bộ các phần tử trong lớp đó.
column-gap: 30px; chèn khoảng trống giữa các phần tử theo hàng ngang
row-gap: 30px; chèn khoảng trống giữa các phần tử theo hàng dọc
gap: 30px; chèn khoảng trống giữa các phần tử cả ngang lẫn dọc
=======================================
====display====
- _display_ : nôm na cách mà các khối và nội dung hiển thị
các thuộc tính của _display_:
`flex`: hiển thị nội dung 1 cách linh hoạt
`inline-flex`: hiển thị nội dung trên 1 dòng 1 cách linh hoạt
`inline-block` : thẻ inline sẽ bị giới hạn css, nếu thêm dòng này thì thẻ inline đó sẽ áp dụng được mọi css và có độ rộng bằng nội dung mà nó chứa.
===========================================
====potition====
- _position: ;_ 
`relative`: giúp thay đổi vị trí của 1 phần tử mà không ảnh hưởng hoặc thay đổi vị trí của các phần tử khác, khi phần tử này thay đổi vị trí thì phần tử vẫn chiếm không gian cố định tại vị trí ban đầu, Khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là `absolute` hay không ?
`absolute`: thẻ này có thể tưởng tượng là nó sẽ đưa 1 phần tử lên cao, phần tử không chiếm không gian trong khối đó nữa do đã bay lên cao. (ví dụ : có 2 khối a và b, khối b muốn đứng ngay vị trí của khối a nhưng không được do bị khối a chiếm chỗ rồi, nếu muốn khối b cũng chen được vào vị trí của khối a thì phải dùng lệnh này để đưa khối b lên cao, như vậy khối b sẽ có thể đứng lên trên khối a), Khi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó gần nhất có sử dụng _position_ là `absolute` hay `relative` không ?, vì thường các thẻ có css position `absolute` hay `relative` sẽ đè lên các thẻ không có potition.
thuộc tính _position: absolute_ sẽ di chuyển vị trí nằm đè lên bên trong thẻ cha có chứa _position: relative_ để nằm cố định 1 chỗ.
nôm na dễ hiểu là thẻ con _position: absolute_ có thể bay lên cao di chuyển tới và đè lên bất cứ đâu với phạm vi là thẻ cha có chứa _position: relative_ (thẻ cha sẽ là khu vực bay của thẻ con), còn nếu thẻ cha không có cái nào chứa _position: relative_ thì thẻ chứa _position: absolute_ có thể bay tới và đè lên bất cứ đâu trong body.
===============
