# 1. Giới thiệu

**Tên dự án:** Phân tích và quản lý yêu cầu cho dự án phát triển hệ thống Quản lý bán hàng và chăm sóc khách hàng cho công ty PepsiCo Vietnam.

**Phát biểu bài toán:**
Hiện tại, PepsiCo Vietnam đang quản lý khách hàng và các giao dịch kinh doanh qua nhiều công cụ rời rạc. Điều này dẫn đến việc khó kiểm soát thông tin, theo dõi cơ hội bán hàng và chăm sóc khách hàng chưa hiệu quả. 

**Mục tiêu dự án:**
Triển khai một hệ thống quản lý và chăm sóc khách hàng (CRM) tích hợp, thông minh nhằm tự động hóa quy trình, hỗ trợ ra quyết định và dễ dàng mở rộng trong tương lai. Dự án do nhóm sinh viên chịu trách nhiệm phân tích, quản lý yêu cầu và triển khai.

---

# 2. Các mức Heading (1-6)
Dưới đây là ví dụ về cách sử dụng 6 mức Heading trong Markdown áp dụng cho tài liệu dự án:

# Heading 1: TÀI LIỆU DỰ ÁN PEPSICO
## Heading 2: 1. Tổng quan hệ thống
### Heading 3: 1.1 Phân tích yêu cầu
#### Heading 4: 1.1.1 Yêu cầu chức năng
##### Heading 5: a. Module Quản lý khách hàng
###### Heading 6: Chi tiết trường dữ liệu khách hàng

---

# 3. Định dạng chữ

Trong dự án này, chúng ta cần lưu ý các từ khóa quan trọng sau:

* **In đậm (Bold):** Hệ thống sẽ được áp dụng cho **PepsiCo Vietnam**.
* *In nghiêng (Italic):* Các chức năng cần đảm bảo tính *tự động hóa* và *thông minh*.
* ***In đậm và in nghiêng (Bold - Italic):*** Chức năng ***tích hợp AI dự đoán*** là điểm nhấn quan trọng nhất của hệ thống báo cáo.
* ~~Gạch ngang (Strikethrough):~~ ~~Sử dụng các công cụ rời rạc cũ~~ (Sẽ được thay thế hoàn toàn).

---

# 4. Danh sách

### Danh sách không thứ tự (Các chức năng chính của hệ thống):
* **Quản lý thông tin khách hàng:** Lưu trữ và phân loại dữ liệu tập trung.
* **Theo dõi lịch sử giao dịch và cơ hội bán hàng:** Ghi nhận, nhắc nhở và cảnh báo kịp thời.
* **Chăm sóc khách hàng tự động:** Gửi email, SMS, thông báo và tích hợp chatbot.
* **Báo cáo và phân tích kinh doanh:** Tổng hợp doanh thu, KPI, tích hợp AI dự đoán và gợi ý chiến lược.

### Danh sách có thứ tự (Quy trình thực hiện của nhóm):
1. Phân tích bài toán hiện tại của doanh nghiệp.
2. Thu thập và quản lý yêu cầu hệ thống.
3. Thiết kế kiến trúc phần mềm.
4. Triển khai hệ thống tự động hóa.
5. Kiểm thử và bàn giao.

---

# 5. Liên kết

Dưới đây là một số liên kết tài liệu tham khảo cho dự án:

* [Trang chủ PepsiCo Việt Nam](https://suntorypepsico.vn/)
* [Tài liệu Hướng dẫn sử dụng Markdown trên GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* Để liên hệ với nhóm phát triển, vui lòng gửi email tới: [admin@example.com](mailto:admin@example.com)

---

# 6. Hình ảnh

*(Dưới đây là cú pháp để chèn hình ảnh. Bạn hãy thay thế `link_hinh_anh_cua_ban` bằng URL hình ảnh thực tế của sơ đồ hệ thống)*

![Sơ đồ phát biểu bài toán PepsiCo](https://via.placeholder.com/800x400.png?text=Sơ+đồ+Kiến+trúc+Hệ+thống+CRM+-+PepsiCo)

> **Lưu ý:** Nếu bạn có file ảnh lưu trong cùng thư mục GitHub, bạn có thể dùng đường dẫn tương đối như `![Sơ đồ](./images/sodo.png)`

---

# 7. Code

### Code trên một dòng (Inline code)
Để chạy dự án ở môi trường local, bạn cần cài đặt `Node.js` và chạy lệnh `npm install` trước khi khởi động.

### Khối code (Code block)
Dưới đây là ví dụ minh họa một đoạn code mô phỏng chức năng **Chăm sóc khách hàng tự động** (Gửi Email) bằng Python:

```python
import smtplib
from email.message import EmailMessage

def send_automated_email(customer_email, customer_name):
    """
    Hàm gửi email chăm sóc khách hàng tự động cho hệ thống CRM PepsiCo
    """
    msg = EmailMessage()
    msg.set_content(f"Kính chào {customer_name},\nCảm ơn bạn đã đồng hành cùng PepsiCo Vietnam!")
    msg['Subject'] = 'Thông báo từ PepsiCo CRM'
    msg['From'] = 'crm_system@pepsico.example.com'
    msg['To'] = customer_email

    # Giả lập gửi email
    print(f"Đang gửi email tự động tới: {customer_email}...")
    # server = smtplib.SMTP('localhost')
    # server.send_message(msg)
    # server.quit()
    print("Gửi thành công!")

# Test thử hàm
send_automated_email("khachhang@gmail.com", "Nguyễn Văn A")
