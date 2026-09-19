# Nhật ký tuần 01 · 15/09 – 21/09/2026

**Lead tuần này:** Phạm Hữu Hải (2A202602098) — phần BBox_Polygon_Polyline · lead phần Segmentation: *(chưa ghi tên)*
**Dữ liệu / task CVAT:** Ảnh 2D camera hành trình trên đường phố (có cả cảnh đêm), gồm 2 phần:
- **BBox_Polygon_Polyline:** 4 job × 25 frame
- **Segmentation:** 4 job × 25 ảnh

## Thành viên và phân công

| Thành viên | Vị trí | BBox_Polygon_Polyline | Segmentation |
|---|---|---|---|
| Phạm Hữu Hải (2A202602098) | Lead · Annotator · Reviewer | Gán 1497 **(nhận lại từ Dũng, 19/09)**; review 1494 | Gán 1710 |
| Nguyễn Hữu Dũng (2A202602153) | Annotator · Reviewer | ~~Gán 1497~~ → chuyển cho Hải (19/09) | ~~Gán 1713; review 1710~~ — 1713 tạm chưa ai làm, review 1710 chuyển cho Mạnh (19/09) |
| Nguyễn Hùng Mạnh (2A202602062) | Annotator · Reviewer | Gán 1496; review 1497 | Gán 1712; review 1710 **(thay Dũng, 19/09)** |
| Nguyễn Tuấn Khôi (2A202602241) | Annotator · Reviewer | Gán 1495; review 1496 | Gán 1711; review 1712 |
| Vũ Tiến Thắng (2A202602087) | Annotator · Reviewer | Gán 1494; review 1495 | Review 1711 |

Tuần này **review chéo** (tạm thời): không ai review job do chính mình gán. Reviewer của từng job
ghi trong bảng Công việc.

**Thay đổi 19/09:** Dũng không liên lạc được nên rút khỏi phân công. Job BBox 1497 chuyển cho Hải gán
(Mạnh vẫn review); review job Seg 1710 chuyển từ Dũng sang Mạnh; job Seg 1713 tạm chưa ai làm.

## Công việc

Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

### BBox_Polygon_Polyline

| # | Nội dung công việc | Annotator | Reviewer | Hoàn thành | Ghi chú |
|---|---|---|---|---|---|
| 1 | Job 1497 — 25 frame, 2D | ~~Nguyễn Hữu Dũng~~ → Phạm Hữu Hải | Nguyễn Hùng Mạnh | 🟡 100% | Gán xong, chờ review. Ban đầu giao Dũng. Dũng không có trong nhóm Discord, liên hệ riêng không phản hồi, đã báo cáo BTC → 19/09 chuyển cho Hải |
| 2 | Job 1496 — 25 frame, 2D | Nguyễn Hùng Mạnh | Nguyễn Tuấn Khôi | 🟡 30% | Đang gán |
| 3 | Job 1495 — 25 frame, 2D | Nguyễn Tuấn Khôi | Vũ Tiến Thắng | 🟡 50% | Đang gán |
| 4 | Job 1494 — 25 frame, 2D | Vũ Tiến Thắng | Phạm Hữu Hải | 🟡 60% | Đang gán |

### Segmentation

| # | Nội dung công việc | Annotator | Reviewer | Hoàn thành | Ghi chú |
|---|---|---|---|---|---|
| 1 | Job 1710 — 25 ảnh | Phạm Hữu Hải | ~~Nguyễn Hữu Dũng~~ → Nguyễn Hùng Mạnh | 🟡 100% | Gán xong, chờ review. Trước ghi nhầm sang BBox. 19/09 đổi reviewer từ Dũng sang Mạnh |
| 2 | Job 1711 — 25 ảnh | Nguyễn Tuấn Khôi | Vũ Tiến Thắng | 🟡 % | |
| 3 | Job 1712 — 25 ảnh | Nguyễn Hùng Mạnh | Nguyễn Tuấn Khôi | 🟡 % | |
| 4 | Job 1713 — 25 ảnh | ~~Nguyễn Hữu Dũng~~ → *(chưa ai nhận)* | — | ⬜ 0% | Giao Dũng nhưng Dũng không liên lạc được; tạm thời chưa ai làm |

## Tổng kết

Tính riêng từng phần, không cộng chung.

| Phần | Đã gán | Qua review lần đầu |
|---|---|---|
| BBox_Polygon_Polyline | ~60 / 100 frame (60%) | Chưa review chéo |
| Segmentation | Chưa đủ số (thiếu % job 1711, 1712) / 100 ảnh | Chưa review chéo |

- Edge case mới: [P-001](../problem-backlog.md#p-001) (xe đứng dày đặc), [P-002](../problem-backlog.md#p-002) (vùng không xác định được class) — cả hai thuộc Segmentation, đã tạo Issue, chờ trả lời
- Edge case đã chốt: Chưa có — nháp [QĐ-001](../so-quyet-dinh.md#qđ-001), [QĐ-002](../so-quyet-dinh.md#qđ-002) chờ chốt

## Vướng mắc

- **Chưa liên hệ được 1 thành viên** (Nguyễn Hữu Dũng): không có trong nhóm Discord, liên hệ riêng
  chưa phản hồi, đã báo BTC. Ngày 19/09 đã chuyển job 1497 cho Hải, review job 1710 cho Mạnh.
- **Team có 2 lead, mỗi lead chỉ thấy một phần:** lead 1 chỉ thấy `bbox_polygon`, lead 2 chỉ thấy
  segmentation. Khó tổng hợp tiến độ, edge case và quyết định chung của cả đội.
- **P-001, P-002 chưa có câu trả lời** nên chưa chốt được cách tô xe dày đặc và vùng không xác định
  class. Các ảnh gặp hai trường hợp này có thể phải sửa lại sau khi chốt.

## Kế hoạch tuần 02

**Tiến độ**
- BBox: đưa 1496, 1495, 1494 lên 100%. Seg: đưa 1711, 1712 lên 100%. Job 1497, 1710 của Hải đã gán xong. Xong job nào thì review chéo job đó.
- Tìm người nhận job Seg 1713.
- Mỗi reviewer ghi số ảnh bị trả lại để điền "Qua review lần đầu".

**Thành viên chưa liên hệ được**
- ✅ Đã chuyển job 1497 cho Hải, review job 1710 cho Mạnh (19/09).
- Cập nhật assignee job 1497 trên CVAT sang Hải.
- Nếu Dũng liên lạc lại: báo BTC, lead xếp việc mới cho Dũng (không lấy lại job 1497).

**Phối hợp 2 lead**
- Dùng chung repo này làm nơi tổng hợp: cả 2 lead cùng cập nhật nhật ký tuần, backlog và sổ quyết định.
- ✅ Tách bảng Công việc và Tổng kết thành 2 phần BBox_Polygon_Polyline / Segmentation (19/09).
- Ghi rõ mỗi mục P / QĐ áp dụng cho phần nào.
- Hẹn 2 lead trao đổi ngắn mỗi cuối tuần trước khi chốt nhật ký.

**Edge case**
- Theo dõi Issue của P-001, P-002. Có câu trả lời thì chốt QĐ-001, QĐ-002 và báo cả đội.
- Rà lại các ảnh đã gặp hai trường hợp này sau khi chốt.

**Hoàn thiện repo**
- Thu handle GitHub của các thành viên để thay cho mã sinh viên.
- Bổ sung link CVAT (job + frame) cho P-001, P-002 và task của tuần.
