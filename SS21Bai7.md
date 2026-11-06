# Bài 7: Chuẩn Hóa Cú Pháp Googling Sửa Lỗi Phần Mềm Điều Khiển Kiosk Trạm Sạc

## Vấn đề:

- Một kỹ thuật viên IT đang cấu hình phần mềm VoltCharge trên máy tính nhưng phần mền báo Lỗi

-Nhân viên thực tập đã tìm kiếm trên Googlenhưng sử dụng các truy vấn quá chung chung, không đúng bối cảnh kỹ thuật và có nhiều từ khóa không an toàn.

## Yêu cầu:

**Phần 1: Phân tích sai lầm trong tư duy tìm kiếm**

**1.** Phân tích vì sao Query 1 của bạn thực tập sinh là một 'Bad Query' điển hình? Thuật toán máy tìm kiếm bị nhiễu loạn như thế nào trước các câu văn nói dài dòng?

**2.** Chỉ ra hiểm họa an ninh thông tin nghiêm trọng nếu nhân viên kỹ thuật click vào các kết quả của Query 3 để sửa máy trạm sạc của công ty.

**Phần 2: Chuẩn hóa Cú pháp Tìm kiếm Chuyên nghiệp**

**3.** Bóc tách thông báo lỗi trên màn hình Kiosk (`Error: Failed to bind OCPP port. System error: Access is denied`) thành 3 thành phần cốt lõi:

**4.** Xây dựng 03 câu lệnh tìm kiếm Google chuẩn kỹ sư (sử dụng phối hợp toán tử `site:`, \`\`, \`-\`):

- Cú pháp 1: Tìm bài viết sửa lỗi chính xác trên diễn đàn Microsoft Community dành riêng cho Windows 11, loại bỏ Windows 7 và Windows 8.

- Cú pháp 2: Tìm tài liệu đặc tả lỗi phân quyền cổng OCPP từ trang chủ của tổ chức liên minh sạc mở (`openchargealliance.org`).

- Cú pháp 3: Tìm hướng dẫn sửa lỗi trên diễn đàn StackOverflow sạch bóng từ khóa quảng cáo và crack.

## Cách làm:

**Phần 1**:

**1**:

- Query 1 của bạn thực tập sinh là một 'Bad Query' điển hình là vì chứa nhiều câu văn nói dài dòng, từ ngữ dư thừa và thiếu từ khóa trọng tâm.

- Điều này khiến máy tìm kiếm khó xác định nội dung cần tìm,làm nhiễu từ khóa chính,mở rộng phạm vi tìm kiếm và trả về nhiều kết quả không liên quan.

**2**: Hiểm hạo thông tin từ Query 3

- Nhiểm mã độc Trojan

- Đánh cắp dữ liệu, mật khẩu và thông tin nội bộ công ty

- Chiếm quyền điều khiển máy trạm Kiosk

- Làm gián đoạn hoạt động của trạm 

**Phần 2**:

**3**: Bóc tách thông báo lỗi 

| Thành phần | Nội dung trích xuất chuẩn | Mục đích |
|---|---|---|
| 1. Tên phần mềm và môi trường | VoltCharge Controller Windows 11 | Xác định phần mềm và hệ điều hành đang sử dụng. |
| 2. Mã lỗi nguyên văn | `"Access is denied"` | Tìm chính xác thông báo lỗi xuất hiện. |
| 3. Thao tác/giao thức | `bind OCPP port` | Xác định thao tác gây ra lỗi. |

**4**:

- Tìm lỗi trên Microsoft Community 

site:answers.microsoft.com "Access is denied" "bind OCPP port" "Windows 11" -win7 -win8

- Tìm tài liệu kx thuật trên Open Charge Alliance

site:openchargealliance.org "Access is denied" "OCPP port" "Windows 11"

-  Tìm hướng dẫn đến StackOverflow

site:stackoverflow.com "Access is denied" "bind OCPP port" "Windows 11" -crack -keygen -quangcao -win7