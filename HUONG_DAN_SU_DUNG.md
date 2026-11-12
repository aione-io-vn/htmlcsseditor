# Hướng dẫn sử dụng

Phần mềm soạn & nộp bài HTML/CSS qua mạng LAN. Tài liệu này có 2 phần: **Phần 1** cho giáo viên
(các bước cốt lõi để dạy được ngay buổi đầu), **Phần 2** cho học sinh (in ra phát ở tiết đầu tiên).

Cài đặt phần mềm lên máy: xem [README.md](README.md) mục "Cài đặt".

---

## Phần 1 — Dành cho giáo viên

Các bước dưới đây theo đúng thứ tự, từ lúc vừa cài xong phần mềm đến lúc chấm bài.

### Bước 1. Mở tường lửa (chỉ làm 1 lần)

Chuột phải file `MO_TUONG_LUA.bat` → **Run as administrator**. Bước này cho phép máy học sinh
trong cùng mạng LAN kết nối tới máy giáo viên. Không cần làm lại ở các buổi sau.

### Bước 2. Khởi động máy chủ

Bấm đúp `KHOI_DONG.bat`. Một cửa sổ đen hiện ra và in địa chỉ, ví dụ:

```
Học sinh mở trình duyệt và gõ địa chỉ:
    http://192.168.1.10
```

Ghi đúng địa chỉ này lên bảng cho học sinh. **Giữ cửa sổ đen này mở** suốt tiết học — đóng cửa sổ
là tắt máy chủ, học sinh mất kết nối ngay.

> Lần đầu Windows hỏi về tường lửa: chọn **Private network** → **Allow**.

### Bước 3. Đặt mật khẩu quản trị (chỉ làm 1 lần)

Trên chính máy giáo viên, mở trình duyệt, gõ `http://localhost/admin`. Lần đầu chạy, trang hỏi đặt
mật khẩu (từ 6 ký tự). Mật khẩu này chỉ đặt được từ máy giáo viên, không đặt được từ máy học sinh.
Các lần sau mở `/admin` sẽ hỏi đăng nhập bằng mật khẩu này.

### Bước 4. Kiểm tra thư mục lưu bài

Vào mục **Cài đặt** ở thanh bên. Phần mềm đã tự tạo sẵn một thư mục lưu bài (ví dụ `D:\BAITAP_HTML`)
— nếu muốn đổi sang thư mục khác, nhập đường dẫn mới rồi bấm **Lưu thư mục**. Mỗi bài tập sau này
sẽ là một thư mục con nằm trong đây, mỗi bài nộp là một file `.html` đặt tên theo Lớp + Họ tên.

### Bước 5. Tạo bài tập đầu tiên

Vào mục **Bài tập** → bấm **+ Tạo bài tập mới**:

1. **Tên bài tập** — học sinh sẽ thấy đúng tên này trong danh sách chọn bài.
2. **Đề bài** (không bắt buộc) — soạn có định dạng (đậm/nghiêng/tiêu đề/ảnh/âm thanh/video); để
   trống nếu định đọc đề trực tiếp trên lớp.
3. **Code mẫu** (không bắt buộc) — khung HTML cơ bản nạp sẵn vào ô soạn của học sinh khi các em mở
   bài. Để trống thì học sinh thấy một mẫu HTML cơ bản có sẵn của phần mềm.
4. **Code giải** (không bắt buộc) — lời giải đầy đủ, học sinh chỉ **xem** được ở tab riêng, không
   bị nạp vào ô soạn.
5. Bấm **Lưu**.

Bài tập vừa tạo hiện ngay trong danh sách và học sinh thấy được ngay (không cần khởi động lại gì).

### Bước 6. Theo dõi và chấm bài

Vào mục **Bài nộp**, chọn đúng bài tập ở ô trên cùng. Danh sách học sinh đã nộp hiện bên trái; bấm
vào tên một em để xem bài bên phải (2 tab: **Xem code** và **Xem kết quả**). Có thể:

- Lọc theo **Lớp**, hoặc gõ vào ô **Tìm theo tên** (không cần gõ dấu).
- Chuyển qua lại giữa các em bằng nút **◀ Bài trước / Bài sau ▶** hoặc phím **mũi tên lên/xuống**.
- Bấm **Phóng to** ở tab Xem kết quả để chiếu bài lên màn hình lớn cho cả lớp xem.

