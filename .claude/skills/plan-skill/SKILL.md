---
name: plan-skill
description: Quy tắc bắt buộc khi Claude Code lập kế hoạch cho task coding, chia phase, xác định skill cần dùng, testing, documentation, logging và quy trình hoàn thành.
argument-hint: "planning task"
user-invocable: true
---

# Plan Skill

Với mỗi task coding đủ phức tạp, Claude Code phải tuân thủ quy trình sau.

## Quy trình lập kế hoạch

1. Lập plan rõ ràng trước khi code khi task có nhiều bước, ảnh hưởng nhiều file hoặc có nhiều cách triển khai.
2. Nếu user yêu cầu lưu plan thành file, tạo file trong folder `plans` với tên `plan-{task_name}.md`.
3. Trong plan phải mô tả:
   - Mục tiêu task.
   - Các phase hoặc bước cụ thể cần thực hiện.
   - Thời gian dự kiến cho mỗi bước nếu user yêu cầu.
   - Tài nguyên cần thiết nếu có.
   - File hoặc khu vực code dự kiến bị ảnh hưởng nếu đã biết.
4. Plan phải xác định skill cần dùng, ví dụ: `backend-skill`, `frontend-skill`, `testing-skill`, `documentation-skill`, `logging-skill`, `push-code-skill`, `readme-style`.
5. Nếu task chưa rõ, phải hỏi lại trước khi bắt đầu để tránh làm sai quy trình hoặc bỏ qua bước quan trọng.

## Quy trình thực hiện theo phase

Với mỗi phase:

1. Đọc hoặc áp dụng skill cần thiết.
2. Thực hiện phase đó.
3. Test hoặc verify phase đó bằng command hoặc kiểm tra phù hợp.
4. Cập nhật documentation nếu task yêu cầu hoặc thay đổi có ảnh hưởng kỹ thuật quan trọng.
5. Ghi log nếu user hoặc quy trình dự án yêu cầu.
6. Chỉ chuyển phase tiếp theo khi phase hiện tại đã pass theo tiêu chí testing phù hợp.

## Hoàn thành task

- Không được bỏ qua phase đã cam kết trong plan nếu chưa cập nhật lại hướng đi với user.
- Sau khi hoàn thành, tổng kết ngắn gọn trong phản hồi cuối: đã đổi gì, đã test gì, còn gì chưa làm nếu có.
- Nếu task yêu cầu documentation, ghi lại khó khăn và cách giải quyết trong documentation của task.
- Nếu task yêu cầu logging, ghi lại quá trình thực hiện theo `logging-skill`.
- Chỉ push code khi user yêu cầu rõ ràng, và khi đó áp dụng `push-code-skill`.
