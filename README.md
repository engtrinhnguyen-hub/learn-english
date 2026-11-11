# English Knowledge V1

Ứng dụng tích lũy kiến thức tiếng Anh chạy hoàn toàn trên trình duyệt, tối ưu cho GitHub Pages.

## Tính năng
- Dashboard, thư viện sách, duyệt theo unit và loại kiến thức
- Flashcard chủ động, đánh dấu đã biết/chưa biết
- Ôn tập lặp lại ngắt quãng theo mô hình FSRS-inspired
- Tìm kiếm không dấu, lọc theo book/unit/type/tag
- Ghi chú cá nhân, bookmark, dark mode
- IndexedDB; import/export JSON; dữ liệu không rời thiết bị
- PWA cơ bản, responsive cho điện thoại

## Chạy local
Do trình duyệt chặn `fetch()` khi mở trực tiếp file, dùng:

```bash
python3 -m http.server 8080
```

Mở http://localhost:8080

## Đưa lên GitHub Pages
1. Tạo repository và upload toàn bộ nội dung thư mục này vào nhánh `main`.
2. GitHub > Settings > Pages > Deploy from a branch > `main` / `(root)`.
3. Không cần build và không cần Node.js.

## Thêm sách mới
Tạo JSON theo `docs/DATA_SCHEMA.md`, sau đó vào Settings > Import JSON. Không cần sửa UI.

## Lưu ý bản quyền
Repo chỉ chứa dữ liệu mẫu để kiểm tra hệ thống. Không đưa nguyên văn sách có bản quyền lên repository công khai nếu chưa có quyền phân phối.