### Bước 7. Hết tiết

Đóng cửa sổ đen (hoặc tắt máy) là xong — bài nộp đã lưu trên đĩa, không mất. Buổi học sau chỉ cần
lặp lại **Bước 2**.

### Còn nhiều chức năng khác

Thanh bên còn có: **Thông báo cho lớp** (gửi dòng chữ hiện trên màn hình mọi học sinh), khóa/mở
nộp bài và đặt đếm ngược giờ làm bài (trong mục Bài tập), tải toàn bộ bài nộp thành 1 file `.zip`,
đổi mật khẩu, và mục **Hỗ trợ** (xem phiên bản, tự cập nhật phần mềm khi có bản mới, liên hệ tác
giả). Cứ thử dần khi đã quen với các bước cơ bản ở trên.

**Quên mật khẩu?** Xem mục "Xử lý sự cố" trong [README.md](README.md).

---

## Phần 2 — Dành cho học sinh

**Địa chỉ truy cập:** `http://________________` *(giáo viên ghi lên bảng)*

### Bước 1. Mở trình duyệt và vào toàn màn hình

Mở **Chrome** hoặc **Edge**, gõ địa chỉ giáo viên ghi trên bảng. Trang hiện hộp thoại **bắt buộc
vào chế độ toàn màn hình** — bấm **Đồng ý** mới dùng được trang.

> ⚠️ Sau khi đã vào toàn màn hình, nếu bấm phím **Esc**, chuyển sang cửa sổ khác (Alt+Tab, phím
> Windows...), hoặc bấm **PrintScreen**, trang sẽ **tự thoát** và tab bị đóng. Muốn làm tiếp: mở
> lại đường link (hoặc bấm F5), bấm **Đồng ý** lại từ đầu. Code đang soạn dở **không bị mất** —
> phần mềm tự lưu nháp trước khi thoát.

### Bước 2. Chọn bài tập, nhập tên

Ở thanh trên: chọn **Bài tập**, nhập **Họ tên** và **Lớp** (ví dụ `10A1`).

> Máy này dùng chung nhiều lớp — tên chỉ nhớ đến khi đóng trình duyệt, **không lưu qua ngày
> hôm sau**.

### Bước 3. Soạn code

- Gõ HTML/CSS vào ô bên trái. CSS viết trong cặp thẻ `<style> ... </style>`.
- Kết quả hiện ngay bên phải, tự cập nhật khi ngừng gõ (không chạy được JavaScript).
- Gõ `<` hoặc gõ trong `<style>` sẽ tự hiện gợi ý — bấm **Ctrl + Space** để gọi gợi ý bất cứ lúc
  nào.
- Bài soạn dở tự lưu tạm trong trình duyệt — lỡ bấm F5 hay bị thoát toàn màn hình vẫn còn, nhưng
  **đổi sang máy khác là mất**.

### Bước 4. Chèn ảnh, video, file (nếu cần)

Ba nút **"Lấy link ảnh / video / file"** ở trên **không tự viết thẻ** — phải tự gõ thẻ trước, đặt
con trỏ đúng chỗ, rồi mới bấm nút để điền đường dẫn vào. Ví dụ:

```html
<img src="">          ← đặt con trỏ vào giữa hai dấu ngoặc kép, rồi bấm "Lấy link ảnh"
<video src="" controls></video>   ← tương tự, bấm "Lấy link video"
<a href="">Tải file</a>           ← đặt con trỏ giữa hai dấu ngoặc kép của href, bấm "Lấy link file"
```

Giới hạn: ảnh ≤ 2 MB, video ≤ 10 MB, file (PDF/Word/Excel/PowerPoint/ZIP/RAR/TXT) ≤ 10 MB; tối đa
10 file cho mỗi bài.

> ⚠️ **Chèn ảnh/video/file xong thì đừng đổi lại Họ tên hoặc Lớp nữa** — đổi tên sẽ làm các file
> đã chèn không hiện đúng (phải chèn lại từ đầu).

### Bước 5. Nộp bài

1. Bấm **Nộp bài**.
2. Hộp xác nhận hiện tên — đúng thì bấm **"Đúng, nộp bài"**; nếu không phải tên mình, bấm
   **"Không phải tôi"** rồi nhập lại.
