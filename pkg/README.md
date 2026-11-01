# Sổ Công Thức Bâng Quơ

Ghi liền tên món, xuống dòng là lưu. App tự nhận nguyên liệu, nhắc cách sơ chế,
gợi ý món từ nguyên liệu trong tủ lạnh và nhắc "lưu công thức rồi có nấu không pà?".

App web cài được lên điện thoại (PWA), chạy offline. Dữ liệu lưu ngay trong máy (localStorage).

## Đưa lên GitHub Pages

1. Tạo repo mới trên GitHub (Public), ví dụ `so-cong-thuc`.
2. Upload toàn bộ file trong thư mục này lên repo (kéo thả, nhớ có cả `.nojekyll`).
3. Vào **Settings → Pages**, mục *Build and deployment* chọn **Deploy from a branch**,
   Branch: `main`, thư mục `/ (root)`, bấm **Save**.
4. Chờ 1 đến 2 phút, link sẽ là `https://<tên-github>.github.io/so-cong-thuc/`.

## Cài lên điện thoại

- **iPhone (Safari):** mở link, bấm Chia sẻ, chọn *Thêm vào MH chính*.
- **Android (Chrome):** mở link, bấm ⋮, chọn *Cài đặt ứng dụng* hoặc *Thêm vào màn hình chính*.

## Sao lưu sổ

Tab **Sổ** có nút **Xuất sổ** (tải file `.json`) và **Nhập sổ** để chuyển sang máy khác.

## Cập nhật app

Sửa `index.html`, rồi đổi số phiên bản `CACHE` trong `sw.js` (ví dụ `v2`)
để điện thoại tải bản mới thay vì dùng bản cũ trong bộ nhớ.

## Thêm nguyên liệu

Mở `index.html`, tìm mảng `ING`, thêm một dòng theo mẫu:
`[["tên nhận diện","tên khác"],"Nhãn hiển thị","Cách sơ chế"],`
