# Bài 2 — Công cụ và IDE dành cho coding

> **Bản nháp:** Phần A và bảng phần B là nội dung tham khảo để bạn đọc, kiểm tra nguồn và diễn đạt lại bằng lời của mình. Phần C đã cập nhật theo thông tin bạn cho biết là đang dùng VS Code; hãy sửa các chỗ đánh dấu để khớp trải nghiệm thực tế trước khi nộp.

## Phần A — Tìm hiểu khái niệm

### 1. IDE là gì?

IDE (Integrated Development Environment) là môi trường phát triển tích hợp, gom những công cụ lập trình thường dùng vào một ứng dụng, chẳng hạn trình soạn thảo code, chạy chương trình, tìm lỗi và quản lý dự án. Notepad chủ yếu dùng để soạn văn bản, không hiểu nhiều về cấu trúc chương trình. Code editor được thiết kế để viết code và thường có tô màu cú pháp, gợi ý; có thể bổ sung thêm chức năng bằng extension. Ranh giới giữa code editor và IDE không phải lúc nào cũng tuyệt đối: một editor như Visual Studio Code có thể trở thành môi trường phát triển mạnh khi cài thêm extension.

### 2. Một số công cụ lập trình viên dùng hằng ngày

- **Terminal:** gõ lệnh để chạy chương trình, cài thư viện hoặc thao tác với Git.
- **Trình duyệt:** xem tài liệu, kiểm tra website và tìm lỗi hiển thị.
- **Git:** ghi lại lịch sử thay đổi code, tạo nhánh và phối hợp làm việc.
- **Debugger:** chạy từng bước và kiểm tra giá trị biến để tìm nguyên nhân lỗi.
- **Công cụ quản lý công việc** như GitHub Issues: ghi nhận lỗi, yêu cầu tính năng và việc cần làm.

### 3. Extension/plugin là gì?

Extension hoặc plugin là phần cài thêm để bổ sung chức năng cho IDE/editor mà không cần viết lại ứng dụng chính. Ví dụ, extension Python cho Visual Studio Code bổ sung hỗ trợ viết và chạy Python; Prettier định dạng code theo quy tắc thống nhất. Extension hữu ích nhưng nên chọn từ nguồn đáng tin cậy và chỉ cài những cái cần dùng.

## Phần B — So sánh một số công cụ

Nhận xét về mức độ nhẹ, dễ dùng và phổ biến dưới đây là so sánh định tính; hiệu năng thực tế còn tùy máy, dự án và số extension. Giá và ưu đãi có thể thay đổi, hãy mở link chính thức trước khi nộp.

| Công cụ | Giá / ưu đãi sinh viên | Dễ dùng cho người mới | Tính năng AI | Máy yếu có chạy nổi không? | Mức độ phổ biến |
|---|---|---|---|---|---|
| **Visual Studio Code** | Editor miễn phí; dịch vụ AI có gói/giới hạn riêng, không nên mặc định là miễn phí toàn bộ. | Khá dễ bắt đầu; ban đầu có thể phải tự cài extension. | Có tính năng AI của GitHub Copilot và các extension khác; quyền lợi tùy gói. | Thường phù hợp hơn IDE đầy đủ, nhưng nhiều extension hoặc dự án lớn có thể tốn RAM. | Rất phổ biến, hỗ trợ nhiều ngôn ngữ. |
| **Cursor** | Có gói miễn phí giới hạn và các gói trả phí; kiểm tra giá và điều kiện mới nhất trên trang chính thức. Chưa xác nhận ưu đãi sinh viên riêng. | Khá dễ nếu đã quen VS Code; có thể cần thời gian học cách dùng AI an toàn. | AI tích hợp để hỏi về code, gợi ý và hỗ trợ chỉnh sửa nhiều file. | Cần chạy ứng dụng cục bộ và dùng dịch vụ AI qua mạng; nên thử trực tiếp trên máy. | Đang được nhiều lập trình viên quan tâm, nhất là nhóm dùng AI hỗ trợ code. |
| **JetBrains PyCharm** | Có lựa chọn miễn phí; sinh viên đủ điều kiện có thể xin giấy phép giáo dục miễn phí theo chính sách JetBrains. | Nhiều tính năng có sẵn; giao diện có thể nhiều mục hơn editor đơn giản. | Tích hợp AI Assistant; quyền sử dụng phụ thuộc gói và chính sách hiện hành. | IDE đầy đủ thường cần tài nguyên máy nhiều hơn editor nhẹ. | Phổ biến trong cộng đồng Python và giáo dục. |
| **GitHub Codespaces** | Có hạn mức sử dụng theo tài khoản; vượt hạn mức có thể phát sinh phí. Kiểm tra quota/điều kiện hiện tại trước khi dùng. | Khá dễ bắt đầu nếu đã có repo GitHub; cần mạng ổn định. | Có thể dùng extension AI trong môi trường phát triển; không đồng nghĩa mọi tính năng AI đều miễn phí. | Code chạy trên máy chủ cloud nên đỡ phụ thuộc cấu hình máy cá nhân; cần Internet và có thể bị giới hạn quota. | Phổ biến trong các dự án làm việc trên GitHub và môi trường cloud. |

