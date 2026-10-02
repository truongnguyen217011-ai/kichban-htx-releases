# KICHBAN HTX Releases

Kho công khai này chỉ chứa bộ cài Windows, mã kiểm tra SHA-256 và manifest cập nhật đã ký số. Mã nguồn của ứng dụng không được phát hành tại đây.

Phiên bản mới nhất: **0.1.44**.

Từ 0.1.26, ứng dụng có khay hệ thống Windows thật và tự kiểm tra cập nhật định kỳ khi đang chạy. Bản 0.1.27 hoàn thiện Content/Hook/SEO, prompt ảnh/thumbnail/Veo theo DNA và chỉ dẫn huấn luyện mới; làm mới cache/UI cho tác vụ mới, đồng thời bổ sung lớp bảo vệ SQLite: phát hiện hỏng trước ghi, khóa một runtime, snapshot có checksum/xác minh và backup/restore đầy đủ dữ liệu nghiệp vụ.

Bản 0.1.33 hợp nhất các sửa đổi mới nhất cho Viết đơn/Hàng loạt/Trend, QA/JSON/Hook/độ dài, dừng tác vụ, prompt ảnh còn thiếu, DNA và nhận dạng nhân vật, hồ sơ kênh và thư mục đầu ra theo kênh.

Bản 0.1.34 bổ sung file content chia đúng theo từng cue SRT AI33 nhưng không có timestamp, đồng thời sửa launcher để không còn giao diện HTML thô do thiếu tài nguyên static.

Từ phiên bản 0.1.3, ứng dụng tự kiểm tra chữ ký, tải và cài bản cập nhật hợp lệ khi khởi động.

Bản 0.1.36 sửa tận gốc các lỗi lặp lại: dữ liệu cố định ở D:\HTX\data và tự chuyển từ bản cũ ở lần mở đầu; kịch bản do Claude chấm theo tiêu chí có trích dẫn (Gemini viết), giữ đúng tiêu đề bạn nhập ở hàng loạt; SEO tự bổ sung phần thiếu; prompt ảnh/Veo cho bài 9 phút chạy song song trong khoảng 2 phút; AI33 chỉ tạo một task trả phí mỗi voice; bộ cài tự đóng app đang chạy và luôn giữ dữ liệu khi gỡ.

Bản 0.1.37 thêm khóa DNA nhân vật theo từng kênh: tải ảnh tham chiếu vào hồ sơ kênh, AI đọc ảnh một lần, bạn sửa và bấm "Duyệt & khóa"; mọi tập dùng nguyên văn mô tả đã duyệt trong prompt ảnh, Veo và thumbnail. Kênh đã có ảnh tham chiếu từ trước cần bấm "Duyệt & khóa" một lần.

Bản 0.1.38 thêm chọn và xóa tác vụ ở trang Tác vụ (ô chọn, "Chọn tất cả", "Xóa đã chọn"); tác vụ đang chạy được dừng trước, file thành phẩm trên ổ được giữ nguyên và app tự sao lưu dữ liệu trước khi xóa.

Bản 0.1.39: ảnh tham chiếu nhân vật chính quyết định **loại hình + nét vẽ** cho mọi nhân vật (prompt ảnh, Veo, thumbnail), đè phong cách của kênh lead — khóa ảnh người que thì ra người que. Kênh phải khóa ảnh nhân vật chính (Hồ sơ kênh → bước 3 → chọn loại hình, nét vẽ → "Duyệt & khóa") mới tạo được prompt ảnh; kênh đã khóa ở 0.1.37–0.1.38 cần duyệt lại một lần. Mỗi kênh có thể đặt thư mục gốc đầu ra riêng; đổi kênh là đường dẫn đầu ra đổi theo.

Bản 0.1.40: viết kịch bản không còn kẹt ở QA — chương đạt từ 80 điểm (75–79 hoàn tất kèm cảnh báo "QA gần đạt"), tool tự đưa bài về đúng độ dài trước khi chấm, và sửa lỗi chấm "mạch văn" từng chặn nhầm bài. Kiểm số từ, hook, SEO, ngôn ngữ vẫn giữ chặt.

Bản 0.1.41: hồ sơ kênh đã lưu gì thì dùng đúng cái đó — lưu/duyệt DNA hay phân tích lại kênh lead không còn đè số phút, WPM, ngách, ngôn ngữ đã lưu bằng gợi ý của DNA. Hồ sơ từng bị đè: nhập lại số phút/WPM và bấm "Lưu hồ sơ" một lần.

Bản 0.1.42: hết kẹt SEO "tiêu đề chưa theo công thức tiêu đề của DNA kênh" (chỉ công thức dạng khuôn mới chấm cứng, công thức mô tả bằng lời chỉ cảnh báo); chọn model chấm QA bất kỳ kèm danh sách dự phòng theo thứ tự trong Cấu hình; hết báo nhầm "9Router hết hạn mức" — lỗi khác hiện nguyên lỗi thật kèm tên model, có nút "Thử lại ngay".

Bản 0.1.43: hết kẹt QA — tool giữ cách "sửa đúng câu bị chỉ ra" khi điểm còn tăng, giám khảo nhớ lỗi đã sửa; viết đơn dưới 75 có nút "Chấp nhận bản tốt nhất" (xong là có nút "Tạo voice & SRT"), hàng loạt/trend tự chấp nhận khi chương thấp nhất từ 60 và chạy tiếp voice/SRT/prompt ảnh.

Bản 0.1.44: cập nhật tự chờ bài đang chạy xong; không mất bài khi chuyển tác vụ; mỗi câu SRT có 1 prompt ảnh + 1 prompt Veo, mọi người trong cảnh vẽ là nhân vật chính đã khóa, prompt bám đúng câu đang nói; bước chỉnh độ dài gộp (bài 10 phút ~9 lần gọi model viết); lỗi nhà cung cấp báo rõ giờ mở lại. Máy đang dùng bản cũ: cập nhật khi không có bài nào đang chạy.
