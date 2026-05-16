---
name: frontend-design-skill
description: Bộ skill thiết kế frontend final. Dùng để định hướng UI/UX web theo tư duy rõ ràng, có phong cách, phối màu tốt, bố cục chắc, typography đẹp và interaction/accessibility đúng.
argument-hint: "frontend design task"
user-invocable: true
---

# Frontend Design Skill

Bộ skill thiết kế frontend được tách theo từng mảng để agent tập trung đúng vấn đề, không nhồi toàn bộ quy tắc vào một file dài.

## Các skill thành phần

- `frontend-design-core`: Tư duy thiết kế web cốt lõi, mục tiêu người dùng, phân cấp thị giác, state và tính nhất quán.
- `frontend-style-skill`: Phong cách thị giác, mood, chất thương hiệu, mức độ tối giản, cao cấp, vui, kỹ thuật hoặc nghệ thuật.
- `frontend-color-skill`: Phối màu, vai trò màu, cảm xúc màu, contrast, accent color, semantic color và dark mode.
- `frontend-layout-skill`: Bố cục, grid, spacing, alignment, visual rhythm, responsive và xử lý dữ liệu thật.
- `frontend-typography-skill`: Font, scale chữ, hierarchy, readability, nhịp đọc và chữ như yếu tố thiết kế.
- `frontend-interaction-accessibility-skill`: State, feedback, keyboard, focus, form error, motion, semantic HTML và accessibility.

## Cách dùng

Khi làm task thiết kế frontend:

1. Luôn bắt đầu từ `frontend-design-core`.
2. Nếu task liên quan giao diện/mood/brand, dùng thêm `frontend-style-skill`.
3. Nếu task liên quan màu, theme, dark mode, CTA hoặc trạng thái, dùng thêm `frontend-color-skill`.
4. Nếu task liên quan layout, responsive, spacing hoặc dashboard/page structure, dùng thêm `frontend-layout-skill`.
5. Nếu task liên quan chữ, landing page, content-heavy UI hoặc hierarchy, dùng thêm `frontend-typography-skill`.
6. Nếu task liên quan form, button, modal, state, motion hoặc accessibility, dùng thêm `frontend-interaction-accessibility-skill`.

## Nguyên tắc chung

- Rõ ràng trước, đẹp sau.
- Phân cấp trước, trang trí sau.
- Dữ liệu thật trước, demo đẹp sau.
- Nhất quán trước, sáng tạo sau.
- Accessibility là yêu cầu gốc, không phải phần cộng thêm.