3. Nộp lại bài cũ sẽ **ghi đè** (có hỏi lại trước khi ghi đè).
4. **Nộp lần đầu** của bài này hiện thêm 1 hộp **"Mã lấy lại bài"** — xem cách dùng ở mục ngay
   bên dưới.

### Bước 6. Xem danh sách đã nộp

Bấm nút **Đã nộp** ở thanh trên để xem bạn nào trong lớp đã nộp bài này.

### Lấy lại bài đã nộp (đổi máy, qua ngày khác, hoặc trình duyệt xóa mất bản nháp)

Máy dùng chung nhiều lớp nên bản nháp đang soạn **chỉ nhớ trong trình duyệt hiện tại** (HS-06).
Muốn sửa/bổ sung bài đã nộp vào lúc khác — ngồi máy khác, qua buổi học sau, hoặc trình duyệt đã
quên bản nháp — làm theo 2 bước:

1. **Lúc nộp lần đầu:** ngay sau khi nộp, một hộp hiện ra ghi **"Mã lấy lại bài"** (4 ký tự, ví
   dụ `A1B2`). Mã này **chỉ hiện đúng 1 lần, không hiện lại được** — chụp màn hình hoặc ghi ra
   giấy ngay. Các lần nộp đè sau đó (sửa/bổ sung rồi nộp lại) dùng lại đúng mã này, không cấp mã
   mới, nên không cần lo mã nào là mới nhất.
2. **Lúc cần lấy lại:** mở lại trang, bấm nút **Đã nộp** ở thanh trên → bấm **"Lấy lại bài đã
   nộp của tôi"** → nhập đúng mã đã lưu → bấm **Lấy lại**. **Chỉ cần nhập mã**, không cần nhớ lại
   Họ tên hay Lớp — phần mềm tự điền lại 2 ô đó, và nạp đúng bài đã nộp (bản mới nhất) vào ô soạn.
   Nếu ô soạn đang có code khác, sẽ hỏi xác nhận trước khi ghi đè.

> Lỡ làm mất cả mã: nhờ giáo viên mở trang quản trị xem lại code bài đã nộp rồi gửi cho em.

### Bài nhiều trang (bài "Tạo liên kết")

Khi thầy/cô cho làm bài nhiều trang, trên ô soạn có hàng tab các trang:

1. Trang chủ luôn là **index.html** (không xóa được).
2. Bấm **+ Thêm trang**, gõ tên (ví dụ `thong_tin`) → có trang `thong_tin.html`. Bấm tab để
   chuyển qua lại giữa các trang.
3. Liên kết từ trang này sang trang khác: `<a href="thong_tin.html">Thông tin</a>`. Quay về
   trang chủ: `<a href="index.html">Trang chủ</a>`.
4. Khung Xem trước chỉ hiện **trang đang soạn**. Muốn bấm thử liên kết giữa các trang: **nộp
   bài**, rồi bấm nút **"Xem website đã nộp"** trên khung Xem trước. Gõ tiếp code là quay lại
   xem trước bình thường.
5. Ảnh/video/file chèn bằng nút "Lấy link" tự có dạng `../10A1_NguyenVanAn_files/...` — đúng rồi,
   giữ nguyên, không tự sửa.

### Sự cố thường gặp

| Hiện tượng | Cách xử lý |
| --- | --- |
| Không vào được trang | Kiểm tra đúng địa chỉ giáo viên ghi, cùng mạng Wi-Fi/LAN với máy giáo viên |
| Trang tự thoát, tab đóng | Bình thường khi rời chế độ toàn màn hình — mở lại link, bấm Đồng ý, code không mất |
| Nộp bài báo lỗi | Kiểm tra đã nhập đủ Họ tên và Lớp hợp lệ (2 ký tự trở lên) |
| Chèn ảnh báo "quá lớn" | Chọn ảnh/video/file nhỏ hơn, hoặc nén lại trước |
| Chèn file báo "không hợp lệ" | Chỉ nhận PNG/JPG/GIF/WEBP (ảnh), MP4/WEBM (video), PDF/DOC(X)/XLS(X)/PPT(X)/ZIP/RAR/TXT (file) |

---

Bản quyền © 2026 Đào Viết Danh. Phần mềm miễn phí — chi tiết trong file `LICENSE`.
