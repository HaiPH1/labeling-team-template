# Nhật ký tuần 01 · 15/09 – 21/09/2026

**Lead tuần này:** Phạm Hữu Hải (2A202602098) — phần BBox_Polygon_Polyline · lead phần Segmentation: *(chưa ghi tên)*
**Dữ liệu / task CVAT:** Ảnh 2D camera hành trình trên đường phố (có cả cảnh đêm), gồm 2 phần:
- **BBox_Polygon_Polyline:** 4 job × 25 frame
- **Segmentation:** 4 job × 25 ảnh

## Thành viên và phân công

| Thành viên | Vị trí | BBox_Polygon_Polyline | Segmentation |
|---|---|---|---|
| Phạm Hữu Hải (2A202602098) | Lead · Annotator · Reviewer | Gán 1497 **(nhận lại từ Dũng, 19/09)**; review 1494 | Gán 1710 |
| Nguyễn Hữu Dũng (2A202602153) | Annotator · Reviewer | ~~Gán 1497~~ → chuyển cho Hải (19/09) | Gán 1713 **(vào làm lại 20/09)**; review 1710 |
| Nguyễn Hùng Mạnh (2A202602062) | Annotator · Reviewer | Gán 1496; review 1497 | Gán 1712; review 1713 |
| Nguyễn Tuấn Khôi (2A202602241) | Annotator · Reviewer | Gán 1495; review 1496 | Gán 1711; review 1712 |
| Vũ Tiến Thăng (2A202602087) | Annotator · Reviewer | Gán 1494; review 1495 | Review 1711 |

Tuần này **review chéo** (tạm thời): không ai review job do chính mình gán. Reviewer của từng job
ghi trong bảng Công việc.

**Thay đổi 19/09:** Dũng không liên lạc được nên rút khỏi phân công. Job BBox 1497 chuyển cho Hải gán
(Mạnh vẫn review); review job Seg 1710 chuyển từ Dũng sang Mạnh; job Seg 1713 tạm chưa ai làm.

**Thay đổi 20/09:** Dũng vào làm lại và gán xong job Seg 1713. Review job Seg 1710 trả lại cho Dũng
như phân công ban đầu; job Seg 1713 do Mạnh review. Job BBox 1497 vẫn giữ ở Hải.

## Công việc

Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

### BBox_Polygon_Polyline

| # | Nội dung công việc | Annotator | Reviewer | Hoàn thành | Ghi chú |
|---|---|---|---|---|---|
| 1 | Job 1497 — 25 frame, 2D | ~~Nguyễn Hữu Dũng~~ → Phạm Hữu Hải | Nguyễn Hùng Mạnh | ✅ 100% | Review lần 1 trả lại (rejected), Hải sửa, review lại đã qua. Ban đầu giao Dũng. Dũng không có trong nhóm Discord, liên hệ riêng không phản hồi, đã báo cáo BTC → 19/09 chuyển cho Hải |
| 2 | Job 1496 — 25 frame, 2D | Nguyễn Hùng Mạnh | Nguyễn Tuấn Khôi | ✅ 100% | Review lần 1 trả lại (rejected), Mạnh sửa, review lại đã qua |
| 3 | Job 1495 — 25 frame, 2D | Nguyễn Tuấn Khôi | Vũ Tiến Thăng | ✅ 100% | Review lần 1 trả lại (rejected), Khôi sửa, review lại đã qua |
| 4 | Job 1494 — 25 frame, 2D | Vũ Tiến Thăng | Phạm Hữu Hải | ✅ 100% | Review lần 1 trả lại (rejected), Thăng sửa, review lại đã qua |

### Segmentation