### Nhận xét ngắn

Nếu mới học trên Windows và muốn bắt đầu không tốn tiền mua IDE, Visual Studio Code là một lựa chọn đáng thử: có thể viết nhiều loại code, cài thêm chức năng khi cần và có nhiều tài liệu hướng dẫn. Đây chỉ là lựa chọn tham khảo; quyết định cuối cùng nên dựa trên cấu hình máy, ngôn ngữ học và trải nghiệm cài đặt của bạn.

## Phần C — Chọn và giải thích

> Bạn cho biết hiện đang sử dụng VS Code. Các lý do dưới đây là bản nháp dựa trên thông tin hiện có; hãy bổ sung trải nghiệm thật và ảnh chụp màn hình.

### 1. Bạn chọn công cụ nào?

Tôi chọn Visual Studio Code làm IDE/code editor để học lập trình. Hiện tôi đang sử dụng VS Code.

### 2. Vì sao chọn công cụ này?

**Bản nháp — chỉ giữ những lý do đúng với bạn; bổ sung thông tin trong ngoặc:**

1. Tôi đã quen với VS Code vì hiện đang dùng công cụ này, nên có thể tiếp tục học và thực hành mà không phải chuyển sang một môi trường mới ngay.
2. Bản editor cơ bản của VS Code miễn phí; các dịch vụ AI hoặc extension riêng có thể có điều kiện và giới hạn khác. Điều này phù hợp với ngân sách của tôi vì **[xác nhận lý do ngân sách của bạn]**.
3. Tôi có thể cài extension phù hợp với mục tiêu học **[ngôn ngữ/lĩnh vực bạn đang học]** và thêm chức năng khi cần. Máy tôi đang dùng là **[hãng/model hoặc cấu hình RAM nếu biết]** chạy **[Windows/macOS/Linux]**; sau khi dùng thử, tôi thấy VS Code **[nhận xét thật về hiệu năng]**.

### 3. Nhược điểm và khi nào sẽ đổi công cụ?

VS Code có thể cần tự tìm và cài extension cho từng ngôn ngữ; cài quá nhiều extension cũng có thể làm ứng dụng chậm hoặc giao diện rối. Nếu dự án của tôi cần nhiều công cụ chuyên sâu được tích hợp sẵn, hoặc tôi thấy editor chạy không ổn trên máy, tôi sẽ thử một IDE chuyên dụng như PyCharm. **Bổ sung nhược điểm bạn thật sự nhận thấy khi dùng:** [CẦN BẠN BỔ SUNG].

### 4. Ba extension hoặc tính năng hữu ích sau khi dùng thử

Bạn đang dùng VS Code nên hãy chọn ba extension/tính năng bạn đã thực sự thử và ghi kết quả:

1. **[Tên extension/tính năng]** — [đã thử làm gì, giúp ích thế nào?]
2. **[Tên extension/tính năng]** — [đã thử làm gì, giúp ích thế nào?]
3. **[Tên extension/tính năng]** — [đã thử làm gì, giúp ích thế nào?]

Gợi ý để thử: tìm extension Python nếu đang học Python; dùng Prettier để định dạng HTML/CSS/JavaScript; hoặc mở Terminal tích hợp và Source Control để xem cách chạy lệnh, theo dõi thay đổi. Chỉ ghi những gì bạn đã kiểm tra.

### Ảnh chụp màn hình

**[CẦN BẠN BỔ SUNG: chèn ảnh chụp màn hình IDE sau khi cài và mở một file.]**

## Nguồn tham khảo

- [Visual Studio Code — FAQ và thông tin sử dụng](https://code.visualstudio.com/docs/supporting/faq)
- [Cursor — trang chủ](https://cursor.com/) và [trang giá](https://cursor.com/pricing)
- [JetBrains — giấy phép giáo dục cho sinh viên](https://www.jetbrains.com/community/education/#students)
- [GitHub Codespaces — thông tin sản phẩm](https://github.com/features/codespaces) và [tài liệu billing](https://docs.github.com/en/billing/concepts/product-billing/github-codespaces)
- [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/vscode)

*Ngày tham khảo: 26/11/2026. Giá, quota, quyền lợi AI và điều kiện sinh viên có thể thay đổi; cần kiểm tra lại trên trang chính thức khi hoàn thiện bài.*
