# BÀI KIỂM TRA ĐÁNH GIÁ NĂNG LỰC (12:00 - 18:00)

## 1. Yêu cầu
-   Tạo repo từ `fork`. Tham khảo [tại đây](https://www.youtube.com/shorts/XvxWFST1i4A)
-   Ngôn ngữ: java 17+, python 3.11+
-   Thư viện:
    - Không bắt buộc
    - Đối với python có thể dùng như điểm cộng. Chú ý tạo `requirements.txt` và phải giải thích được lý do dùng trong phần báo cáo
-   Cho phép dùng AI nhưng phải giải thích được lý do dùng. **NGHIÊM CẤM** cho AI gene câu trả lời từ đầu đến cuối.
- Yêu cầu trung thực. Câu nào không làm được ghi rõ là không biết làm.
- Hoàn thiện báo cáo ở [REPORT.md](/REPORT.md)

## 2. Câu hỏi
### Câu 1: BASE CODE (bai1.java / bai1.py)
> **Đề bài:** Hệ thống yêu cầu bạn quản lý danh sách các tài khoản kiểm toán. Mỗi tài khoản gồm Tên khách hàng và Số tiền gửi ($USD). Nhiệm vụ của bạn là xử lý dữ liệu đầu vào và xây dựng một tính năng truy vấn thông minh: Khi nhập một tên không có dấu, hệ thống vẫn phải tìm và trả về Top 3 tài khoản có tên gần giống nhất kèm theo Tổng số tiền của 3 tài khoản đó.

**Luồng xử lý (Workflow):** 
- **Nhập dữ liệu:** Nhập số lượng tài khoản $N$, sau đó nhập Tên và Số tiền cho từng tài khoản.
- **Tìm kiếm:** Tìm Top 3 tài khoản có tên chứa từ khóa đó. Nếu trùng mức độ ưu tiên, sắp xếp theo số tiền giảm dần. Kết xuất: In ra thông tin Top 3 và tổng số tiền của chúng.
>   - VD: trong ds có Hà, Hằng, Thắng, Trung. Khi gõ 'ha'. Danh sách phải hiển thị Hà, Hằng, Thắng và tổng số tiền tương ứng
- **Chuẩn hóa:** Hiển thị tổng số tiền theo format `1.000,000 USD`

### Câu 2: CRAWL DATA (bai2.py, bai2.java)
- Cho trang web [`bai2_crawled\mock.html`](bai2_crawled\mock.html)

> Đề bài: Viết file đào dữ liệu. Chạy xong lưu vào output dưới dạng `metadata_bai2.json`

**Lưu ý:** Nếu không quen với html có thể cho đọc file từ [bai2_crawled\mock.txt](bai2_crawled\mock.txt)