---
name: logging-skill
description: Quy tắc bắt buộc khi Claude Code ghi và quản lý logs phiên làm việc, task log hoặc nhật ký triển khai; không dùng cho debug log trong source code.
argument-hint: "logging task"
user-invocable: true
---

# Logging Skill

Skill này áp dụng cho logs của phiên làm việc hoặc task, không phải debug log trong code.

## Lưu trữ

- Tất cả task logs phải lưu trong folder tổng `logs` ở project tổng, trừ khi user chỉ định vị trí khác.
- Mỗi task nên có log riêng hoặc được gom vào file liên quan nếu cùng một nhóm công việc.
- Chia folder rõ ràng theo loại task hoặc thời gian nếu số lượng log nhiều.

## Tóm tắt

- Mỗi file log không được quá dài; chỉ tóm tắt điểm quan trọng và trọng tâm.
- Nếu nhiều logs liên quan đến nhau, có thể gom chung và viết summary ngắn.
- Sau mỗi task có yêu cầu logging, quét lại logs liên quan để clean, tóm tắt, xóa hoặc sửa phần lỗi thời nếu cần.

## Format

- Log phải có thời gian rõ ràng.
- Ghi mục tiêu task, hành động chính, kết quả test/verify, blocker nếu có.
- Không ghi secret, token, password, thông tin cá nhân hoặc dữ liệu nhạy cảm.
