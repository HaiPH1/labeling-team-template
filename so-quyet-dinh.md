# Sổ quyết định

Ghi lại những gì đội đã chốt, và **vì sao**. Ba tuần sau không ai còn nhớ vì sao box lại vẽ
kiểu này — người mới vào đội lại càng không.

**Quyết định đã ghi thì không sửa nội dung.** Đổi ý thì ghi một quyết định mới, và chuyển
trạng thái quyết định cũ thành *Bị thay bởi QĐ-xxx*. Nhờ vậy vẫn truy được vì sao các job
cũ được gán theo cách cũ.

## Danh sách

| Mã | Quyết định | Ngày | Xuất phát từ | Trạng thái |
|---|---|---|---|---|
| [QĐ-001](#qđ-001) | Segmentation: xe đứng dày đặc, sát nhau thì tô chung thành một mảng | 19/09/2026 | [P-001](problem-backlog.md#p-001) | Hiệu lực |
| [QĐ-002](#qđ-002) | Segmentation: vùng không xác định được class (vd. vùng đen) thì không tô, để trống | 19/09/2026 | [P-002](problem-backlog.md#p-002) | Hiệu lực |

**Trạng thái:** ⏳ Chờ chốt (bản nháp, còn sửa được) · Hiệu lực · Bị thay bởi QĐ-xxx · Huỷ (ghi lý do)

---

## QĐ-001

**Segmentation: xe đứng dày đặc, sát nhau thì tô chung thành một mảng**

- **Ngày:** 19/09/2026
- **Người tham gia:** Phạm Hữu Hải (@HaiPH1) (chốt)
- **Xuất phát từ:** [P-001](problem-backlog.md#p-001) · ảnh `w1/segmentation/G06/G06_S002.jpg`
- **Bối cảnh:** Nhiều xe đứng sát nhau, chồng lên nhau theo phối cảnh. Guideline §1 nói semantic
  không tách instance, §3 nói pixel thuộc object phía trước, nhưng không nói có phải bám biên từng
  xe, khe hở nhỏ giữa các xe xử lý thế nào, và xe ở xa quá nhỏ thì làm gì. Đã tạo Issue để hỏi.
- **Các phương án đã cân nhắc:**
  1. *Tô gộp cả cụm xe cùng class thành một vùng, bỏ qua khe hở nhỏ* — nhanh, đúng tinh thần semantic;
     nhưng lấy thừa background ở khe hở. **Chọn.**
  2. *Bám biên từng xe, khe hở thấy mặt đường thì tô `road`* — boundary chính xác; nhưng tốn thời gian. Loại.
  3. *Xe ở xa quá nhỏ để phân biệt `car` / `truck` / `bus` thì không đoán, đưa review* — theo §3, §4.
     Không thuộc phạm vi quyết định này.
- **Quyết định:** Cụm xe đứng dày đặc, sát nhau được tô chung thành **một mảng**, không cần bám biên
  từng xe.
- **Việc phải làm theo:**
  - [x] Chốt phương án (@HaiPH1)
  - [ ] Báo cả đội phần Segmentation
  - [ ] Rà lại các ảnh đã tô tách từng xe
- **Trạng thái:** Hiệu lực

## QĐ-002

**Segmentation: vùng không xác định được class (vd. vùng đen) thì không tô, để trống**

- **Ngày:** 19/09/2026
- **Người tham gia:** Phạm Hữu Hải (@HaiPH1) (chốt)
- **Xuất phát từ:** [P-002](problem-backlog.md#p-002) · ảnh `w1/segmentation/G06/G06_S002.jpg`
- **Bối cảnh:** Có vùng trong ảnh (ví dụ một vùng đen) không thuộc được class nào trong 19 class.
  Guideline §1 RULE 03 cấm ép vào class gần giống, §6 chỉ cho dùng label ignore/unlabeled nếu batch
  có cấu hình — chưa rõ batch này có không. Đã tạo Issue để hỏi.
- **Các phương án đã cân nhắc:**
  1. *Để trống, không gán class* — đúng RULE 03 (không ép vào class gần giống); nhưng ảnh không phủ kín. **Chọn.**
  2. *Gán label ignore/unlabeled* — rõ ràng nhất; chỉ làm được nếu batch có cấu hình label này. Loại.
  3. *Gán theo vùng xung quanh (vd. vùng đen giữa mặt đường → `road`)* — phủ kín ảnh; nhưng dễ thành
     đoán, trái RULE 03. Loại.
- **Quyết định:** Vùng không xác định được thuộc class nào (ví dụ vùng đen) thì **không tô, để trống**.
- **Việc phải làm theo:**
  - [x] Chốt phương án (@HaiPH1)
  - [ ] Báo cả đội phần Segmentation
  - [ ] Rà lại các ảnh đã tô vùng đen bằng class khác
- **Trạng thái:** Hiệu lực

---

## Mẫu để copy

```markdown
## QĐ-NNN

**Quyết định trong một dòng**

- **Ngày:** dd/mm/yyyy
- **Người tham gia:** @ (chốt), @, @
- **Xuất phát từ:** [P-NNN](problem-backlog.md#p-nnn) | Họp tuần NN | …
- **Bối cảnh:** vì sao phải quyết định
- **Các phương án đã cân nhắc:**
  1. *Phương án* — ưu / nhược. Loại hoặc **Chọn.**
  2. *Phương án* — ưu / nhược. Loại hoặc **Chọn.**
- **Quyết định:** đủ rõ để người không dự họp vẫn làm đúng
- **Việc phải làm theo:**
  - [ ] việc (@người phụ trách)
- **Trạng thái:** Hiệu lực
```

Nhớ thêm một dòng vào bảng **Danh sách** ở đầu file, và đóng mục P-xxx tương ứng trong backlog.
