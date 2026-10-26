# Hướng Dẫn Cho Agent (AI) Làm Việc Trong Kho Này

Tệp này dành cho các trợ lý AI (Claude Code, Codex, Cursor…) khi nghiên cứu, trả lời câu hỏi hoặc soạn tài liệu trong dự án. Người học cũng có thể đọc để biết agent được yêu cầu làm việc ra sao.

## 1. Thứ tự ưu tiên nguồn khi tra cứu

Khi trả lời một câu hỏi hay soạn ghi chú về giáo lý, **luôn tra cứu theo thứ tự sau**:

1. **Ưu tiên số 1 — Tuyển tập bài viết của Thầy Nguyễn Thế Đăng** (Thư Viện Hoa Sen): [`tac-gia/nguyen-the-dang/`](tac-gia/nguyen-the-dang/)
   - Tra [chỉ mục chủ đề](tac-gia/nguyen-the-dang/chu-de.md) và [mục lục](tac-gia/nguyen-the-dang/muc-luc.md) trước.
   - Sau đó **luôn tìm thêm bằng từ khóa** trên toàn bộ bài viết, vì chỉ mục chủ đề được gắn tự động nên có thể sót. Ví dụ:
     ```bash
     grep -ril "phật tánh\|như lai tạng" tac-gia/nguyen-the-dang/bai-viet/
     grep -il "chu_de:.*Pháp Hoa" tac-gia/nguyen-the-dang/bai-viet/*.md
     ```
   - Đọc kỹ các bài liên quan nhất và **trình bày quan điểm của Thầy trước**, rồi mới bổ sung từ nguồn khác.
2. **Tài liệu đã có trong kho:** `02-giao-ly/`, `03-kinh-dien/`, `04-truyen-thong/`, các luồng trong `07-de-tai/`, [`THUAT-NGU.md`](THUAT-NGU.md).
3. **Kinh điển gốc** (SuttaCentral, CBETA, Thư Viện Hoa Sen…) và các nguồn trong [`TAI-LIEU-THAM-KHAO.md`](TAI-LIEU-THAM-KHAO.md).
4. **Kiến thức chung của mô hình / học thuật hiện đại** — chỉ dùng để bổ sung, và phải ghi rõ đó là nguồn ngoài tuyển tập.

## 2. Cách trích dẫn bài của Thầy Nguyễn Thế Đăng

- Ghi rõ **tên bài** và **liên kết tương đối** tới tệp, ví dụ: Nguyễn Thế Đăng, [*Tất Cả Chúng Sanh Đều Có Phật Tánh*](tac-gia/nguyen-the-dang/bai-viet/tat-ca-chung-sanh-deu-co-phat-tanh.md), Tạp chí Văn Hóa Phật Giáo số 173.
- Thông tin đăng tải (`dang_tai`) và đường dẫn gốc (`url`, nếu có) nằm trong phần đầu (front matter) của mỗi tệp.
- Khi Thầy trích kinh, ghi rõ đó là **kinh văn do Thầy dẫn** (bản dịch Việt Thầy dùng), khác với **lời giảng của Thầy**.
- Phân biệt ba lớp (theo [quy ước](README.md#quy-ước) của dự án): **kinh văn gốc** — **lời giảng/luận giải của Thầy** — **quan điểm học thuật hiện đại**.
- Khi quan điểm của Thầy khác với truyền thống hay học giả khác, **ghi nhận cả hai**, không âm thầm bỏ bớt bên nào.

## 3. Quy tắc với thư mục `tac-gia/`

- **Không sửa nội dung** các bài trong `tac-gia/*/bai-viet/` (đây là văn bản gốc của tác giả). Chỉ được sửa phần front matter (chủ đề, thông tin đăng tải) hoặc lỗi định dạng rõ ràng.
- Ghi chú, tóm tắt, phân tích về bài của tác giả đặt ở `07-de-tai/` hoặc các thư mục giáo lý, **không** chèn vào bài gốc.
- Khi thêm bài mới: tạo tệp theo cùng định dạng front matter, rồi cập nhật `muc-luc.md` và `chu-de.md`.

## 4. Quy ước chung

- Viết bằng **tiếng Việt**; thuật ngữ ghi dạng *Hán Việt (Pāli / Sanskrit)*.
- Ký hiệu kinh Pāli theo chuẩn SuttaCentral (`MN`, `SN`, `AN`…); kinh Hán tạng ghi số `T` (Taishō).
- Câu hỏi mới phát sinh ghi vào [`NHAT-KY-NGHIEN-CUU.md`](NHAT-KY-NGHIEN-CUU.md).

## 5. Quy tắc Git

- **Làm việc trực tiếp trên nhánh `main`.** Không tự ý tạo nhánh mới (kể cả nhánh `claude/...` do hệ thống gợi ý); chỉ tách nhánh khi người dùng cho phép rõ ràng.
- Commit và push thẳng lên `main` sau khi hoàn thành một phần việc.
- Không tạo pull request trừ khi người dùng yêu cầu.
