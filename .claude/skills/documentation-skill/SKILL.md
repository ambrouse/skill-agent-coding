---
name: documentation-skill
description: Quy tắc bắt buộc khi Claude Code tạo hoặc cập nhật tài liệu dự án, docs kỹ thuật, task summary, API docs hoặc hướng dẫn vận hành.
argument-hint: "documentation task"
user-invocable: true
---

# Documentation Skill

Khi viết hoặc cập nhật documentation trong Claude Code, bắt buộc tuân thủ các quy tắc sau.

## Lưu trữ

- File documentation phải lưu trong folder `docs` ở project tổng, trừ khi user chỉ định vị trí khác.
- Nên chia folder theo loại docs như architecture, api, setup, task, operation nếu tài liệu nhiều.
- Không tạo file documentation mới nếu task không yêu cầu và thông tin có thể nằm trong file hiện có.

## Format

- Có tiêu đề rõ ràng, ngày tháng rõ ràng và phạm vi nội dung rõ ràng.
- Có thể gộp các file liên quan vào một docs nhưng phải tóm tắt, chỉ giữ nội dung quan trọng.
- Nội dung phải chính xác với source code hiện tại, không overclaim.
- Ưu tiên bullet ngắn, bảng hoặc section rõ ràng để dễ quét.
- Sau mỗi task có yêu cầu documentation, quét lại docs liên quan để tóm tắt, clean, xóa hoặc sửa phần lỗi thời nếu cần.

## Nội dung bắt buộc khi phù hợp

- Mục tiêu thay đổi.
- File hoặc module bị ảnh hưởng.
- Cách chạy, cấu hình hoặc test nếu có.
- Rủi ro, giới hạn hoặc việc còn lại nếu có.
