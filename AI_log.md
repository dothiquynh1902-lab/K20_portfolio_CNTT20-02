# AI LOG – BUỔI 7, TIẾT 3

> Điền vào `[ ... ]`, tích `[x]` vào lựa chọn phù hợp. Ghi đúng việc đã làm; chưa kiểm tra thì ghi “Chưa kiểm tra”. Không cần chép toàn bộ cuộc trò chuyện AI.

## Thông tin sinh viên

- Họ và tên: Đỗ Thị Quỳnh
- Mã sinh viên – Lớp: 2071020163 - CNTT20-02
- Ngày thực hiện: 30/10/2026
- Link repository: https://github.com/dothiquynh1902-lab/K20_portfolio_CNTT20-02.git
- URL website: https://dothiquynh1902-lab.github.io/K20_portfolio_CNTT20-02/
- Tình huống: [x] Website của tôi  [ ] Repo luyện của giảng viên

## 1. Nhận định của tôi trước khi hỏi AI

- Trang/thao tác gặp lỗi:  Trang chủ (index.html) phần tiêu đề và bố cục bị lệch hẳn sang một bên, các thẻ bên dưới hiển thị sai định dạng.
- Mong muốn và hiện tượng thực tế: Mong muốn trang web hiển thị đúng cấu trúc các khối như đã học. Thực tế là thanh điều khiển bị tràn ra ngoài và chữ không xuống dòng đúng chỗ.
- Dữ kiện đã kiểm tra (cấu trúc tệp, Request URL, Status…): Đã mở file index.html nhưng chưa tìm ra chỗ sai vì mã nguồn khá dài và nhiều thẻ lồng nhau. Không thấy thông báo lỗi đỏ trong Console của trình duyệt.
- Tôi nghi nguyên nhân là: Có thể viết nhầm hoặc quên đóng thẻ HTML nào đó.
- Vì sao tôi nhận định như vậy: Tôi vừa mới copy một đoạn code trên mạng dán vào nhưng quên kiểm tra lại các thẻ mở và thẻ đóng.

## 2. Tôi hỏi AI và nhận được gợi ý

- Nguồn: [x] Công cụ AI: Gemini [ ] Phản hồi mẫu của giảng viên
- Câu hỏi/prompt tôi đã gửi (hoặc tình huống của phản hồi mẫu):

  Xem giúp tôi lỗi ở ảnh này

- Gợi ý chính của AI:

  Bạn quên viết thẻ đóng </div> cho khối <div class="container">, khiến tất cả các phần tử bên dưới bị dồn vào chung một khối và bị CSS đè lên làm lệch giao diện.

## 3. Quyết định của tôi

- [x] Chấp nhận gợi ý
- [x] Chỉnh sửa gợi ý rồi áp dụng
- [ ] Bác bỏ gợi ý

- Tôi quyết định làm gì:  Làm như AI gợi ý
- Lý do, dựa trên dữ kiện nào: Triệu chứng bố cục bị lệch và các phần tử bị dồn vào nhau phù hợp với khả năng thiếu thẻ đóng. Tôi đã kiểm tra lại cấu trúc HTML và áp dụng gợi ý đóng khối container đúng vị trí.

## 4. Thực hiện và kiểm chứng

- Tệp/vị trí đã sửa (không sửa thì ghi rõ): Đã rà soát `index.html`, đặc biệt các thẻ `<div class="container">` trong trang chủ. Mã nguồn hiện tại có thẻ đóng cho các khối này.
- Nội dung thay đổi hoặc cách xử lý khác: Theo ghi nhận khi xử lý, đã áp dụng gợi ý kiểm tra/đóng thẻ `</div>` đúng vị trí. Tuy nhiên, lịch sử Git hiện có không cho thấy thay đổi cụ thể về thẻ đóng để xác nhận lần sửa bố cục; các thay đổi `index.html` có thể đối chiếu được chủ yếu là cập nhật thông tin cá nhân và nội dung portfolio.
- Commit của bản sửa, nếu có: Chưa xác nhận được commit riêng cho lỗi bố cục. Các commit gần đây của `index.html` gồm `42561b8`, `005a2dd` và `134fe00`, chủ yếu cập nhật thông tin portfolio.
- Bản sửa đã deploy: [x] Có  [] Chưa  [ ] Không phát sinh bản sửa (chưa xác minh trạng thái deploy)

| Nội dung kiểm tra | Trước xử lý | Sau xử lý/thử lại |
| --- | --- | --- |
| Request URL và Status của tài nguyên liên quan | Chưa kiểm tra/lưu lại | Chưa kiểm tra |
| Giao diện/chức năng trên URL website | Ghi nhận trang chủ bị lệch bố cục, thanh điều hướng tràn và chữ xuống dòng sai; chưa lưu ảnh kiểm chứng | Chưa kiểm tra lại trên URL website |

- Cách thử lại và kết quả thực tế: Chưa thử lại trên trình duyệt sau khi sửa; cần mở trang chủ, kiểm tra bố cục ở màn hình rộng và màn hình nhỏ, đồng thời xem Console/Network nếu lỗi còn xuất hiện.
- Căn cứ để đối chiếu (URL tệp, commit, đường dẫn ảnh chụp hoặc dữ kiện quan sát): Cấu trúc trang trong `index.html`; URL website dự kiến: https://dothiquynh1902-lab.github.io/K20_portfolio_CNTT20-02/ (chưa xác minh bản deploy sau sửa). Chưa có ảnh chụp trước/sau.

## 5. Kết luận

- [ ] Đã xử lý được  [x] Xử lý được một phần  [ ] Chưa xử lý được
- Điều tôi rút ra hoặc việc cần làm tiếp: Cần đóng các thẻ HTML đúng cấp và kiểm tra lại cấu trúc sau khi chỉnh sửa. Việc tiếp theo là mở website trên trình duyệt, kiểm tra giao diện ở nhiều kích thước màn hình và xác nhận bản sửa đã được deploy.

---

*Tệp là minh chứng MC2 để nhận định mức đạt của tiết học; không tính điểm MC2 riêng. Nếu có tình huống khác, sao chép mục 1–5 để ghi thêm.*
