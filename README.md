# NÀNG THÍCH GÌ, CHÀNG NHỚ ĐÓ — The Gift Reveal Minigame

Dashboard minigame 20/10 cho SEM JSC / BETMA ENGLISH. Web tĩnh (HTML/CSS/JS thuần), không cần backend.

## Cấu trúc
```
index.html          # toàn bộ ứng dụng
assets/bgm.mp3      # nhạc nền (thay file này để đổi bài)
mau-dap-an.csv      # file đáp án mẫu (2 cột: Cau, Dap an)
.nojekyll
```

## Chạy thử trên máy
Mở `index.html` bằng Chrome/Edge. (Lần đầu cần internet để tải font và thư viện đọc XLSX.)

## Đưa lên GitHub Pages
1. Tạo repository mới trên GitHub, upload toàn bộ file trong thư mục này (kéo thả trên web hoặc `git push`).
2. Vào **Settings → Pages**.
3. Mục **Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, thư mục `/ (root)`, bấm **Save**.
4. Chờ 1–2 phút, trang chạy tại `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

## Chuẩn bị dữ liệu trước chương trình
1. **① Ảnh GÓC**: 10 ảnh crop làm câu hỏi. Đặt tên có số, ví dụ `goc_01.jpg` … `goc_10.jpg`.
2. **② Ảnh ĐẦY ĐỦ**: 10 ảnh nguyên sản phẩm, lật ra khi công bố đáp án, ví dụ `full_01.jpg` … `full_10.jpg`.
3. **③ File đáp án**: XLSX / CSV / JSON, hai cột `Câu | Đáp án` (xem `mau-dap-an.csv`).
4. Kiểm tra từng câu, sửa nếu cần, rồi bấm **BẮT ĐẦU GAME**.

Ảnh, đáp án và tiến độ được lưu trong trình duyệt của máy vận hành: dùng đúng một máy, một trình duyệt suốt chương trình. Ảnh và đáp án **không** được đưa lên GitHub.

## Điều khiển MC
- Chọn hộp → **MỞ QUÀ** → **BẮT ĐẦU 30 GIÂY** → **KẾT THÚC LƯỢT** (hoặc chờ hết giờ) → **CÔNG BỐ ĐÁP ÁN** → chấm điểm 0/5/10 cho từng đội → **HOÀN THÀNH CÂU**.
- Phím tắt: `Space` bắt đầu/tạm dừng/tiếp tục đồng hồ · `H` ẩn/hiện bảng điều khiển · `M` bật/tắt nhạc.
- Không có countdown, công bố đáp án hay chấm điểm tự động.
- Nhạc và hiệu ứng: thanh nhỏ góc dưới bên trái (nhạc phải do MC bấm bật).

## Lưu ý bản quyền
`assets/bgm.mp3` là bài hát có bản quyền. Hãy chắc chắn bạn có quyền sử dụng, hoặc thay bằng nhạc khác trước khi công khai repository.
