# Lab tuần 1 - Website tĩnh

Website này phục vụ yêu cầu Lab tuần 1 môn An toàn điện toán đám mây.

## Cấu trúc

- `index.html`: trang giới thiệu nhóm và nội dung chính.
- `styles.css`: giao diện responsive.
- `_headers`: header bảo mật dùng cho Cloudflare Pages.
- `404.html`: trang lỗi để Cloudflare Pages không hiểu nhầm là SPA.

## Deploy lên Cloudflare Pages

1. Tạo repository GitHub mới.
2. Push mã nguồn lên repository.
3. Vào Cloudflare Pages, chọn **Create a project**.
4. Kết nối GitHub repository.
5. Cấu hình:
   - Framework preset: `None`
   - Build command: để trống
   - Build output directory:
     - `/` nếu repository chỉ chứa các file trong thư mục `website`
     - `website` nếu repository chứa cả thư mục `lab-1`
6. Deploy và ghi lại URL dạng `https://<ten-du-an>.pages.dev`.

Sau khi deploy, kiểm tra:

- Security Headers: https://securityheaders.com
- PageSpeed Insights: https://pagespeed.web.dev
