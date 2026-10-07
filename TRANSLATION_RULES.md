# Quy tắc dịch tiếng Việt

Áp dụng cho tài liệu Markdown trong `vandunxg/java-design-patterns`. Đọc file này trước khi dịch hoặc rà soát bản dịch. Các yêu cầu về nội dung và cấu trúc bên dưới là bắt buộc; không cần tạo thêm quy trình QA nhiều vòng.

## Mục tiêu

Tạo bản tiếng Việt đầy đủ, chính xác và tự nhiên, giữ đúng ý đồ của tài liệu nguồn và giúp người đọc hiểu cách hoạt động của từng design pattern.

- Dịch từ file tiếng Anh hiện có trong đúng revision được giao. Không dịch từ trí nhớ hay tự bổ sung kiến thức.
- Không sửa nội dung nguồn tiếng Anh.
- Dịch đầy đủ nội dung dành cho người đọc; không tóm tắt, bỏ ví dụ, đổi thứ tự hoặc thêm giải thích của người dịch.
- Viết tiếng Việt gọn, rõ, đúng ngữ cảnh kỹ thuật. Giữ nguyên thuật ngữ tiếng Anh khi đó là tên chuẩn, tên API hoặc cách gọi phổ biến; không dịch máy móc từng từ.
- Không sửa nhận định hoặc lỗi có thể có trong nguồn. Nếu gặp chỗ nguồn mơ hồ đến mức không thể dịch chắc chắn, ghi rõ vị trí trong kết quả bàn giao thay vì đoán.

## Phạm vi và đầu ra

- Chỉ dịch tài liệu Markdown được giao, thường là `README.md` của một pattern hoặc tài liệu tổng quan.
- Đặt bản dịch dưới `translations/vi/` với cùng đường dẫn tương đối. Ví dụ: `builder/README.md` → `translations/vi/builder/README.md`.
- Không dịch hoặc chỉnh sửa Java code, test, build file, tên package, class, method, biến, cấu hình hay output chương trình. Chỉ dịch code comment khi task ghi rõ.
- Chỉ sửa file đích được giao. Không sửa README nguồn, tài liệu pattern khác, website, workflow hoặc cấu hình deploy nếu task không yêu cầu.
- Nếu file đích đã tồn tại, cập nhật đúng file đó; giữ các thay đổi sẵn có ngoài phạm vi được giao.

## Giữ cấu trúc và nội dung kỹ thuật

Giữ nguyên ý nghĩa và thứ tự của tiêu đề, đoạn văn, danh sách, bảng, cảnh báo, ví dụ, liên kết, hình ảnh, sơ đồ và các phần như Intent, Explanation, Applicability, Real World Examples.

Giữ nguyên chính xác:

- code, cú pháp, tên pattern, tên class/interface/method, identifier và chuỗi mà chương trình hiển thị;
- lệnh, đường dẫn, URL, anchor, tên file, tên thuộc tính Markdown/HTML và metadata máy đọc;
- số liệu, điều kiện, quan hệ nhân quả, mức độ chắc chắn và mức khuyến nghị trong nguồn.

Dịch văn bản hiển thị cho người đọc, kể cả tiêu đề, nhãn, mô tả bảng, chú thích và alt text. Trong code fence, giữ code nguyên trạng. Không dịch nội dung có thể được sao chép hoặc thực thi.

## Thuật ngữ

- Giữ nguyên tên design pattern chuẩn bằng tiếng Anh; có thể thêm cách gọi tiếng Việt ở lần xuất hiện đầu nếu tự nhiên và hữu ích.
- Giữ nguyên tên công nghệ, Java API, tên thư viện, class và identifier.
- Dùng nhất quán một cách gọi trong cùng tài liệu. Chỉ thêm mục vào glossary khi thuật ngữ cần thống nhất giữa nhiều file; không tạo glossary chỉ để ghi các thuật ngữ hiển nhiên.
- Không thêm chú giải cho mọi thuật ngữ tiếng Anh. Chỉ giải thích khi nguồn có giải thích hoặc nếu thiếu giải thích khiến câu dịch khó hiểu.

## Quy trình dịch một file

1. Đọc trọn file nguồn được giao và xác định file đích tương ứng.
2. Dịch toàn bộ nội dung theo các quy tắc trên, giữ cấu trúc và các thành phần kỹ thuật.
3. Tự đối chiếu một lượt với nguồn trước khi bàn giao: kiểm tra không bỏ sót nội dung, không thêm ý, và code/link/markup không bị đổi.
4. Bàn giao file dịch cùng đường dẫn nguồn và ghi chú ngắn nếu có điểm mơ hồ. Không tạo báo cáo dài hay chạy nhiều vòng tự kiểm tra.

## Review nhẹ

Reviewer chỉ làm một lượt đối chiếu file dịch với file nguồn và quy tắc này.

- Chỉ tìm lỗi có thể chỉ ra cụ thể: thiếu/thừa nội dung, sai hoặc lệch ý, thuật ngữ dùng sai/ngược nhau, câu tiếng Việt khó hiểu do vi phạm quy tắc, hoặc code/link/markup bị thay đổi.
- Nếu thấy lỗi, sửa trực tiếp đúng chỗ trong file được giao. Không dịch lại toàn file và không mở rộng sang code hay tài liệu khác.
- Không yêu cầu sửa chỉ vì reviewer thích một cách viết khác nếu câu hiện tại đã tự nhiên, rõ nghĩa và đúng rule.
- Không lặp lại các bước rà soát đã làm; sau khi sửa, chỉ kiểm tra lại đoạn vừa sửa và phần cấu trúc/kỹ thuật bị ảnh hưởng.
- Nếu không có lỗi thuộc các tiêu chí trên, xác nhận đạt. Không yêu cầu vòng review tiếp theo.

## Hoàn tất

Một file đạt khi bản dịch đầy đủ, đúng ý, tự nhiên, giữ cấu trúc và thành phần kỹ thuật, không có lỗi rõ ràng theo mục Review nhẹ. Không yêu cầu checklist dài, điểm số, bản dịch thứ hai, hay review độc lập nhiều vòng.
