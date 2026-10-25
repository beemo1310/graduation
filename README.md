# Thư mời Lễ Tốt Nghiệp – Trần Khánh Linh

Trang tĩnh (HTML/CSS/JS thuần), không cần build.

```
thiep-tot-nghiep/
├── index.html
├── README.md
└── assets/
    ├── logo.png, hero.jpg
    ├── img/     (12 ảnh kỷ niệm)
    └── video/   (2 video + ảnh poster)
```

## Deploy

**GitHub Pages**: tạo repo mới, upload *toàn bộ nội dung* thư mục (index.html nằm ở gốc repo) →
Settings → Pages → Branch `main` / `(root)` → Save. Sau ~1 phút có link dạng `https://<user>.github.io/<repo>/`.

**Netlify Drop** (nhanh nhất): vào app.netlify.com/drop rồi kéo thả cả thư mục vào.

**Cloudflare Pages**: Create project → Direct Upload → kéo thả thư mục.

Có thể mở thử ngay trên máy bằng cách bấm đúp `index.html` (cần có mạng để tải font).

## Chỉnh nội dung (mở index.html, tìm bằng Ctrl+F)

- Ngày giờ đếm ngược: `data-date="2026-10-30T11:00:00+07:00"`
- Số Zalo: `0399941082` (2 chỗ: nút và thẻ "Xác nhận tham dự")
- Link chỉ đường: `maps.app.goo.gl/nRGkqAVeqXcGtdjm8`
- Lời thư: tìm `Một lá thư nhỏ`
- Ảnh/video: sửa trong các thẻ `<figure class="pol">` ở mục `Khoảnh khắc`

## Lưu ý

- Trang có `noindex` nên Google sẽ không tìm thấy, chỉ ai có link mới vào được.
- Muốn link gửi qua Zalo/Messenger hiện ảnh xem trước, thêm sau deploy:
  `<meta property="og:image" content="https://<link-trang-của-bạn>/assets/hero.jpg">`
