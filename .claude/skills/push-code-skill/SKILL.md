---
name: push-code-skill
description: Quy tắc bắt buộc khi Claude Code chuẩn bị commit, push, tạo PR, kiểm tra CI/CD, README, versioning hoặc cấu hình repository.
argument-hint: "push or release task"
user-invocable: true
---

# Push Code Skill

Áp dụng khi user yêu cầu commit, push, tạo PR, release hoặc chuẩn bị repository để đưa code lên remote.

## CI/CD

- Trước khi push, kiểm tra CI/CD hiện có để xem có cần cập nhật hoặc bổ sung không.
- Đảm bảo test phù hợp đã được chạy và pass.
- Với project production, ưu tiên test nghiêm ngặt cho các phần quan trọng.
- Không bỏ qua hook, linter hoặc test bằng `--no-verify` trừ khi user yêu cầu rõ ràng.

## Quy tắc commit và push

- Chỉ commit hoặc push khi user yêu cầu rõ ràng.
- Commit message phải rõ ràng, mô tả đúng lý do thay đổi.
- Nếu repository yêu cầu format riêng, tuân thủ format hiện có trong git log.
- Không commit secret, `.env`, credential, token hoặc file nhạy cảm.
- Trước khi push, kiểm tra trạng thái git và diff để đảm bảo chỉ đưa đúng file cần thiết.

## Setup repository

- Kiểm tra `.gitignore`, `.env.example`, CI/CD workflow nếu task liên quan đến setup hoặc release.
- Nếu thiếu cấu hình khởi đầu quan trọng, đề xuất hoặc thêm theo yêu cầu user.
- Quản lý version rõ ràng, chuyên nghiệp nếu project có versioning.

## README

- Khi tạo hoặc sửa README, dùng `readme-style`.
- Nếu chưa có banner, ưu tiên ảnh frontend nếu project có UI; nếu không, có thể đề xuất banner đơn giản nhưng không tạo tài nguyên không cần thiết.
