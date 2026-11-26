# AI Log – Lịch sử sử dụng Agent

Tệp này dùng để ghi lại những lần sử dụng AI Agent trong quá trình phát triển, kiểm tra hoặc bảo trì website Công Minh.

## 1. Mục đích

- Theo dõi yêu cầu đã giao cho AI Agent.
- Ghi lại nội dung Agent đã hỗ trợ.
- Phân biệt phần do Agent đề xuất với phần người phát triển đã kiểm tra và chấp nhận.
- Hỗ trợ truy vết khi cần sửa lỗi hoặc tiếp tục phát triển.

## 2. Nhật ký

| Ngày | Agent/Công cụ | Yêu cầu | Kết quả | Trạng thái |
|---|---|---|---|---|
| 2026-11-17 | ChatGPT | Đọc mã nguồn `index.html` và `style.css`; soạn tài liệu README, AI Log và Change Log | Tạo nội dung hướng dẫn chạy website và hai tệp nhật ký. Không chỉnh sửa mã nguồn HTML/CSS. | Đã tạo tài liệu; cần người phát triển rà soát |

**Ghi chú:** Đây là mục ghi nhận công việc tài liệu được thực hiện trong phiên hiện tại. Không có lịch sử Agent cũ nào được cung cấp trong mã nguồn, vì vậy tệp này không tự tạo thêm các phiên sử dụng trước đó.

## 3. Mẫu ghi nhật ký mới

Sao chép một dòng mẫu dưới đây và điền sau mỗi lần sử dụng Agent:

| Ngày, giờ | Agent/Công cụ | Người yêu cầu | Mục tiêu | Tệp liên quan | Nội dung Agent thực hiện | Kết quả/đường dẫn | Người kiểm tra | Trạng thái |
|---|---|---|---|---|---|---|---|---|
| YYYY-MM-DD HH:MM | Tên Agent | Tên người thực hiện | Mô tả ngắn | `file1`, `file2` | Mô tả công việc | Kết quả cụ thể | Tên người kiểm tra | Chờ kiểm tra/Đã duyệt |

## 4. Quy ước trạng thái

- **Đang thực hiện:** Agent đang xử lý yêu cầu.
- **Chờ kiểm tra:** Đã có kết quả nhưng chưa được kiểm tra.
- **Đã duyệt:** Người phụ trách đã kiểm tra và chấp nhận.
- **Không sử dụng:** Kết quả không được đưa vào dự án.

## 5. Nguyên tắc ghi nhận

1. Ghi đúng ngày thực hiện và tên công cụ/Agent.
2. Nêu rõ yêu cầu đầu vào và kết quả đầu ra.
3. Ghi tên tệp được tạo hoặc chỉnh sửa.
4. Không ghi thông tin bí mật, mật khẩu, khóa API hoặc dữ liệu cá nhân nhạy cảm.
5. Chỉ chuyển trạng thái sang “Đã duyệt” sau khi đã kiểm tra kết quả.
