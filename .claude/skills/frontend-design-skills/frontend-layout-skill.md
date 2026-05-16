---
name: frontend-layout-skill
description: Quy tắc bố cục web: grid, spacing, alignment, visual rhythm, responsive, grouping, density và xử lý layout với dữ liệu thật.
argument-hint: "frontend layout task"
user-invocable: true
---

# Frontend Layout Skill

## Tư duy bố cục

Bố cục là cách dẫn mắt. Một layout tốt giúp người dùng biết phần nào quan trọng, phần nào liên quan và nên hành động ở đâu.

## Quy tắc nền tảng

- Căn lề theo container rõ ràng.
- Dùng grid hoặc flex có chủ đích.
- Phần liên quan đặt gần nhau; phần khác nhóm tách xa nhau.
- Khoảng trắng dùng để phân cấp, không phải phần thừa.
- Không chia quá nhiều cột nếu nội dung không cần.

## Spacing scale

Ưu tiên scale nhất quán:

- 4px: tinh chỉnh nhỏ.
- 8px: khoảng cách gần.
- 12–16px: khoảng cách trong component.
- 24–32px: khoảng cách giữa group/section.
- 48px trở lên: khoảng cách giữa block lớn.

Không dùng spacing ngẫu nhiên như 13px, 27px nếu project không có lý do.

## Visual rhythm

- Section quan trọng cần nhiều không gian hơn.
- Danh sách cần nhịp đều để dễ quét.
- Form cần group field theo ý nghĩa.
- Dashboard cần summary trước, chi tiết sau.
- Landing page cần nhịp: hook → value → proof → detail → CTA.

## Responsive

- Mobile không phải bản thu nhỏ của desktop.
- Trên mobile, ưu tiên nội dung và hành động chính.
- Sidebar thường chuyển thành drawer hoặc section dưới.
- Table rộng cần scroll có kiểm soát hoặc chuyển thành card/list.
- Modal phải vừa viewport nhỏ.

## Checklist hoàn thành

- Mắt đi đúng thứ tự mong muốn.
- Group thông tin rõ.
- Spacing nhất quán.
- Mobile/tablet/desktop không vỡ.
- Layout chịu được text dài, empty state và dữ liệu nhiều.
