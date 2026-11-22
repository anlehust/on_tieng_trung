# on_tieng_trung

Trắc nghiệm từ vựng tiếng Trung (A/B/C/D). Trang: https://anlehust.github.io/on_tieng_trung

## Thêm bài mới (ví dụ bài 5)

1. Tạo `data/tu_vung/bai05.csv`, cùng cột với các file cũ: `Bài,Chữ Hán,Pinyin,Nghĩa,Ví dụ,Ghi chú`.
2. (Tuỳ chọn) Tạo `data/cau_hoi/bai05.json` cho câu ngữ pháp/ngữ cảnh soạn tay:
   ```json
   [
     {"muc": 2, "cau_hoi": "Điền vào chỗ trống: 你忙＿＿？", "dap_an": ["吗","呢","的","们"], "giai_thich": "吗 đặt cuối câu để hỏi có/không."}
   ]
   ```
   `muc`: 1 = dễ, 2 = vừa, 3 = khó. Đáp án đúng luôn là phần tử đầu của `dap_an` (trang tự trộn A/B/C/D).
3. Thêm số `5` vào `data/danh_sach.json`: `{"bai": [1,2,3,4,5]}`.
4. (Tuỳ chọn) Thêm nhóm từ vào `data/nhom_tu.json` cho dạng câu "khác nhóm".
5. Commit và push. Trang cập nhật sau khoảng 1 phút.

Câu hỏi dạng Hán tự/nghĩa/pinyin/điền từ/nghe được sinh tự động từ file CSV.

## Chạy trên máy

Trang tải dữ liệu bằng `fetch`, nên không mở trực tiếp bằng nhấp đúp được. Chạy:

```
python -m http.server
```

rồi mở http://localhost:8000.
