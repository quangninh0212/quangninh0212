# HƯỚNG DẪN ĐĂNG GITHUB PROFILE — ANIME / PIXEL EDITION

## 1. Thư mục cần upload

```text
quangninh0212/
├── README.md
├── assets/
│   ├── banner.svg
│   ├── fraud.svg
│   ├── smart-parking.svg
│   ├── travel.svg
│   ├── jobs.svg
│   └── film.svg
└── .github/
    └── workflows/
        └── snake.yml
```

`HUONG_DAN.md` chỉ là hướng dẫn, không cần upload.

## 2. Tạo repository đặc biệt để hiện profile

1. Đăng nhập **github.com/quangninh0212**, không đăng bằng tài khoản GitHub khác.
2. Mở https://github.com/new
3. Repository name **quangninh0212** (trùng CHÍNH XÁC username), chọn **Public**.
4. Có thể chọn **Add a README** hoặc không. Nếu đã chọn, bạn sẽ thay README bằng file này.
5. Vào repo > **Add file** > **Upload files**, upload thư mục con theo đúng cấu trúc hoặc dùng Git (bên dưới).
6. Vào https://github.com/quangninh0212 xem profile hiện lên.

**Cách upload an toàn trên Windows (PowerShell / Git Bash) khi đã tạo repo trống:**

```bash
git clone https://github.com/quangninh0212/quangninh0212.git
cd quangninh0212
# chép README.md, assets/ và .github/ từ ZIP này vào thư mục repo
git add README.md assets .github
git commit -m "feat: add anime pixel GitHub profile"
git push origin main
```

Nếu repository đã có README, nên backup trước khi thay.

## 3. Bật hiệu ứng con rắn

- Mở repo **quangninh0212** > **Settings > Actions > General**.
- Đảm bảo Actions được bật và GitHub Actions được phép ghi nội dung khi cần. Nếu workflow báo lỗi 403, xem **Workflow permissions** và chọn **Read and write permissions**; cần quyền phù hợp.
- Mở tab **Actions** > **Generate contribution snake** > **Run workflow**.
- Sau khi workflow thành công, nhánh `output` sẽ chứa 2 file snake SVG. README đã cấu hình sẵn. Nếu hình chưa hiện, thử tải lại trang sau khi nhánh xuất hiện.

## 4. Chỉnh sửa nội dung

- Tên, email, Facebook, trường học, GPA và học bổng được điền từ thông tin bạn cung cấp.
- 2 dự án Travel & 28.ITJobs chưa có GitHub repo: KHÔNG gắn nhầm vào repo `project-1`, `project-2` đang hiện diện công khai.
- KMA.Film cũng chưa được gắn repo công khai; khi có link, thay tên hoặc ảnh thành link.
- Hình minh họa các dự án là **pixel-art mang tính biểu tượng**, không phải screenshot từ các ứng dụng.
- `README.md` dùng ảnh SVG nội bộ (ổn định), nhưng chữ chạy / badge / biểu đồ phụ thuộc dịch vụ công khai và có thể bị chặn / giới hạn request.

## 5. Lưu ý với Smart Parking

Repository `smart-parking` hiện có `parking.db` và một đoạn code đăng nhập mặc định. Bạn nên kiểm tra dữ liệu thực, credential và lịch sử commit trước khi chia sẻ rộng rãi. Điều này không ảnh hưởng việc làm profile; nó là việc nên cải thiện riêng ở repo đó.

## 6. Quy ước minh bạch dự án

- Không khai kinh nghiệm đi làm nếu chưa có.
- Không mô tả vibe-coded Unity / KMA.Film như bằng chứng năng lực game hoặc media chuyên sâu.
- Nhóm học online không tự nhận là sản phẩm thương mại.
- FraudDetection mô tả là đồ án đang phát triển, có Codex hỗ trợ và bạn đang học sâu để bảo vệ.
