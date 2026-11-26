# Gợi ý lời thuyết trình — Bài 3

Thời lượng mục tiêu: khoảng 5 phút. Tập nói theo ý, không cần đọc nguyên văn.

## Slide 1 — Từ ý tưởng đến sản phẩm (20 giây)

Chào mọi người, hôm nay em trình bày hành trình từ một ý tưởng đến sản phẩm phần mềm. Ý chính là phần mềm không chỉ gồm việc viết code; nhóm cần hiểu đúng vấn đề, xây dựng, kiểm thử, đưa sản phẩm đến người dùng rồi tiếp tục cải tiến.

## Slide 2 — Bản đồ SDLC (55 giây)

SDLC là vòng đời phát triển phần mềm. Đầu tiên nhóm khám phá vấn đề và người dùng. PM hoặc BA giúp làm rõ mục tiêu, yêu cầu và phạm vi. UX/UI thiết kế luồng sử dụng; developer biến thiết kế thành code; QA, tester và developer kiểm thử; DevOps hỗ trợ triển khai, còn nhóm support tiếp nhận vấn đề sau khi phát hành. Tùy công ty, một người có thể đảm nhiệm nhiều vai trò. Các giai đoạn cũng không nhất thiết chỉ đi một chiều: kết quả kiểm thử hay phản hồi của người dùng có thể khiến nhóm quay lại điều chỉnh yêu cầu hoặc thiết kế.

## Slide 3 — Waterfall, Agile và Scrum (60 giây)

Waterfall thường tổ chức công việc theo các giai đoạn tuần tự, nên có thể phù hợp khi yêu cầu ổn định và cần kế hoạch rõ từ đầu. Nếu yêu cầu thay đổi muộn, việc sửa có thể tốn kém. Agile chia công việc thành các phần nhỏ, giao giá trị thường xuyên và học từ phản hồi để điều chỉnh; cách này hữu ích khi nhóm chưa biết chắc người dùng cần gì. Scrum là một framework thuộc Agile, không phải tên khác của toàn bộ Agile. Nhóm chọn việc từ Product Backlog, làm trong một Sprint có thời hạn cố định, xem Increment và điều chỉnh cách làm. Scrum Guide quy định Sprint không dài hơn một tháng.

## Slide 4 — Ví dụ giả định với Grab (60 giây)

Em lấy Grab làm ví dụ giả định và nghĩ về tính năng cho người dùng theo dõi trạng thái đơn đồ ăn. Trước hết nhóm cần kiểm tra vấn đề: người dùng có thật sự lo lắng vì không biết quán đã nhận đơn hay chưa? Sau đó BA hoặc PM xác định yêu cầu; UX/UI thiết kế các trạng thái dễ hiểu. Developer triển khai việc hiển thị và kết nối dữ liệu. Tester thử các tình huống như mạng yếu, hủy đơn hoặc trạng thái cập nhật trễ. Sau khi phát hành, nhóm theo dõi lỗi và phản hồi để cải thiện. Đây chỉ là tình huống minh họa SDLC, không phải mô tả quy trình nội bộ thật của Grab.

## Slide 5 — MVP và cải tiến (45 giây)

Nhóm có thể bắt đầu với MVP, tức phiên bản nhỏ nhất vẫn đủ hữu ích để kiểm tra giả định. MVP không có nghĩa là làm ẩu hoặc bỏ kiểm thử. Ví dụ, trước tiên chỉ cần hiển thị những trạng thái quan trọng của đơn hàng. Sau khi người dùng thử, nhóm đo lường, lắng nghe phản hồi và xem vấn đề ban đầu đã được giải quyết chưa. Từ đó nhóm quyết định cải tiến gì tiếp theo. Công việc còn tiếp tục sau khi ra mắt: sửa lỗi, tăng bảo mật, cải thiện hiệu năng và bổ sung tính năng.

## Slide 6 — GitHub và IDE (45 giây)

IDE, như VS Code, hỗ trợ lập trình viên viết, chạy và tìm lỗi trong code. GitHub hỗ trợ nhóm lưu lịch sử thay đổi, ghi việc cần làm qua issue, tạo pull request và review code. Có thể hình dung developer làm trong IDE, sau đó đưa thay đổi lên GitHub để đồng đội xem xét và hệ thống chạy kiểm tra tự động. Những công cụ này giúp phối hợp, nhưng không thay cho việc hiểu yêu cầu và kiểm thử phần mềm.

## Slide 7 — Tổng kết (15 giây)

Tóm lại, SDLC giúp nhóm đi từ vấn đề đến sản phẩm được duy trì. Waterfall và Agile có cách tổ chức khác nhau, nên cần chọn theo dự án. Dù làm theo cách nào, phản hồi, kiểm thử và cải tiến vẫn rất quan trọng. Em cảm ơn mọi người.

## Nguồn tham khảo

- [The Scrum Guide](https://scrumguides.org/scrum-guide.html)
- [Manifesto for Agile Software Development](https://agilemanifesto.org/)
- [IBM — Software development lifecycle](https://www.ibm.com/think/topics/sdlc)
- [GitHub Docs — GitHub flow](https://docs.github.com/en/get-started/using-github/github-flow)
