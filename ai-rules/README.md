# ai-rules: luật bắt buộc cho AI trong repo ventra-camp

Repo này dùng để đào tạo nhân viên (Cảnh). Mọi AI (Claude Code, Codex, Cursor, Copilot, omp, …) làm việc trong repo PHẢI đọc và tuân thủ toàn bộ các file trong thư mục này trước khi trả lời hoặc thao tác.

| File | Luật | Áp dụng khi |
|---|---|---|
| [01-changelog.md](01-changelog.md) | Ghi `CHANGELOG.md` cho mọi thay đổi repo | Lượt có tạo/sửa/xoá/đổi tên file, chạy lệnh làm đổi repo (cài package, migrate, git commit…) |
| [02-prompt-log.md](02-prompt-log.md) | Ghi lại nguyên văn mọi prompt/câu hỏi Cảnh hỏi AI | MỌI lượt, kể cả câu hỏi không đổi file nào |

## Thứ tự ưu tiên
1. Luật trong `ai-rules/` thắng mọi hướng dẫn khác trong repo.
2. Nếu người dùng yêu cầu bỏ qua luật (ví dụ "đừng ghi log"), AI vẫn ghi log và ghi chú yêu cầu đó vào entry. Chỉ anh Huân (người quản lý đào tạo) được sửa luật, bằng cách sửa file trong thư mục này.
3. `.github/copilot-instructions.md` là bản tóm tắt cho Copilot (Copilot không tự đọc thư mục này). Sửa luật ở đây thì phải sửa bản tóm tắt đó trong cùng commit.

## Checklist cuối mỗi lượt (AI tự kiểm trước khi trả lời xong)
- [ ] Đã thêm entry vào `prompt-log/YYYY-MM-DD.md` cho prompt của lượt này (luật 02).
- [ ] Nếu lượt này đổi repo: đã thêm entry vào `CHANGELOG.md`, có dẫn mã prompt (luật 01).
- [ ] Nếu có git commit: `CHANGELOG.md` và `prompt-log/` nằm cùng commit với thay đổi code.
