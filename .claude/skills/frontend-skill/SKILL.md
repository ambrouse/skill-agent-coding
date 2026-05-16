---
name: frontend-skill
description: Quy tắc bắt buộc khi Claude Code viết hoặc sửa frontend, UI component, page, style, state, API client, accessibility, SEO hoặc test frontend.
argument-hint: "frontend task"
user-invocable: true
---

# Frontend Skill

Khi làm task frontend trong Claude Code, bắt buộc tuân thủ các quy tắc sau.

## Skill phụ trợ

- Sử dụng skill /frontend-design-skills để thiết kế giao diện, không tự thiết kế.

## Cấu trúc thư mục

- `src/`: Chứa mã nguồn chính của ứng dụng.
  - `components/`: Chứa UI components.
  - `pages/`: Chứa pages của ứng dụng.
  - `services/`: Chứa service gọi API hoặc xử lý dữ liệu.
  - `utils/`: Chứa tiện ích chung.
- `assets/`: Chứa hình ảnh, font chữ và tài nguyên tĩnh.
- `styles/`: Chứa CSS hoặc stylesheet khác.
- `tests/`: Chứa test cho frontend.
- `docs/`: Chứa tài liệu kỹ thuật liên quan đến ứng dụng.
- `logs/`: Chứa log của ứng dụng hoặc log làm việc khi được yêu cầu.
- `public/`: Chứa static files như index.html, favicon.

## Quy tắc đặt tên

- Tên biến, hàm, lớp phải rõ ràng và mô tả đúng chức năng.
- Sử dụng `camelCase` cho biến và hàm.
- Sử dụng `PascalCase` cho component, class, type hoặc interface nếu phù hợp.
- Tránh viết tắt không rõ nghĩa.
- Biến boolean nên dùng tiền tố `is`, `has`, `can`, `should`.
- Hàm xử lý event nên dùng tiền tố `handle`.

## Quy tắc viết code

- Viết code sạch, dễ đọc, dễ bảo trì.
- Ưu tiên component nhỏ, rõ trách nhiệm và tái sử dụng hợp lý.
- Không thêm abstraction hoặc refactor ngoài phạm vi task nếu không cần thiết.
- Viết hoặc cập nhật test khi task thay đổi logic, state, validation hoặc interaction quan trọng.
- Chạy linter, typecheck hoặc test phù hợp trước khi báo hoàn thành nếu project có sẵn command.
- Với thay đổi UI, phải chạy app và kiểm tra trực tiếp trên browser nếu môi trường cho phép.
- Tối ưu hiệu suất bằng lazy loading, code splitting, memoization khi có vấn đề thực tế.
- Đảm bảo accessibility: semantic HTML, keyboard navigation, label, aria khi cần.
- Đảm bảo responsive design và tương thích trình duyệt theo yêu cầu dự án.
- Không lưu secret hoặc thông tin nhạy cảm trong frontend source.
- Validate input tại boundary và xử lý lỗi từ API rõ ràng.
- Cập nhật tài liệu kỹ thuật khi thay đổi flow, page, setup hoặc behavior quan trọng.

## Kiến trúc và thiết kế

- Sử dụng kiến trúc component-based để tạo UI dễ tái sử dụng và bảo trì.
- Thiết kế giao diện rõ ràng, nhất quán, có feedback cho user.
- Sử dụng pattern phù hợp như Container/Presentational hoặc custom hooks khi thật sự giúp code rõ hơn.
- Đảm bảo app có khả năng mở rộng và dễ bảo trì.
- Dùng công nghệ và framework phù hợp với stack đang có.
- Có cơ chế cleanup logs, cache, dữ liệu tạm nếu task tạo ra dữ liệu phụ.
