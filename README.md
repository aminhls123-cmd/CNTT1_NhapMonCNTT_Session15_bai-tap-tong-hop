# (Bài tập tổng hợp) Nhóm SmartCampus Chạy Nước Rút Trước Deadline Nộp Báo Cáo

## Phần 1 – Thiết lập Hybrid Workflow
1. **Sự cố mất file khi hỏng ổ cứng:** Không xảy ra. Vì mô hình *Hybrid Workflow* kết hợp *Auto Sync* (Delta Sync) đã tự động đồng bộ ngầm mọi thay đổi lên Cloud theo thời gian thực.
2. **3 bước thiết lập Auto Sync:**
   - Bước 1: Cài đặt ứng dụng đồng bộ đám mây (Google Drive / OneDrive).
   - Bước 2: Tạo thư mục dự án nằm trong thư mục đồng bộ.
   - Bước 3: Lưu và làm việc trực tiếp tại thư mục đó.
3. **Khôi phục file bị xóa nhầm:** Nhấp chuột phải vào file trên Cloud, chọn **Version History**, chọn mốc thời gian trước khi xóa và nhấn **Restore**.
4. **Xử lý sai lầm:** 
   - Đồng bộ `node_modules` (gây treo app): Thêm vào `.gitignore` và dùng lệnh `npm install` để tái tạo.
   - Lưu phim 4K cá nhân: Di chuyển ra ngoài, không để trong thư mục dự án chung.

---

## Phần 2 – Phân quyền chia sẻ an toàn
1. **Bảng phân quyền:**

| File tài liệu | Mức quyền | Phạm vi chia sẻ | Giải thích |
| :--- | :--- | :--- | :--- |
| **`BaoCao_CuoiKy_SmartCampus.docx`** (giảng viên) | **Viewer** | **Restricted** | Giảng viên chấm điểm |
| **`Slide_BaoCao.pptx`** (5 thành viên) | **Editor** | **Restricted** | Cùng chỉnh sửa gấp slide chung. |
| **`GopY_BanNhap.docx`** (anh khóa trên) | **Commenter** | **Restricted** | Nhận xét góp ý trực tiếp, không sửa file gốc. |
| **`ThongTin_CaNhan_NhomVien.xlsx`** | **Editor** (nội bộ) | **Restricted** | Bảo mật tuyệt đối dữ liệu cá nhân (CCCD, SĐT). |

2. **Quy tắc Cờ Đỏ Bảo mật:** Tuyệt đối không kết hợp liên kết công khai với quyền `Editor` cho file chứa dữ liệu cá nhân để tránh lộ thông tin hoặc bị xóa dữ liệu.
3. **2 thao tác Settings:** Tắt quyền *"Editors can change permissions and share"* và bật giới hạn tải xuống nếu cần.

---

## Phần 3 – Tổ chức giao tiếp nhóm chuẩn doanh nghiệp
1. **3 vấn đề trong chat Zalo:** Lỗi No-Hello, spam ảnh giải trí làm loãng công việc, tag `@all` lúc nửa đêm (23:47).
2. **Đề xuất Channel:** `#thong-bao-chung`, `#thao-luan-du-an`, `#giai-tri-meme`.
3. **Viết lại tin nhắn của Lan:** 
   > *"Chào mọi người, mình đang gặp lỗi ở module xử lý dữ liệu. Bạn nào rảnh có thể trao đổi qua thread này giúp mình nhé!"*
4. **Viết lại tin nhắn 23:47 :** 
   > *[@Minh @Tuan] Chào mọi người, ngày mai là hạn nộp báo cáo SmartCampus rồi. Các bạn hoàn thành nốt phần việc của mình giúp nhóm nhé!*

---

## Phần 4 – Thông báo tổng hợp
*Đăng lên kênh `#thong-bao`:*
> `@all Chào mọi người, mình đã hoàn tất các việc sau:`
> `1. Đã bật **Auto Sync** toàn bộ thư mục dự án lên Cloud Workspace.`
> `2. Đã chia sẻ file báo cáo cho giảng viên đúng chuẩn **Restricted** với quyền **Viewer**.`
> `3. @Minh @Tuan Các bạn kiểm tra và hoàn thành gấp phần nội dung còn thiếu để kịp deadline nhé!`
