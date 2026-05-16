---
name: frontend-interaction-accessibility-skill
description: Quy tắc interaction và accessibility cho UI web: state, feedback, keyboard, focus, form error, motion, semantic HTML và khả năng thao tác.
argument-hint: "frontend interaction accessibility task"
user-invocable: true
---

# Frontend Interaction Accessibility Skill

## Tư duy chính

UI không chỉ để nhìn. UI phải phản hồi rõ, thao tác được, không gây bối rối và dùng được với nhiều kiểu người dùng, thiết bị, kích thước màn hình.

## State bắt buộc

Với component quan trọng, cân nhắc các state:

- Default.
- Hover.
- Active.
- Focus.
- Loading.
- Disabled.
- Empty.
- Error.
- Success.

Không chỉ thiết kế happy path.

## Feedback

- Mọi hành động quan trọng cần phản hồi.
- Loading phải cho biết hệ thống đang xử lý.
- Error phải nói lỗi gì và cách sửa.
- Success nên xác nhận kết quả ngắn gọn.
- Disabled action nên có lý do nếu user có thể thắc mắc.

## Accessibility

- Dùng semantic HTML trước khi dùng ARIA.
- Mọi chức năng phải dùng được bằng bàn phím.
- Focus state phải thấy rõ.
- Form input phải có label.
- Error message không chỉ dựa vào màu.
- Icon button cần accessible name.
- Không tạo keyboard trap trong modal/dropdown.

## Motion

- Motion phải có mục đích: hướng chú ý, giải thích chuyển trạng thái, giảm cảm giác giật.
- Duration thường 150–300ms.
- Không dùng animation lặp gây phân tâm.
- Tôn trọng reduced motion nếu project hỗ trợ.

## Microcopy

- Button dùng động từ rõ nghĩa.
- Empty state nói vì sao trống và nên làm gì tiếp.
- Error message cụ thể, không đổ lỗi cho user.
- Tooltip chỉ bổ sung thông tin, không chứa nội dung bắt buộc để hoàn thành flow.

## Checklist hoàn thành

- Dùng keyboard được.
- Focus rõ.
- Có feedback cho action quan trọng.
- Loading/empty/error không bị bỏ quên.
- Form có label và error rõ.
- Motion không gây nhiễu.
