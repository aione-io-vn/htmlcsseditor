# Soạn & Nộp bài HTML/CSS qua mạng LAN

Phần mềm **miễn phí** cho phòng máy Tin học THPT: học sinh soạn HTML/CSS (gợi ý code, xem kết quả
ngay) và nộp bài vào máy giáo viên qua mạng LAN. Khi dạy không cần Internet, học sinh không cần
đăng nhập.

Kho này **chỉ chứa bản đóng gói** để tải về và để phần mềm tự cập nhật.

## Video giới thiệu

Bấm vào ảnh để xem trên YouTube:

<a href="https://www.youtube.com/watch?v=Et6L2yWU_pw" title="Xem video giới thiệu trên YouTube">
  <img src="https://img.youtube.com/vi/Et6L2yWU_pw/maxresdefault.jpg" alt="Video giới thiệu phần mềm HTML CSS EDITOR" width="640">
</a>

## Yêu cầu

- Máy giáo viên: Windows 10/11, Node.js bản LTS.
- Máy học sinh: Chrome hoặc Edge, cùng mạng LAN với máy giáo viên.

## Cài đặt (một lần)

1. Vào mục [Releases](https://github.com/aione-io-vn/htmlcsseditor/releases), tải file
   `HTMLEDITOR-<phiên bản>.zip` mới nhất.
2. **Trước khi giải nén:** chuột phải file .zip → **Properties** → tích ô **Unblock** (Bỏ chặn) ở
   cuối → OK. Bỏ qua bước này thì Windows sẽ cảnh báo "Windows protected your PC" khi bấm file .bat
   (nếu đã lỡ gặp: bấm **More info** → **Run anyway**).
3. Giải nén vào thư mục `D:\PHANMEM\HTMLEDITOR` (sao cho file `KHOI_DONG.bat` nằm ngay trong thư mục đó).
4. Nếu máy chưa có Node.js: tải bản **LTS** (file `.msi` cho Windows 64-bit) ở https://nodejs.org,
   chạy, bấm Next đến hết. Kiểm tra: mở PowerShell, gõ `node -v` thấy số phiên bản là được.
5. Chuột phải `MO_TUONG_LUA.bat` → **Run as administrator** (chỉ cần một lần) để máy học sinh vào được.
6. Bấm đúp `KHOI_DONG.bat`. Cửa sổ đen hiện địa chỉ (ví dụ `http://192.168.1.10`) — ghi lên bảng cho
   học sinh gõ. Trang quản trị: mở `http://localhost/admin` trên máy giáo viên, lần đầu đặt mật khẩu.

> **Không bắt buộc:** địa chỉ máy giáo viên có thể đổi giữa các buổi (phần mềm vẫn chạy bình thường,
> chỉ cần xem địa chỉ mới trên cửa sổ đen). Muốn địa chỉ luôn cố định thì nhờ người phụ trách phòng
> máy đặt IP tĩnh cho máy giáo viên.

Hướng dẫn đầy đủ (sử dụng, xử lý sự cố) trong file `README.md` bên trong gói.

## Cập nhật

Đã cài rồi thì không cần tải lại: khi máy giáo viên có Internet, trang quản trị tự báo có phiên bản
mới, bấm **Cập nhật ngay** là xong. Bài nộp, đề bài, mật khẩu giữ nguyên.

## Bản quyền

Bản quyền © 2026 Đào Viết Danh (GV Trường THPT Lý Thái Tổ - TP Hồ Chí Minh). Phần mềm **miễn phí**:
được cài, dùng và chia sẻ bản gốc nguyên vẹn. **Không được** sửa đổi, bán, xóa thông tin tác giả
hay phát hành lại dưới tên khác khi chưa có sự đồng ý của tác giả. Chi tiết: [LICENSE](LICENSE).
