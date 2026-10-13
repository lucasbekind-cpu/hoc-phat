# Nguyễn Thế Đăng — Tuyển Tập Bài Viết

> **Nguồn tra cứu ưu tiên số 1 của dự án** — xem [`AGENTS.md`](../../AGENTS.md).

Tuyển tập **225 bài viết** (khoảng 500.000 từ) của Thầy Nguyễn Thế Đăng đăng trên [Thư Viện Hoa Sen](https://thuvienhoasen.org/author/post/115/1/nguyen-the-dang). Nhiều bài từng in trên *Tạp chí Văn Hóa Phật Giáo*.

## Cách tra cứu

| Muốn… | Dùng |
|---|---|
| Tìm bài theo chủ đề (Phật tánh, Tánh Không, Pháp Hoa, Thiền…) | [`chu-de.md`](chu-de.md) — chỉ mục chủ đề |
| Xem toàn bộ danh sách bài | [`muc-luc.md`](muc-luc.md) — mục lục theo thứ tự chữ cái |
| Tìm theo từ khóa bất kỳ | `grep -ril "từ khóa" tac-gia/nguyen-the-dang/bai-viet/` |
| Đọc một bài | thư mục [`bai-viet/`](bai-viet/) — mỗi bài một tệp |

## Những chủ đề lớn trong tuyển tập

Một số nhận xét ban đầu, rút ra từ chỉ mục chủ đề và các bài đã đọc:

- **Phật tánh – Như Lai tạng** là trục xuyên suốt. Nhiều bài trực tiếp: *Tất Cả Chúng Sanh Đều Có Phật Tánh*, *Tìm Hiểu Phật Tánh Theo Kinh Luận*, *Đều Có Phật Tánh, Tại Sao Phải Tu?*, *Phật Tánh Thường Lạc Ngã Tịnh*, *Thuận Tánh Khởi Tu*…
- **Tánh Không – Bát Nhã** được đọc chung với Phật tánh: Phật tánh là “Chân Không Diệu Hữu”, “Đệ nhất nghĩa Không”.
- **Kinh điển Đại thừa:** Đại Bát Niết-bàn, Pháp Hoa, Hoa Nghiêm, Viên Giác, Lăng Nghiêm, Duy Ma Cật, Lăng Già.
- **Thiền Việt Nam:** Trần Nhân Tông, Trần Thánh Tông, Tuệ Trung, Thường Chiếu, Kiều Trí Huyền, Hương Hải, Thiền Lão, Chân Không…
- **Kim Cang thừa:** Đại Toàn Thiện (*Dzogchen*), Đại Ấn (*Mahamudra*), Padmasambhava; Thầy thường đối chiếu với Thiền tông.
- **Đời sống và xã hội:** giới, đạo đức, giáo dục, văn hóa, thanh niên, môi trường; và loạt bài **Xuân** dùng hình ảnh mùa xuân để nói về thực tại bất sanh bất diệt.

## Định dạng mỗi bài

```yaml
---
tieu_de: "Tất Cả Chúng Sanh Đều Có Phật Tánh"
tac_gia: Nguyễn Thế Đăng
nguon: Thư Viện Hoa Sen (thuvienhoasen.org)
chu_de: [Phật tánh – Như Lai tạng, Tánh Không – Bát Nhã, ...]   # gắn tự động theo từ khóa
dang_tai: "Tạp chí Văn Hóa Phật Giáo số 173"                      # nếu bài có ghi
url: https://thuvienhoasen.org/...                               # nếu tìm được đường dẫn gốc
---
```

## Ghi chú biên tập

- **Nguồn dữ liệu:** 5 tệp tổng hợp (255 mục) do người dùng cung cấp, chép từ Thư Viện Hoa Sen.
- **Loại bản trùng:** các mục có cùng tiêu đề hoặc cùng đoạn mở đầu được gộp lại, giữ bản đầy đủ nhất. Còn **225 bài**.
- **Nội dung bài giữ nguyên**, chỉ bỏ ảnh nhúng dạng base64 và các dòng siêu dữ liệu bị lặp. Lỗi chính tả trong bản gốc (ví dụ “sẳn”) được giữ nguyên.
- Bài *Hạnh Bồ-tát Trong Kinh Xuất Hiện Quang Minh* chỉ có bản hình ảnh, **chưa có văn bản**.
- Bài *Nguyện Cho Người Khác Được Hạnh Phúc* thiếu tiêu đề trong bản gốc; tiêu đề hiện tại do người biên tập đặt theo nội dung.
- **Chỉ mục chủ đề được gắn tự động** bằng từ khóa, nên có thể sót hoặc gắn nhầm; cần hiệu đính dần khi đọc.
- Chỉ khoảng 1/10 số bài có đường dẫn gốc (`url`), và gần một nửa có thông tin đăng tải (`dang_tai`). Có thể bổ sung dần khi tra lại trên Thư Viện Hoa Sen.
