# BÀI TẬP TỔNG HỢP: HỒ SƠ DỰ ÁN EDTECH "PTIT-LEARNING"

---

## PHẦN 1: PHÂN TÍCH SƠ ĐỒ CÂY CẤU TRÚC HEADING CHO TÀI LIỆU SRS (WORD)

Để kiểm soát tài liệu SRS cho module "Học trực tuyến" và hiển thị trọn vẹn trên Navigation Pane của Microsoft Word với tổng cộng 10 tiêu đề cấp 2, cấu trúc phân cấp cây thư mục Heading được thiết kế như sau:

* **1. Giới thiệu tổng quan hệ thống (Heading 1)**
  * 1.1 Mục đích và phạm vi giải pháp EdTech (Heading 2)
  * 1.2 Đối tượng sử dụng nền tảng (Heading 2)
* **2. Yêu cầu chức năng module "Lớp học ảo" (Heading 1)**
  * 2.1 Quản lý phòng học trực tuyến và phát trực lượng video (Heading 2)
  * 2.2 Tương tác trực tiếp qua Chat và tính năng giơ tay phát biểu (Heading 2)
  * 2.3 Chia nhóm thảo luận (Breakout Rooms) cho học viên (Heading 2)
  * 2.4 Điểm danh tự động qua thời gian tham gia (Heading 2)
* **3. Quản lý dữ liệu khóa học và học viên (Heading 1)**
  * 3.1 Quy tắc quản lý và lọc danh sách 200 khóa học đa điều kiện (Heading 2)
  * 3.2 Cơ chế phân quyền và ghi nhận kết quả học tập (Heading 2)
* **4. Yêu cầu phi chức năng và bảo mật (Heading 1)**
  * 4.1 Băng thông và độ trễ tối ưu cho đường truyền video (Heading 2)
  * 4.2 Bảo mật dữ liệu cá nhân và mã hóa phiên học (Heading 2)

---

## PHẦN 2: TRIỂN KHAI HỒ SƠ DỰ ÁN (WORD, EXCEL, POWERPOINT)

### 1. Phần Excel: Hướng dẫn Lọc AutoFilter Đa Điều Kiện (Điểm chuyên cần < 7 và Khoa CNTT)
Để quản lý danh sách 200 khóa học và học viên đăng ký theo đúng ràng buộc (Hàng đầu tiên là Header Row duy nhất, không chứa hàng tổng cộng ngắt quãng ở giữa dữ liệu), thao tác sử dụng `Ctrl + Shift + L` được thực hiện như sau:

* **Bước 1: Chuẩn hóa vùng dữ liệu**
  Đảm bảo hàng 1 là tiêu đề duy nhất (Header). Không chèn các dòng tính tổng (Total / Subtotal) ở giữa bảng dữ liệu.
* **Bước 2: Kích hoạt bộ lọc AutoFilter**
  Bôi đen toàn bộ bảng dữ liệu, nhấn tổ hợp phím **`Ctrl + Shift + L`** để hiển thị các mũi tên bộ lọc trên hàng tiêu đề.
* **Bước 3: Lọc đa điều kiện**
  * Tại cột **"Khoa"**: Nhấp vào mũi tên lọc, bỏ chọn tất cả và chỉ tích chọn ô **"CNTT"** (hoặc dùng Text Filters ➔ Equals ➔ CNTT).
  * Tại cột **"Điểm chuyên cần"**: Nhấp vào mũi tên lọc, chọn **Number Filters ➔ Less Than (Nhỏ hơn)**, sau đó nhập giá trị **`7`**.
* *Kết quả:* Excel sẽ lọc ra chính xác danh sách các sinh viên thuộc khoa CNTT có điểm chuyên cần dưới 7 để cố vấn học tập gửi cảnh báo.

---

### 2. Phần PowerPoint: Thiết kế Slide Trực quan (Rule 3 Vùng & Combo Màu Tối)
Slide giới thiệu tính năng "Lớp học ảo" được thiết kế tuân thủ nghiêm ngặt các tiêu chuẩn kỹ thuật:

* **Phối màu & Độ tương phản (Contrast Ratio):**
  * **Màu nền (Background):** Xanh Navy tối (`#0B132B`) giúp giảm mỏi mắt và tăng độ tập trung.
  * **Màu chữ (Text Color):** Trắng sáng (`#FFFFFF`) đảm bảo tỷ lệ tương phản cao tuyệt đối (High Contrast Ratio).
  * **Màu điểm nhấn (Accent Color):** Cam sáng (`#FF6B35`) dùng cho các tiêu đề chính, biểu tượng hoặc nút quan trọng.
* **Cấu trúc Slide chuẩn 3 vùng (Flowchart Lộ trình học tập):**
  * **Vùng 1 (Tiêu đề - Top):** Assertion Title khái quát nội dung: *"Lộ trình học tập trực tuyến tối ưu hóa tương tác thời gian thực"* (Font chữ tối thiểu **30pt**).
  * **Vùng 2 (Nội dung trung tâm - Center Flowchart):** Sơ đồ khối (Flowchart) chia thành 3 bước ngang: `[Đăng nhập lớp]` ➔ `[Tham gia bài giảng & Tương tác]` ➔ `[Làm bài tập & Nhận feedback]`.
  * **Vùng 3 (Chân trang - Bottom):** Thông tin định danh thương hiệu Startup EdTech PTIT-Learning.

---

## PHẦN 3: KIỂM THỬ VÀ XỬ LÝ LỖI KHI LỌC DỮ LIỆU TÊN (HÀM TRIM)

**Tình huống kiểm thử:** Khi thực hiện lọc sinh viên theo tên trên Excel nhưng hệ thống không trả về kết quả mặc dù bằng mắt thường nhìn thấy tên đó xuất hiện trong bảng.

**Nguyên nhân và Quy trình xử lý bằng hàm `TRIM`:**
1. **Nguyên nhân gốc rễ:** Dữ liệu họ tên học viên được đồng bộ từ nhiều nguồn khác nhau (Form đăng ký web, file CSV, Excel thô), dẫn đến việc xuất hiện các **khoảng trắng vô hình** ở đầu, ở cuối hoặc các khoảng trắng kép ở giữa chuỗi (Ví dụ: `"Nguyễn Văn An "` khác với `"Nguyễn Văn An"`). Khi lọc chính xác, Excel không tìm thấy khớp giá trị.
2. **Quy trình xử lý khắc phục:**
   * **Bước 1:** Chèn một cột phụ ngay bên cạnh cột họ tên cần kiểm tra.
   * **Bước 2:** Sử dụng hàm `TRIM()` để làm sạch khoảng trắng thừa bằng công thức:
     ```excel
     =TRIM(A2)
     ```
     *(Trong đó A2 là ô chứa họ tên học viên bị lỗi).*
   * **Bước 3:** Kéo công thức xuống cho toàn bộ các dòng dữ liệu. Hàm `TRIM` sẽ tự động cắt bỏ mọi khoảng trắng thừa không cần thiết.
   * **Bước 4:** Copy toàn bộ cột phụ vừa làm sạch, nhấp chuột phải vào cột họ tên gốc chọn **Paste as Values** (Dán giá trị) để ghi đè dữ liệu chuẩn, sau đó xóa cột phụ đi. Lúc này, tính năng lọc AutoFilter sẽ hoạt động chính xác tuyệt đối.