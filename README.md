# Công Minh – Website mua bán sách

Tài liệu hướng dẫn cài đặt, chạy thử và sử dụng website Công Minh.

## 1. Giới thiệu

Đây là website giới thiệu dịch vụ mua bán sách mới và thu mua sách cũ của Công Minh. Giao diện được xây dựng bằng **HTML5** và **CSS3**, không sử dụng JavaScript hoặc cơ sở dữ liệu.

Các chức năng/giao diện hiện có:
- Thanh điều hướng đến các khu vực trên trang.
- Danh sách 6 đầu sách mẫu, chia thành Văn học, Công nghệ và Kỹ năng.
- Bộ lọc danh mục sách thực hiện bằng CSS.
- Giới thiệu dịch vụ, bảng giá thu mua sách cũ.
- Quy trình đặt sách gồm 4 bước.
- Các câu hỏi thường gặp có thể mở/đóng.
- Biểu mẫu liên hệ có kiểm tra dữ liệu cơ bản từ trình duyệt.
- Thông tin liên hệ ở cuối trang.

## 2. Yêu cầu

- Máy tính có trình duyệt web hiện đại: Google Chrome, Microsoft Edge, Firefox hoặc Safari.
- Không cần cài máy chủ, Node.js, PHP hay hệ quản trị cơ sở dữ liệu để xem giao diện tĩnh.

## 3. Cấu trúc thư mục

Đặt các tệp trong cùng một thư mục như sau:

```text
CongMinh/
├── index.html
├── style.css
├── README.md
├── AI_log.md
└── change_log.md
```


## 4. Cách chạy website

### Cách 1: Mở trực tiếp

1. Giải nén hoặc sao chép toàn bộ tệp vào cùng một thư mục.
2. Kiểm tra tên `index.html` và `style.css` chính xác như cấu trúc ở trên.
3. Nhấp đúp vào `index.html`.
4. Trình duyệt sẽ mở website. Bạn có thể sử dụng menu, bộ lọc sách, phần hỏi đáp và biểu mẫu để kiểm tra giao diện.

### Cách 2: Mở bằng Visual Studio Code

1. Mở Visual Studio Code.
2. Chọn **File → Open Folder...** và chọn thư mục `CongMinh`.
3. Mở tệp `index.html`.
4. Có thể mở tệp bằng trình duyệt từ File Explorer; nếu đã cài tiện ích Live Server, nhấp chuột phải `index.html` và chọn **Open with Live Server**.

## 5. Hướng dẫn sử dụng và kiểm tra

- **Điều hướng:** Nhấp Sách, Dịch vụ, Quy trình, Hỏi đáp hoặc Liên hệ trên thanh đầu trang.
- **Lọc sách:** Chọn Tất cả, Văn học, Công nghệ hoặc Kỹ năng.
- **Xem hỏi đáp:** Nhấp vào từng câu hỏi để mở nội dung trả lời.
- **Kiểm tra biểu mẫu:** Nhập họ tên, email và nội dung theo hướng dẫn rồi nhấn Gửi tin nhắn.

## 6. Giới hạn hiện tại cần biết

- Website hiện là giao diện tĩnh. Danh sách sách và thông tin dịch vụ được viết trực tiếp trong HTML.
- Biểu mẫu liên hệ đang có `action="#"`; do đó, nhấn gửi **không gửi dữ liệu đến cửa hàng hoặc máy chủ**. Trình duyệt chỉ kiểm tra một số trường bắt buộc và định dạng.
- Các liên kết Facebook, thông tin cửa hàng và dữ liệu sách là nội dung mẫu trong mã nguồn; hãy cập nhật trước khi triển khai thực tế.
- Website tải phông chữ Be Vietnam Pro từ Google Fonts. Nếu không có kết nối Internet, trình duyệt sẽ dùng phông chữ dự phòng.
- Chưa có chức năng đăng nhập, giỏ hàng, thanh toán trực tuyến, quản trị sách hoặc lưu đơn hàng.

## 7. Chỉnh sửa nội dung

- Nội dung, tên sách, giá bán, dịch vụ, câu hỏi và thông tin liên hệ: chỉnh trong `index.html`.
- Màu sắc, bố cục, khoảng cách, kích thước chữ và hiển thị trên thiết bị di động: chỉnh trong `style.css`.
- Sau khi lưu thay đổi, tải lại trang trong trình duyệt (nhấn `Ctrl + F5` nếu cần làm mới bộ nhớ đệm).

## 8. Xử lý lỗi thường gặp

| Hiện tượng | Cách kiểm tra |
|---|---|
| Trang chỉ hiện chữ, không có định dạng | Đảm bảo `style.css` nằm cùng thư mục với `index.html` và đúng tên tệp. |
| Mở trang không được | Kiểm tra tệp `index.html` có tồn tại và thử mở bằng Chrome hoặc Edge. |
| Bộ lọc sách không hoạt động | Kiểm tra các radio `c-all`, `c-van`, `c-cntt`, `c-ky` và thuộc tính `data-cat` trong HTML; không cần JavaScript cho bộ lọc hiện tại. |
| Gửi biểu mẫu nhưng không nhận được tin | Đây là giới hạn hiện tại: biểu mẫu chưa kết nối backend hoặc dịch vụ nhận dữ liệu. |

---
Tài liệu được lập dựa trên mã nguồn HTML/CSS hiện có.
