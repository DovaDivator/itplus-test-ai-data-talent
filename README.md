# BÀI KIỂM TRA ĐÁNH GIÁ NĂNG LỰC (09:00 - 16:00)

## 1. Yêu cầu
- Tạo repo từ `fork`. Tham khảo [tại đây](https://www.youtube.com/shorts/XvxWFST1i4A)
- Ngôn ngữ: Java 17+, Python 3.11+
- Thư viện:
  - Không bắt buộc
  - Đối với Python có thể dùng như điểm cộng. Chú ý tạo `requirements.txt` và phải giải thích được lý do dùng trong phần báo cáo
- Cho phép dùng AI nhưng phải giải thích được lý do dùng. **NGHIÊM CẤM** cho AI generate câu trả lời từ đầu đến cuối.
- Yêu cầu trung thực. Câu nào không làm được ghi rõ là không biết làm.
- Hoàn thiện báo cáo ở [REPORT.md](/REPORT.md)
- Nộp file dưới dạng link git hoặc đóng zip gửi vào Zalo

## 2. Câu hỏi thực hành

### Câu 1: BASE CODE (bai1.java / bai1.py)
> **Đề bài:** Hệ thống yêu cầu bạn quản lý danh sách các tài khoản kiểm toán. Mỗi tài khoản gồm Tên khách hàng và Số tiền gửi ($USD). Nhiệm vụ của bạn là xử lý dữ liệu đầu vào và xây dựng một tính năng truy vấn thông minh: khi nhập một tên không có dấu, hệ thống vẫn phải tìm và trả về Top 3 tài khoản có tên gần giống nhất kèm theo tổng số tiền của 3 tài khoản đó.

**Luồng xử lý (Workflow):**
- **Nhập dữ liệu:** Nhập số lượng tài khoản `N`, sau đó nhập Tên và Số tiền cho từng tài khoản.
- **Tìm kiếm:** Tìm Top 3 tài khoản có tên chứa từ khóa đó. Nếu trùng mức độ ưu tiên, sắp xếp theo số tiền giảm dần. Kết xuất: in ra thông tin Top 3 và tổng số tiền của chúng.
  - VD: trong ds có Hà, Hằng, Thắng, Trung. Khi gõ `ha`. Danh sách phải hiển thị Hà, Hằng, Thắng và tổng số tiền tương ứng
- **Chuẩn hóa:** Hiển thị tổng số tiền theo format `1.000,000 USD`

### Câu 2: CRAWL DATA (bai2.py, bai2.java)
- Cho trang web [`bai2_crawled\mock.html`](bai2_crawled\mock.html)

> Đề bài: Viết file đào dữ liệu. Chạy xong lưu vào output dưới dạng `metadata_bai2.json`

**Lưu ý:** Nếu không quen với html có thể cho đọc file từ [bai2_crawled\mock.txt](bai2_crawled\mock.txt)

### Câu 3: DE CASE
> Mục tiêu là xem tư duy dữ liệu: làm sạch, chuẩn hóa, kiểm tra chất lượng và tổ chức đầu ra.

Bạn nhận một gói dữ liệu gồm:
- 1 file CSV có 200 dòng sản phẩm, trong đó có dòng trùng, thiếu giá, và tên sản phẩm không thống nhất.
- 1 file text mô tả sản phẩm.

- **3.1.** Nếu bạn phải bàn giao dữ liệu này cho team khác dùng tiếp, 4 bước đầu tiên bạn sẽ làm là gì?
- **3.2.** Trong dữ liệu này, 3 loại lỗi nào bạn sẽ ưu tiên xử lý trước? Vì sao?
- **3.3.** Nếu chỉ được giữ lại 1 phiên bản dữ liệu sạch trong ngày đầu, bạn sẽ giữ những trường nào và bỏ những trường nào?

### Câu 4: AI CASE
> Mục tiêu là xem tư duy mô hình / bài toán: chọn baseline, đánh giá, và nhìn ra lỗi sai.

Team đưa cho bạn:
- 1 tập dữ liệu nhỏ gồm câu hỏi và câu trả lời mẫu.
- 3 ví dụ model trả lời sai.
- 1 yêu cầu: làm một demo nhỏ trả lời đúng hơn ở mức cơ bản nhất.

- **4.1.** Nếu là người bắt đầu, bạn sẽ chọn baseline nào trước để thử nhanh?
- **4.2.** Với 3 ví dụ trả lời sai, bạn sẽ phân tích lỗi theo 3 góc nào?
- **4.3.** Nếu chỉ được cải thiện 1 thứ trong tuần đầu, bạn sẽ ưu tiên dữ liệu, prompt, hay đánh giá? Vì sao?

### Câu 5: RAG CASE
> Mục tiêu là xem tư duy truy xuất tài liệu: chia đoạn, tìm đúng ngữ cảnh và kiểm tra câu trả lời có bám nguồn hay không.

Bạn được giao:
- 1 tập tài liệu ngắn rời rạc.
- 10 câu hỏi nội bộ.
- Yêu cầu demo phải trả lời có dẫn nguồn.

- **5.1.** Bạn sẽ chia tài liệu và chuẩn bị chỉ mục theo cách nào để dễ truy xuất nhất?
- **5.2.** Nếu câu trả lời gần đúng nhưng dẫn nhầm đoạn, bạn sẽ kiểm tra lỗi ở bước nào trước?
- **5.3.** Nếu phải chọn giữa trả lời ngắn nhưng chắc, hoặc trả lời dài nhưng có nguy cơ lạc nguồn, bạn sẽ ưu tiên gì trong bản demo đầu tiên?
- **5.4.** Nếu nguồn dữ liệu có cả ảnh chụp màn hình và văn bản, bạn sẽ gán nhãn ảnh theo tiêu chí nào để phục vụ RAG? Nêu tối thiểu 3 nhãn và mô tả ngắn cho mỗi nhãn.
