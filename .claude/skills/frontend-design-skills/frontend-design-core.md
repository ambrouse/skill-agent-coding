---
name: frontend-design-core
description: Quy tắc cốt lõi khi thiết kế UI web/frontend: mục tiêu người dùng, phân cấp thị giác, cấu trúc màn hình, trạng thái và tính nhất quán.
argument-hint: "frontend design task"
user-invocable: true
---

# Frontend Design Core

## Tư duy chính

Thiết kế web tốt phải giúp người dùng hiểu nhanh, thao tác dễ và tin được vào giao diện. Đẹp chỉ có giá trị khi làm sản phẩm rõ hơn, dễ dùng hơn hoặc đáng nhớ hơn.

Trước khi thiết kế, luôn xác định:

1. Người dùng đang muốn hoàn thành việc gì?
2. Thông tin nào quan trọng nhất?
3. Hành động chính là gì?
4. Trạng thái nào có thể xảy ra: loading, empty, error, disabled, success?
5. UI có nhất quán với phần còn lại của sản phẩm không?

## Quy tắc bắt buộc

- Mỗi màn hình chỉ nên có một mục tiêu chính.
- Primary action phải rõ hơn secondary action.
- Không làm mọi thứ nổi bật cùng lúc.
- UI phải hoạt động với dữ liệu thật: text dài, ảnh lỗi, danh sách trống, quyền bị thiếu.
- Nếu project đã có component, token hoặc design system, dùng cái có sẵn trước.
- Không thêm thư viện UI mới nếu task không yêu cầu.

## Thứ tự ưu tiên khi thiết kế

1. Rõ ý.
2. Đúng phân cấp.
3. Dễ thao tác.
4. Responsive ổn.
5. Accessible.
6. Đẹp và có cá tính.

Không được đảo thứ tự này để chạy theo hiệu ứng hoặc trang trí.

## Checklist hoàn thành

- Nhìn vào biết màn hình dùng để làm gì.
- Hành động chính dễ tìm.
- Có đủ state quan trọng.
- Không vỡ khi dữ liệu dài hoặc thiếu.
- Nhất quán với style hiện có.
- Không có chi tiết trang trí thừa làm nhiễu nội dung.
