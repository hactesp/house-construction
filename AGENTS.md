## Tài khoản GitHub & SSH (quy ước bắt buộc)

- **Remote SSH**: luôn dùng alias `github.com-hct` (không dùng `github.com` trần). Remote `origin` phải là `git@github.com-hct:hactesp/house-construction.git`. Alias này trỏ tới key cá nhân `~/.ssh/id_ed25519`, xác thực đúng tài khoản `hactesp` (chủ repo, có quyền push). Nếu dùng `github.com` trần, SSH có thể rơi vào key/tài khoản khác không có quyền ghi trên repo này.
- **`gh` CLI**: máy có nhiều tài khoản đăng nhập trong `gh auth status`, gồm `hactesp` (admin/push trên repo này) và `John-hivo` (chỉ pull, không có quyền ghi). Trước khi chạy bất kỳ thao tác `gh` nào cần quyền ghi trên repo này (tạo/sửa issue, label, PR...), phải kiểm tra active account bằng `gh auth status` và đảm bảo đang active là `hactesp`; nếu không, chạy `gh auth switch --hostname github.com --user hactesp` trước.

## Agent skills

### Issue tracker

Issues are tracked as GitHub Issues in `hactesp/house-construction`, using the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default five canonical roles, each label string equal to its name (`needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `GLOSSARY.md` + `docs/adr/` at the repo root. See `docs/agents/domain.md`.
