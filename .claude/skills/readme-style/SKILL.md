---
name: readme-style
description: README style guide cho Claude Code. Dùng khi tạo hoặc cập nhật README, banner, badges, quick navigation, architecture summary, Mermaid diagram, repo map, docs index hoặc accuracy notes.
argument-hint: "README task"
user-invocable: true
---

# README Style Guide

Tài liệu này mô tả phong cách README có thể tái sử dụng cho landing page, docs hub hoặc repo cùng hệ màu.

## 1. Mục tiêu thiết kế

README được định hướng theo phong cách "product landing page inside GitHub Markdown": vào là thấy banner, nhìn là hiểu sản phẩm, đọc nhanh là hiểu hệ thống chạy thế nào, kéo xuống là thấy pipeline, deployment và repo map.

Mục tiêu không phải trình bày tất cả chi tiết, mà là tạo nhịp đọc rõ ràng giữa marketing kỹ thuật và tài liệu vận hành.

## 2. Nguồn cảm hứng thị giác

Bố cục mô phỏng README dashboard dài, có các đặc điểm sau:

1. Hero mạnh ở đầu trang.
2. Tiêu đề và tagline căn giữa.
3. Badge line đầy, tạo cảm giác sản phẩm có hệ sinh thái rõ.
4. Link điều hướng nhanh ngay dưới hero.
5. Nhiều bảng thông tin và section ngắn thay vì đoạn văn dài.
6. Có section flow và feature matrix để người đọc quét nhanh.

## 3. Nguyên tắc bố cục

README mới đi theo nhịp sau:

1. Hero section.
2. Tổng quan hệ thống.
3. System flow bằng Mermaid.
4. Quick start rất ngắn, ưu tiên lệnh chạy thật.
5. Application pipelines để giải thích giá trị.
6. Deployment profiles.
7. Repository map.
8. Docs index.
9. Accuracy notes để tránh overclaim.

## 4. Ngôn ngữ trình bày

README dùng giọng văn kỹ thuật bên ngoài:

1. Câu ngắn, xác định, ít tính từ khoa trương.
2. Dùng từ mang tính hệ thống và pipeline, không viết quá marketing.
3. Nếu một tính năng là tùy chọn hoặc chưa hoàn tất, phải nói rõ.
4. Mỗi section cần trả lời một câu hỏi cụ thể: hệ thống là gì, chạy như thế nào, thành phần nào quan trọng, vào code ở đâu.

## 5. Ngôn ngữ hình khối

Do GitHub Markdown không cho phép CSS tự do, phong cách được tạo bằng các kỹ thuật sau:

1. `div align="center"` cho hero.
2. Ảnh banner full width để tạo cảm giác product-led.
3. Badge style `for-the-badge` để tạo nhận diện dạng landing page.
4. Bảng Markdown để giả lập card thông tin.
5. Mermaid diagram để đóng khung kiến trúc mà không cần ảnh ngoài.

## 6. Quy tắc nội dung

README là trang điều hướng cấp cao, không phải tài liệu đầy đủ nhất. Vì vậy:

1. Giữ quick start ngắn và thực dụng.
2. Chỉ nói những pipeline đã được đối chiếu với source.
3. Đẩy chi tiết xuống docs chuyên đề.
4. Thêm `Notes On Accuracy` để tránh README đọc hay hơn code.

## 7. Bản sắc cần giữ nếu tái sử dụng

1. Hero rõ ràng và có hình nền nhận diện.
2. Information density cao nhưng có nhóm section rõ.
3. Đọc là thấy flow trước, chi tiết sau.
4. Sự trung thực kỹ thuật được ưu tiên hơn slogan.

## 8. Khi nào không nên dùng phong cách này

Không nên dùng phong cách này nếu repo chỉ là thư viện nhỏ, package đơn lẻ hoặc repo nội bộ không có nhu cầu giới thiệu kiến trúc. Với các repo đó, README ngắn và trực diện sẽ tốt hơn.

## 9. Tóm tắt một câu

Phong cách README này là sự kết hợp giữa landing page sản phẩm và operational architecture brief, được thiết kế để người đọc hiểu nhanh hệ thống làm gì, chạy thế nào và nên vào đâu trong repo nếu muốn đào sâu hơn.
