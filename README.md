# Báo Giá Liluca

Tool tạo báo giá (quotation) cho **Liluca Flowers** — static HTML/CSS/JS, không cần backend.

Dựa trên layout của [Lol6888/BAOGIA](https://github.com/Lol6888/BAOGIA), bổ sung tính năng **upload ảnh sản phẩm** cho từng dòng báo giá (phù hợp shop hoa).

## Cách dùng

Mở `index.html` bằng trình duyệt (kéo thả file vào Chrome/Edge), hoặc deploy lên GitHub Pages.

## Tính năng

- Tạo báo giá nhanh, in PDF / xuất PNG
- Quản lý danh sách khách hàng (lưu localStorage)
- **Mỗi dòng sản phẩm có thể đính kèm 1 ảnh** — thumbnail hiển thị cạnh tên sản phẩm trong báo giá
- Hỗ trợ tiền tệ VND / USD / GBP / AUD
- Export / Import dữ liệu dạng JSON (bao gồm ảnh đã upload)
- Thiết kế responsive, in giấy A4 sẵn sàng

## Cấu trúc

```
├── index.html   # Toàn bộ UI + logic
├── style.css    # Tone đen + đỏ-cam (#ff6f61) theo brand Liluca
├── logo.svg     # Logo Liluca (placeholder — thay file thật vào đây)
└── README.md
```

## Thay logo

Thay file `logo.svg` (hoặc thay tham chiếu `<img id="logo" src="...">` trong `index.html`) bằng logo thật của Liluca.

Người dùng cũng có thể upload logo trực tiếp trên giao diện bằng ô **"Logo (tuỳ chọn)"**.

## Mẹo khi in PDF

Trình duyệt mặc định in kèm tiêu đề trang và URL ở mép giấy. Để báo giá in ra **sạch sẽ chuyên nghiệp**:

1. Bấm **"Tải PDF"** trên giao diện
2. Trong hộp thoại in: mở **"More settings"** (Thiết lập khác)
3. **Bỏ check ô "Headers and footers"** (Tiêu đề và chân trang)
4. **Destination:** chọn `Save as PDF`
5. **Margins:** để `Default` (đừng chọn `None`)

## Deploy GitHub Pages

1. Push repo lên GitHub
2. Vào `Settings` → `Pages` → chọn branch `main` / folder `/ (root)`
3. Truy cập `https://<username>.github.io/Baogia-Liluca/`

## Credits

- Layout & flow gốc: [Lol6888/BAOGIA](https://github.com/Lol6888/BAOGIA)
- PNG export: [html2canvas](https://html2canvas.hertzen.com/)
- Font: [Outfit](https://fonts.google.com/specimen/Outfit) + [Dancing Script](https://fonts.google.com/specimen/Dancing+Script)
