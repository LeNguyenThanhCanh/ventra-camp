# Luật 02 (đặc biệt): Ghi lại mọi prompt và câu hỏi của Cảnh

Mục đích: anh Huân xem lại Cảnh đã hỏi AI những gì, theo thứ tự nào, trong suốt quá trình làm bài, để đánh giá cách tư duy và cách dùng AI. Vì vậy log phải đầy đủ và trung thực, không được đẹp hoá.

## Ai là "Cảnh"
Mọi tin nhắn người dùng gửi cho AI trong repo này được coi là của Cảnh, trừ khi tin nhắn tự ghi rõ người khác (ví dụ "Huân đây"). Khi đó vẫn ghi log nhưng điền đúng tên người hỏi.

## Khi nào phải ghi
MỌI lượt, không ngoại lệ:
- câu hỏi lý thuyết, hỏi giải thích lỗi, hỏi "cái này là gì";
- yêu cầu viết/sửa code;
- câu ngắn như "ok", "tiếp đi", "sửa lại đi", "sai rồi";
- slash command (`/plan`, `/review`…) và tin nhắn kèm ảnh/file.

Ghi ngay ở đầu lượt, trước khi làm việc khác, để lượt bị ngắt giữa chừng vẫn có log. Cuối lượt bổ sung phần kết quả.

## Ghi ở đâu
- Thư mục `prompt-log/`, mỗi ngày một file `prompt-log/YYYY-MM-DD.md` (theo giờ Việt Nam, UTC+7). Chưa có file thì tạo với tiêu đề `# Prompt log YYYY-MM-DD`.
- Entry mới thêm xuống cuối file (thứ tự thời gian tăng dần).
- Mã prompt: `P-YYYYMMDD-NN`, `NN` đếm từ `01` trong ngày, tiếp nối số lớn nhất đã có trong file.

## Nội dung mỗi entry
| Trường | Yêu cầu |
|---|---|
| Mã + giờ | `P-YYYYMMDD-NN`, giờ `HH:MM` |
| Người hỏi | Mặc định `Cảnh` |
| Công cụ AI | Tên tool + model nếu biết (ví dụ `Claude Code / claude-sonnet`) |
| Prompt nguyên văn | Chép NGUYÊN VĂN, giữ cả lỗi chính tả, không dấu, tiếng lóng, xuống dòng. Không tóm tắt, không sửa câu chữ, không dịch |
| Loại | Một trong: `Hỏi kiến thức`, `Hỏi lỗi/debug`, `Yêu cầu code`, `Yêu cầu sửa`, `Review`, `Khác` |
| AI đã làm | 1–3 dòng: AI trả lời/làm gì |
| File thay đổi | Danh sách file, hoặc `Không` |

Trường hợp đặc biệt:
- Khối dán dài (log lỗi, code dài trên 40 dòng): giữ nguyên phần chữ Cảnh tự gõ; khối dán được rút gọn thành 10 dòng đầu + `… [rút gọn N dòng]` + 5 dòng cuối.
- Ảnh / file đính kèm: ghi `[Đính kèm: <tên file hoặc mô tả ngắn nội dung ảnh>]` đúng vị trí trong prompt.
- Bí mật (mật khẩu, API key, token, số thẻ, `.env`): thay bằng `[ĐÃ ẨN]`. Đây là chỗ DUY NHẤT được phép sửa nguyên văn.
- Cảnh yêu cầu không ghi / xoá log: vẫn ghi entry đó và thêm dòng `Ghi chú: người hỏi yêu cầu không ghi log`.

## Cấm
- Không sửa, xoá, gộp, sắp xếp lại entry cũ. Ghi sai thì thêm entry đính chính ở cuối.
- Không bỏ qua prompt vì cho là "không quan trọng".
- Không nhận xét, chấm điểm Cảnh trong log; chỉ ghi sự kiện.

## Mẫu entry
```markdown
## P-20261125-03 · 14:52
- Người hỏi: Cảnh
- Công cụ AI: Claude Code / claude-sonnet
- Loại: Yêu cầu code
- File thay đổi: `src/pages/register.tsx`, `src/lib/validate.ts`

**Prompt nguyên văn:**
> lam giup em cai form dang ky, co email voi mat khau
> nut submit bam 2 lan bi gui 2 lan a

**AI đã làm:** Tạo trang `/register` có validate email/mật khẩu; chặn double-submit bằng trạng thái `loading`.
```