| # | Nội dung công việc | Annotator | Reviewer | Hoàn thành | Ghi chú |
|---|---|---|---|---|---|
| 1 | Job 1710 — 25 ảnh | Phạm Hữu Hải | Nguyễn Hữu Dũng | ✅ 100% | Đã qua review |
| 2 | Job 1711 — 25 ảnh | Nguyễn Tuấn Khôi | Vũ Tiến Thăng | ✅ 100% | Đã qua review |
| 3 | Job 1712 — 25 ảnh | Nguyễn Hùng Mạnh | Nguyễn Tuấn Khôi | ✅ 100% | Đã qua review |
| 4 | Job 1713 — 25 ảnh | Nguyễn Hữu Dũng | Nguyễn Hùng Mạnh | ✅ 100% | 20/09 Dũng vào làm lại, gán xong và đã qua review |

## Tổng kết

Tính riêng từng phần, không cộng chung.

| Phần | Đã gán | Qua review lần đầu |
|---|---|---|
| BBox_Polygon_Polyline | 100 / 100 frame (100%) — **xong cả gán và review** | 0 / 4 job qua review lần đầu — cả 4 job bị trả lại 1 lần, sửa xong đều đã qua |
| Segmentation | 100 / 100 ảnh (100%) — **xong cả gán và review** | 4 / 4 job đã qua review (chưa ghi số lần bị trả lại) |

- Edge case mới: [P-001](../problem-backlog.md#p-001) (xe đứng dày đặc), [P-002](../problem-backlog.md#p-002) (vùng không xác định được class), [P-003](../problem-backlog.md#p-003) (kết cấu cầu) — cả ba thuộc Segmentation
- Edge case đã chốt: P-001 → [QĐ-001](../so-quyet-dinh.md#qđ-001) tô chung thành một mảng (19/09) · P-002 → [QĐ-002](../so-quyet-dinh.md#qđ-002) không tô, để trống (19/09) · P-003 → [QĐ-003](../so-quyet-dinh.md#qđ-003) không vẽ kết cấu cầu (20/09)

## Vướng mắc

- **Chưa liên hệ được 1 thành viên** (Nguyễn Hữu Dũng): không có trong nhóm Discord, liên hệ riêng
  chưa phản hồi, đã báo BTC. Ngày 19/09 đã chuyển job 1497 cho Hải, review job 1710 cho Mạnh.
  Ngày 20/09 Dũng vào làm lại và gán xong job Seg 1713 — đã xử lý xong.
- **Team có 2 lead, mỗi lead chỉ thấy một phần:** lead 1 chỉ thấy `bbox_polygon`, lead 2 chỉ thấy
  segmentation. Khó tổng hợp tiến độ, edge case và quyết định chung của cả đội.

## Kế hoạch tuần 02

**Tiến độ**
- ✅ BBox: xong cả 4 job, đã qua review.
- ✅ Seg: xong cả 4 job, đã qua review.
- Mỗi reviewer ghi số ảnh bị trả lại để điền "Qua review lần đầu".

**Thành viên chưa liên hệ được**
- ✅ Đã chuyển job 1497 cho Hải, review job 1710 cho Mạnh (19/09).
- Cập nhật assignee job 1497 trên CVAT sang Hải.
- ✅ 20/09 Dũng vào làm lại, gán xong job Seg 1713. Job BBox 1497 không lấy lại từ Hải.
- Báo BTC là đã liên lạc lại được với Dũng.

**Phối hợp 2 lead**
- Dùng chung repo này làm nơi tổng hợp: cả 2 lead cùng cập nhật nhật ký tuần, backlog và sổ quyết định.
- ✅ Tách bảng Công việc và Tổng kết thành 2 phần BBox_Polygon_Polyline / Segmentation (19/09).
- Ghi rõ mỗi mục P / QĐ áp dụng cho phần nào.
- Hẹn 2 lead trao đổi ngắn mỗi cuối tuần trước khi chốt nhật ký.

**Edge case**
- ✅ Đã chốt P-001 → QĐ-001, P-002 → QĐ-002 (19/09).
- Báo QĐ-001, QĐ-002 cho cả đội phần Segmentation.
- Rà lại các ảnh đã gặp hai trường hợp này, sửa theo quyết định.

**Hoàn thiện repo**
- Thu handle GitHub của các thành viên để thay cho mã sinh viên.
- Bổ sung link CVAT (job + frame) cho P-001, P-002 và task của tuần.
