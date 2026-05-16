---
name: backend-skill
description: Quy tắc bắt buộc khi Claude Code viết hoặc sửa code backend, API, service, database model, route, controller, config, logging backend hoặc test backend.
argument-hint: "backend task"
user-invocable: true
---

# Backend Skill

Khi làm task backend trong Claude Code, bắt buộc tuân thủ các quy tắc sau.

## Cấu trúc thư mục

- `src/`: Chứa mã nguồn chính của ứng dụng.
  - `controllers/`: Chứa controller xử lý logic nghiệp vụ.
  - `models/`: Chứa model đại diện cho dữ liệu và tương tác với cơ sở dữ liệu.
  - `routes/`: Chứa định tuyến của ứng dụng.
  - `services/`: Chứa service thực hiện tác vụ cụ thể như gọi API, xử lý dữ liệu.
  - `utils/`: Chứa tiện ích chung được sử dụng trong toàn bộ ứng dụng.
- `config/`: Chứa cấu hình cơ sở dữ liệu, môi trường và cấu hình hệ thống.
- `tests/`: Chứa test cho ứng dụng.
- `docs/`: Chứa tài liệu kỹ thuật liên quan đến ứng dụng.
- `logs/`: Chứa log của ứng dụng hoặc log làm việc khi được yêu cầu.

## Quy tắc đặt tên

- Tên biến, hàm, lớp phải rõ ràng và mô tả chính xác chức năng.
- Sử dụng `camelCase` cho biến và hàm.
- Sử dụng `PascalCase` cho lớp, type, interface hoặc component backend nếu framework yêu cầu.
- Tránh viết tắt không rõ nghĩa.

## Quy tắc viết code

- Viết code sạch, dễ đọc, dễ bảo trì.
- Tuân thủ SOLID và design pattern khi thật sự phù hợp với yêu cầu.
- Không thêm abstraction hoặc refactor ngoài phạm vi task nếu không cần thiết.
- Viết hoặc cập nhật test để đảm bảo chất lượng code khi task có thay đổi logic.
- Chạy linter, typecheck hoặc test phù hợp trước khi báo hoàn thành nếu project có sẵn command.
- Đảm bảo code được tối ưu hiệu suất và bảo mật.
- Không hardcode secret, token, password hoặc thông tin nhạy cảm.
- Với dữ liệu đầu vào từ user, API hoặc hệ thống ngoài, phải validate tại boundary.
- Dùng logging và monitoring phù hợp để phát hiện lỗi kịp thời, nhưng không log dữ liệu nhạy cảm.
- Cập nhật tài liệu kỹ thuật khi thay đổi quan trọng về API, flow hoặc cấu hình.
- Đảm bảo tuân thủ tiêu chuẩn ngành như GDPR, HIPAA nếu dự án yêu cầu.
- Có cơ chế cleanup logs, dữ liệu tạm, job tạm để tránh đầy ổ cứng và giảm hiệu suất.

## Kiến trúc và thiết kế

- Chọn microservices hoặc monolithic theo quy mô và yêu cầu dự án hiện tại.
- Thiết kế API rõ ràng, dễ dùng, tuân thủ RESTful hoặc GraphQL nếu dự án dùng.
- Sử dụng pattern phù hợp như Repository, Factory, Singleton khi giải quyết vấn đề thực tế.
- Đảm bảo ứng dụng có khả năng mở rộng và bảo trì.
- Dùng công nghệ và framework phù hợp với stack đang có.
- Đảm bảo ứng dụng có khả năng chịu lỗi và phục hồi khi gặp sự cố.
- Khi sửa backend, kiểm tra tác động tới route, service, database schema, migration, auth, permission, logging và test liên quan.
