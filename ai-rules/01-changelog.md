# Luật 01: Bắt buộc ghi CHANGELOG

## Khi nào phải ghi
Mọi lượt AI làm repo thay đổi, gồm:
- tạo, sửa, xoá, đổi tên, di chuyển file hoặc thư mục;
- chạy lệnh làm đổi repo: cài/gỡ package (đổi lockfile), migrate DB, generate code, format hàng loạt;
- git commit, merge, rebase, tạo/xoá branch.

Không cần ghi khi lượt đó chỉ đọc code, trả lời câu hỏi, hoặc chỉ sửa `CHANGELOG.md` / `prompt-log/` (tránh ghi đệ quy).

## Ghi ở đâu, thế nào
- File: `CHANGELOG.md` ở gốc repo. Chưa có thì tạo theo mẫu đầu file hiện tại.
- Mỗi ngày một mục `## YYYY-MM-DD`, ngày mới nhất ở trên cùng. Trong ngày, entry mới thêm xuống cuối mục của ngày đó.
- Ghi bằng tiếng Việt, câu ngắn, nói thay đổi gì và vì sao; không chép lại code.
- Phân loại mỗi dòng bằng một nhãn: `Thêm`, `Sửa`, `Sửa lỗi`, `Xoá`, `Bảo mật`.
- Mỗi entry PHẢI dẫn mã prompt (`P-YYYYMMDD-NN`, xem luật 02) để truy ngược câu hỏi nào sinh ra thay đổi nào.
- Liệt kê các file chính bị đổi (đường dẫn tương đối).
- Ghi xong changelog TRONG CÙNG lượt với thay đổi, trước khi báo "xong". Không dồn để ghi sau.
- Không sửa/xoá entry cũ. Nếu entry cũ sai, thêm entry mới đính chính.

## Mẫu entry
```markdown
## 2026-11-25

### P-20261125-03: Thêm form đăng ký
- Thêm: trang `/register` với form email + mật khẩu, validate phía client.
- Sửa lỗi: nút Submit bị bấm 2 lần gửi 2 request.
- File: `src/pages/register.tsx`, `src/lib/validate.ts`
```

## Commit
Khi AI tạo git commit, `CHANGELOG.md` và file `prompt-log/` của lượt đó phải nằm trong cùng commit với thay đổi code.
