# Nhật ký tuần 01 · 15/09 – 21/09/2026

**Lead tuần này:** Phạm Hữu Hải (2A202602098)
**Dữ liệu / task CVAT:** Ảnh 2D camera hành trình trên đường phố (có cả cảnh đêm) — 5 job × 25 frame

## Thành viên và phân công

| Thành viên | Vị trí | Phân công tuần này |
|---|---|---|
| Phạm Hữu Hải (2A202602098) | Lead · Annotator · Reviewer | Điều phối, chốt edge case; gán job 1710; review job 1494 |
| Nguyễn Hữu Dũng (2A202602153) | Annotator · Reviewer | Gán job 1497; review job 1710 |
| Nguyễn Hùng Mạnh (2A202602062) | Annotator · Reviewer | Gán job 1496; review job 1497 |
| Nguyễn Tuấn Khôi (2A202602241) | Annotator · Reviewer | Gán job 1495; review job 1496 |
| Vũ Tiến Thắng (2A202602087) | Annotator · Reviewer | Gán job 1494; review job 1495 |

Tuần này **review chéo vòng tròn** (tạm thời): mỗi người review job của người đứng ngay trên
trong bảng, người đầu review job của người cuối. Không ai review job do chính mình gán.

## Công việc

| # | Nội dung công việc | Annotator | Reviewer | Hoàn thành | Ghi chú |
|---|---|---|---|---|---|
| 1 | Job 1710 — 25 frame, 2D | Phạm Hữu Hải | Nguyễn Hữu Dũng | 🟡 30% | Annotation in progress |
| 2 | Job 1497 — 25 frame, 2D | Nguyễn Hữu Dũng | Nguyễn Hùng Mạnh | ⬜ 0% | Chưa bắt đầu. Không có trong nhóm Discord, đã liên hệ riêng nhưng chưa phản hồi, đã báo cáo BTC |
| 3 | Job 1496 — 25 frame, 2D | Nguyễn Hùng Mạnh | Nguyễn Tuấn Khôi | 🟡 30% | Đang gán |
| 4 | Job 1495 — 25 frame, 2D | Nguyễn Tuấn Khôi | Vũ Tiến Thắng | 🟡 50% | Annotation in progress |
| 5 | Job 1494 — 25 frame, 2D | Vũ Tiến Thắng | Phạm Hữu Hải | 🟡 60% | Annotation in progress |

Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

## Tổng kết

- Đã gán: ~42 / 125 frame (34%)
- Qua review lần đầu: Chưa review chéo
- Edge case mới: [P-001](../problem-backlog.md#p-001) (xe đứng dày đặc), [P-002](../problem-backlog.md#p-002) (vùng không xác định được class) — đã tạo Issue, chờ trả lời
- Edge case đã chốt: Chưa có — nháp [QĐ-001](../so-quyet-dinh.md#qđ-001), [QĐ-002](../so-quyet-dinh.md#qđ-002) chờ chốt

## Vướng mắc

- **Chưa liên hệ được 1 thành viên** (Nguyễn Hữu Dũng): không có trong nhóm Discord, liên hệ riêng
  chưa phản hồi, đã báo BTC. Kéo theo:
  - Job 1497 đứng ở 0%.
  - Job 1710 chưa có người review (Dũng là reviewer).
  - Mạnh chưa có job để review.
- **Team có 2 lead, mỗi lead chỉ thấy một phần:** lead 1 chỉ thấy `bbox_polygon`, lead 2 chỉ thấy
  segmentation. Khó tổng hợp tiến độ, edge case và quyết định chung của cả đội.
- **P-001, P-002 chưa có câu trả lời** nên chưa chốt được cách tô xe dày đặc và vùng không xác định
  class. Các ảnh gặp hai trường hợp này có thể phải sửa lại sau khi chốt.

## Kế hoạch tuần 02

**Tiến độ**
- Đưa 4 job đang gán (1710, 1496, 1495, 1494) lên 100%, sau đó bắt đầu review chéo.
- Mỗi reviewer ghi số ảnh bị trả lại để điền "Qua review lần đầu".

**Thành viên chưa liên hệ được**
- Đặt hạn chờ Dũng phản hồi. Quá hạn thì đề nghị BTC chia lại job 1497 cho thành viên khác.
- Trong lúc chờ: chuyển review job 1710 sang Nguyễn Hùng Mạnh.

**Phối hợp 2 lead**
- Dùng chung repo này làm nơi tổng hợp: cả 2 lead cùng cập nhật nhật ký tuần, backlog và sổ quyết định.
- Ghi rõ mỗi job thuộc phần nào (`bbox_polygon` hay segmentation) trong bảng Công việc.
- Ghi rõ mỗi mục P / QĐ áp dụng cho phần nào.
- Hẹn 2 lead trao đổi ngắn mỗi cuối tuần trước khi chốt nhật ký.

**Edge case**
- Theo dõi Issue của P-001, P-002. Có câu trả lời thì chốt QĐ-001, QĐ-002 và báo cả đội.
- Rà lại các ảnh đã gặp hai trường hợp này sau khi chốt.

**Hoàn thiện repo**
- Thu handle GitHub của các thành viên để thay cho mã sinh viên.
- Bổ sung link CVAT (job + frame) cho P-001, P-002 và task của tuần.
