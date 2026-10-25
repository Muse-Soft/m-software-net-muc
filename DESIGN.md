# DESIGN.md — Landing page studio xăm nghệ thuật Nét Mực (MSR-35)

Quyết định thiết kế DỨT KHOÁT cho 1 landing page. Dev và QA đối chiếu đúng tài liệu này;
mọi thông số dưới đây là bắt buộc, không dùng từ chung chung thay cho số liệu.

## 1. Tổng quan sản phẩm

- Sản phẩm: landing page 1 trang cho studio xăm nghệ thuật **Nét Mực** (TP.HCM).
- Chuyên môn: blackwork, fine-line, dotwork.
- Phạm vi: đúng 1 landing page, không giỏ hàng, không thanh toán online, không đặt lịch
  tự động — form đặt lịch chỉ là giao diện (xem §6).
- Ưu tiên visual-first (OPERATIONS.md §16.1): ảnh là nội dung chính, bố cục ảnh lớn +
  khoảng trắng, không nhồi chữ.

## 2. Bảng màu (đúng 5 màu, không thêm màu ngoài danh sách)

| Mã hex | Vai trò |
| --- | --- |
| `#F3EDE3` | Nền chính toàn trang — kem giấy, ấm, hơi ngả vàng như giấy vẽ phác thảo |
| `#E9E0CE` | Nền khối phụ — kem đậm hơn, dùng cho section xen kẽ và thẻ quy trình |
| `#161412` | Chữ chính + viền đậm — mực đen, dùng cho tiêu đề, nội dung, đường kẻ |
| `#6E675E` | Chữ phụ — xám nâu, dùng cho chú thích, giá phụ, ngày/giờ mẫu |
| `#A63D2F` | Nhấn duy nhất — đỏ gạch, CHỈ dùng cho: nút CTA chính, dấu nhấn tiêu đề, gạch dưới link khi hover. Không dùng đỏ gạch làm nền khối lớn |

Quy tắc: nền sáng chiếm đa số diện tích; mực đen làm khung và chữ; đỏ gạch là điểm
nhấn hiếm, không quá 10% diện tích nhìn thấy của một màn hình.

## 3. Font chữ (đúng 2 font, không thêm font khác)

- Tiêu đề: **Cormorant Garamond** (serif, có chân, nét mảnh — hợp phong cách tạp chí).
- Nội dung: **Be Vietnam Pro** (sans-serif, đọc rõ tiếng Việt có dấu).
- Cỡ chữ desktop: H1 hero 64px / H2 section 40px / H3 24px / body 17px, line-height 1.6.
- Cỡ chữ mobile: H1 40px / H2 30px / H3 20px / body 16px, line-height 1.6.
- Breakpoint duy nhất: 768px (dưới 768px = bố cục 1 cột, ảnh xếp dọc).

## 4. Phong cách tham chiếu (MỘT phong cách duy nhất)

**Blackwork tối giản kiểu tạp chí tattoo châu Âu** — trang giấy kem, ảnh đen trắng
tương phản cao chiếm diện tích lớn, tiêu đề serif khổ lớn, khoảng trắng rộng, không
màu mè, không icon trang trí, không khung bo tròn bóng đổ kiểu sàn thương mại điện tử.

## 5. Quy tắc hình ảnh

- Toàn bộ ảnh là **ảnh mẫu** (chưa phải ảnh thật của studio), ghi rõ là ảnh mẫu trong
  comment kết quả của Dev — tuyệt đối không ghi là ảnh thật.
- Tông ảnh: đen trắng, tương phản cao, nền sáng, chi tiết mực rõ nét; cấm ảnh màu
  rực, ảnh sáng phẳng kiểu sàn thương mại điện tử.
- Tỉ lệ khung bắt buộc:
  - Hero: 16:9, toàn màn hình (100vh), 1 ảnh lớn duy nhất (tay xăm đang làm việc
    hoặc lưng/vai có hình xăm blackwork lớn).
  - Giới thiệu studio/nghệ sĩ: ảnh chân dung 3:4.
  - Bộ sưu tập: mỗi tác phẩm 4:5, xếp lưới lệch (editorial, không đều tăm tắp).
  - Quy trình: không dùng ảnh, chỉ dùng số La Mã lớn (I–IV) làm điểm nhấn thị giác.
- Số lượng ảnh mẫu: hero 1 + studio/nghệ sĩ 2 + bộ sưu tập 6 (2 blackwork, 2 fine-line,
  2 dotwork) = 9 ảnh, tất cả đồng tông đen trắng.

## 6. Bố cục trang (đúng 6 section, đúng thứ tự)

1. **Hero** — ảnh lớn toàn màn hình 16:9, tên studio "Nét Mực" serif 64px chồng lên ảnh,
   dòng phụ "Studio xăm nghệ thuật — TP.HCM", nút CTA đỏ gạch "Đặt lịch tư vấn".
2. **Giới thiệu studio và nghệ sĩ** — 2 cột desktop (chữ trái, ảnh 3:4 phải): triết lý
   làm việc (ít hình, kỹ, bền màu), giới thiệu nghệ sĩ chính. Tên nghệ sĩ thật,
   địa chỉ, điện thoại = **[CẦN BỔ SUNG]**, không bịa.
3. **Bộ sưu tập theo phong cách** — 3 nhóm: Blackwork / Fine-line / Dotwork, mỗi nhóm
   2 tác phẩm 4:5, tên tác phẩm mẫu + kích thước mẫu (ví dụ "10 × 15 cm — mẫu").
4. **Quy trình 4 bước** — I. Tư vấn ý tưởng → II. Phác thảo & chốt mẫu → III. Xăm
   (vệ sinh an toàn, kim dùng 1 lần) → IV. Chăm sóc sau xăm. Mỗi bước: số La Mã lớn
   + tiêu đề + 1–2 câu mô tả ngắn.
5. **Bảng giá mẫu** — ghi rõ toàn bộ là **giá mẫu**, chưa phải giá thật:
   hình nhỏ fine-line từ 1.500.000đ, hình vừa blackwork từ 3.500.000đ,
   hình lớn/dotwork theo giờ tư vấn. Giá thật = [CẦN BỔ SUNG].
6. **Form đặt lịch tư vấn (CHỈ giao diện)** — các trường: họ tên, số điện thoại,
   phong cách quan tâm (Blackwork / Fine-line / Dotwork), kích thước mong muốn,
   mô tả ý tưởng. Nút "Gửi yêu cầu tư vấn" chỉ hiển thị, không gửi dữ liệu đi thật
   (preventDefault, không backend, không lưu trữ). Ghi chú dưới form: "Form hiện chỉ
   nhận thông tin hiển thị — chưa gửi đi thật."

## 7. Điều cấm

- Cấm template bán hàng phổ thông, lưới thẻ đều tăm tắp, icon stock, ảnh màu sáng
  phẳng kiểu sàn thương mại điện tử.
- Cấm nút "mua ngay", giỏ hàng, thanh toán online.
- Cấm thêm màu, font, section ngoài danh sách §2, §3, §6.
- Cấm bịa tên nghệ sĩ thật, địa chỉ thật, số điện thoại thật, giá thật — mọi dữ liệu
  thật chưa có đều ghi [CẦN BỔ SUNG].

## 8. Nguồn

- Task: TEC-270 (Epic TEC-269, yêu cầu web MSR-35).
- Repo: https://github.com/Muse-Soft/m-software-net-muc
