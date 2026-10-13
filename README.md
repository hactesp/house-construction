# Thiết kế Nhà 2 tầng phong cách Scandinavian

Hồ sơ thiết kế một Nhà 2 tầng trên khu đất 20m × 18m, hướng Tây/Tây Nam. Mục tiêu là một bộ bản vẽ đủ rõ để kiến trúc sư/kỹ sư có chứng chỉ hành nghề rà soát và ký tên trước khi xin phép xây dựng.

## Thông số đã chốt

- Diện tích xây dựng: 8,5m × 12m. Ban công tầng 2 được đua ra ngoài phần này.
- Khoảng lùi: Phải 4,5m, Trái 7,0m, sau 30cm, trước 5,7m.
- Tầng 1: phòng khách + phòng ăn, 2 phòng ngủ, 1 vệ sinh, Bếp khô. Bếp ướt ở sân Trái.
- Tầng 2: 2 phòng ngủ, phòng thờ, 1 vệ sinh, phòng sinh hoạt chung.
- Chỗ để xe: 1 ô tô 7 chỗ trong Khoảng lùi Phải, khoảng 3 xe máy ở Khoảng lùi trước.

Danh sách đầy đủ và cập nhật nhất nằm ở map [#1](https://github.com/hactesp/house-construction/issues/1).

## Cách làm việc

Dự án dùng bộ skill của Matt Pocock (thư mục `.agents/skills/`):

- **Map** ([#1](https://github.com/hactesp/house-construction/issues/1)): các quyết định thiết kế được chia thành ticket trên GitHub Issues và giải quyết lần lượt bằng skill `wayfinder`, mỗi phiên một ticket.
- **Spec** ([#9](https://github.com/hactesp/house-construction/issues/9)): mô tả bộ bản vẽ cần có. Sẽ cập nhật lại khi map giải quyết xong.
- **Prototype**: bản phác HTML để so sánh phương án, lưu trên nhánh `prototype/<tên>`, không đưa vào `master`.

## Cấu trúc repo

| Đường dẫn | Nội dung |
| --- | --- |
| `GLOSSARY.md` | Thuật ngữ dùng chung (Nhà, Mặt tiền, Trái/Phải, Khoảng lùi…) |
| `docs/adr/` | Ghi chép các quyết định quan trọng và lý do (ADR) |
| `docs/agents/` | Cấu hình cho agent: issue tracker, nhãn triage, tài liệu domain |
| `AGENTS.md` | Quy ước cho agent, gồm tài khoản GitHub và SSH |
| `draft-idea.md` | Ý tưởng ban đầu, giữ nguyên làm tư liệu gốc |
| `skills-lock.json` | Phiên bản các skill đã cài |

## Quy ước GitHub

Remote dùng alias SSH `github.com-hct`. Trước khi ghi lên GitHub bằng `gh`, kiểm tra tài khoản đang active là `hactesp`. Chi tiết trong `AGENTS.md`.
