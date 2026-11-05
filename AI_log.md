# AI LOG – BUỔI 7, TIẾT 3

> Điền vào `[ ... ]`, tích `[x]` vào lựa chọn phù hợp. Ghi đúng việc đã làm; chưa kiểm tra thì ghi “Chưa kiểm tra”. Không cần chép toàn bộ cuộc trò chuyện AI.

## Thông tin sinh viên

- Họ và tên: [ Đỗ Thọ CHiến  ]
- Mã sinh viên – Lớp: [ 2071020222 ]
- Ngày thực hiện: [ 30 ]
- Link repository: [ https://github.com/DoThoChien-dnu/k20_portfolio_CNTT-20-02.git ]
- URL website: [ https://dothochien-dnu.github.io/k20_portfolio_CNTT-20-02/ ]
- Tình huống: [ x ] Website của tôi  [ ] Repo luyện của giảng viên

## 1. Nhận định của tôi trước khi hỏi AI

- Trang/thao tác gặp lỗi: [Trang chủ index.html trên GitHub Pages]
- Mong muốn và hiện tượng thực tế: [ ong muốn trang web hiển thị đầy đủ giao diện và hình ảnh như chạy ở máy tính cá nhân, nhưng khi mở URL GitHub Pages thì trang bị mất CSS, giao diện trắng xóa hoặc lỗi không tải được tài nguyên ]
- Dữ kiện đã kiểm tra (cấu trúc tệp, Request URL, Status…): [ Đã nhấn F12 kiểm tra tab Network, thấy các tệp CSS/ảnh trả về mã lỗi 404 Not Found do đường dẫn tài nguyên chưa chuẩn xác theo cấu trúc thư mục của Pages ]
- Tôi nghi nguyên nhân là: [ Do đường dẫn liên kết đến tệp CSS hoặc hình ảnh trong tệp index.html đang sử dụng đường dẫn tuyệt đối bắt đầu bằng dấu gạch chéo thay vì đường dẫn tương đối ]
- Vì sao tôi nhận định như vậy: [ Vì khi chạy trực tiếp trên máy tính thì trình duyệt nhận diện được, nhưng khi đưa lên GitHub Pages, trang web nằm trong thư mục gốc của repository nên đường dẫn tuyệt đối bị lệch ]

## 2. Tôi hỏi AI và nhận được gợi ý

- Nguồn: [x] Công cụ AI: [ gemini / chatgpt ]  [ ] Phản hồi mẫu của giảng viên
- Câu hỏi/prompt tôi đã gửi (hoặc tình huống của phản hồi mẫu):

  [ Trang web portfolio của tôi sau khi deploy lên GitHub Pages bị mất CSS và báo lỗi 404 ở các tệp tài nguyên. Làm thế nào để khắc phục lỗi này? ]

- Gợi ý chính của AI:

  [AI hướng dẫn chuyển các đường dẫn tệp CSS và hình ảnh trong file index.html từ dạng tuyệt đối (ví dụ: /css/style.css) sang dạng đường dẫn tương đối (ví dụ: ./css/style.css hoặc css/style.css), sau đó commit và push lại lên GitHub.]

## 3. Quyết định của tôi

- [x] Chấp nhận gợi ý
- [ ] Chỉnh sửa gợi ý rồi áp dụng
- [ ] Bác bỏ gợi ý

- Tôi quyết định làm gì: [ Chỉnh sửa lại các đường dẫn tệp CSS và assets trong mã nguồn sang dạng tương đối, kiểm tra chạy thử ở local ]
- Lý do, dựa trên dữ kiện nào: [ Dựa trên cấu trúc thư mục thực tế của repository trên GitHub Pages, cách dùng đường dẫn tương đối giúp trình duyệt định vị đúng vị trí tệp ]

## 4. Thực hiện và kiểm chứng

- Tệp/vị trí đã sửa (không sửa thì ghi rõ): [Tệp index.html và thư mục css/]
- Nội dung thay đổi hoặc cách xử lý khác: [ Đổi các đường dẫn liên kết tệp sang dạng tương đối `./` ]
- Commit của bản sửa, nếu có: [ Cập nhật lại đường dẫn CSS và tài nguyên cho GitHub Pages ]
- Bản sửa đã deploy: [x] Có  [ ] Chưa  [ ] Không phát sinh bản sửa

| Nội dung kiểm tra | Trước xử lý | Sau xử lý/thử lại |
| --- | --- | --- |
| Request URL và Status của tài nguyên liên quan | [ Lỗi 404 Not Found ở tệp CSS ] | [ Status 200 OK, tải thành công tệp CSS ] |
| Giao diện/chức năng trên URL website | [ Giao diện bị vỡ, mất CSS ] | [ Giao diện hiển thị đầy đủ, chính xác ] |

- Cách thử lại và kết quả thực tế: [ Mở URL GitHub Pages bằng cửa sổ trình duyệt ẩn danh, kiểm tra thấy giao diện đã hiển thị bình thường ]
- Căn cứ để đối chiếu (URL tệp, commit, đường dẫn ảnh chụp hoặc dữ kiện quan sát):[ URL GitHub Pages và lịch sử commit trên repository GitHub ]

## 5. Kết luận

- [x] Đã xử lý được  [ ] Xử lý được một phần  [ ] Chưa xử lý được
- Điều tôi rút ra hoặc việc cần làm tiếp: [ Cần chú ý sử dụng đường dẫn tương đối cho các tài nguyên web khi triển khai lên các nền tảng hosting tĩnh như GitHub Pages ]

---

*Tệp là minh chứng MC2 để nhận định mức đạt của tiết học; không tính điểm MC2 riêng. Nếu có tình huống khác, sao chép mục 1–5 để ghi thêm.*
