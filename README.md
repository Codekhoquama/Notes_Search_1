Cách sử dụng:
- Hàm xây dựng bản đồ các tập hợp cho mỗi lần tìm kiếm (trong công cụ Javascript, không phải trong QRadar ReferenceData)
- Mỗi dòng thêm giá trị của nó (nếu chưa có) vào bản đồ các tập hợp này và trả về trạng thái hiện tại
- Điều này có nghĩa là chỉ có dòng cuối cùng có bản đồ hoàn chỉnh từ các tập hợp
- Hàm được thực thi cho mỗi EP

Vì bạn cần nhóm concat trên tất cả các EP, trước tiên chúng ta cần lấy dữ liệu trên bảng điều khiển rồi gọi hàm
=> Chúng ta thực hiện việc này bằng truy vấn/truy vấn phụ lồng nhau.
=> phần bên trong trước tiên sẽ truy xuất tất cả các sự kiện. Phần bên ngoài nhóm các sự kiện này và truy xuất sự kiện cuối cùng và do đó là sự kiện hoàn chỉnh từ hàm tùy chỉnh.
