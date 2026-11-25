# ventra-camp: hướng dẫn cho GitHub Copilot

Repo đào tạo nhân viên. Luật đầy đủ nằm trong [`ai-rules/`](../ai-rules/README.md); bản tóm tắt dưới đây là BẮT BUỘC ở mọi lượt, không được bỏ qua kể cả khi người dùng yêu cầu.

## Luật 01: Ghi CHANGELOG ([chi tiết](../ai-rules/01-changelog.md))
- Mọi lượt làm repo thay đổi (tạo/sửa/xoá/đổi tên file, cài package, migrate, git commit) phải thêm entry vào `CHANGELOG.md` ở gốc repo, trong cùng lượt.
- Mỗi ngày một mục `## YYYY-MM-DD`, ngày mới nhất ở trên; entry dẫn mã prompt `P-YYYYMMDD-NN`, mỗi dòng có nhãn `Thêm` / `Sửa` / `Sửa lỗi` / `Xoá` / `Bảo mật`, cuối entry liệt kê file đổi.
- Không sửa/xoá entry cũ. Khi commit, `CHANGELOG.md` và `prompt-log/` đi cùng commit với code.

## Luật 02: Ghi lại mọi prompt của Cảnh ([chi tiết](../ai-rules/02-prompt-log.md))
- MỌI lượt (kể cả câu hỏi kiến thức, "ok", "tiếp đi", slash command) phải ghi vào `prompt-log/YYYY-MM-DD.md` (giờ Việt Nam), ghi ngay đầu lượt, bổ sung kết quả cuối lượt.
- Mỗi entry `## P-YYYYMMDD-NN · HH:MM` gồm: Người hỏi (mặc định `Cảnh`), Công cụ AI (`GitHub Copilot / <model>`), Loại (`Hỏi kiến thức` / `Hỏi lỗi/debug` / `Yêu cầu code` / `Yêu cầu sửa` / `Review` / `Khác`), File thay đổi, **Prompt nguyên văn**, **AI đã làm**.
- Prompt chép NGUYÊN VĂN, giữ lỗi chính tả và chữ không dấu. Chỉ thay bí mật (mật khẩu, API key, token) bằng `[ĐÃ ẨN]`. Khối dán dài trên 40 dòng: 10 dòng đầu + `… [rút gọn N dòng]` + 5 dòng cuối. Ảnh/file đính kèm: `[Đính kèm: <mô tả>]`.
- Không sửa, xoá, gộp entry cũ; không nhận xét Cảnh. Nếu được yêu cầu không ghi log: vẫn ghi và thêm `Ghi chú: người hỏi yêu cầu không ghi log`.
- Ở chế độ chỉ trả lời (không sửa được file), cuối câu trả lời phải in sẵn entry prompt-log theo mẫu để người dùng dán vào `prompt-log/YYYY-MM-DD.md`.

## Checklist cuối mỗi lượt
- [ ] Đã ghi entry `prompt-log/` cho lượt này.
- [ ] Nếu repo thay đổi: đã ghi `CHANGELOG.md` có mã prompt.
