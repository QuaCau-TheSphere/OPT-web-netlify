---
share: true
created: 2023-09-05T16:17
updated: 2024-06-21T21:42
---
# đối ⊷ thoại
Chương trình rút gọn liên kết cho nhu cầu quản lý và chia sẻ tài liệu phi lợi nhuận

[Để có thể thiết kế một giải pháp một cách nhanh chóng và tự tin, bạn cần được thử nghiệm ý tưởng mới và kiểm tra giả thiết ngay khi chúng vừa được nghĩ ra.](https://doi-thoai.deno.dev/hhUT.BUBw.1/ "Up and Down the Ladder of Abstraction") Nếu giải pháp đó cần sự đối thoại giữa các bên, bạn cần nhanh chóng tìm lại các cuộc thảo luận đã từng có trước đây và nắm được mức độ quan tâm của các bên liên quan. Tuy nhiên, có vẻ như hiện tại không có giải pháp nào giúp đạt được điều này. Điều này khiến cho các nỗ lực đối thoại với cộng đồng bị tủn mủn, không đạt đủ sự chú ý mà nó xứng đáng có.

Để giải quyết vấn đề đó, chương trình này sẽ giúp bạn:
- Tìm nhanh những ghi chú được chia sẻ công khai trong kho dữ liệu của bạn, hoặc các bài đăng trên các website, diễn đàn
- Quản lý và tìm nhanh những cộng đồng bạn muốn mở cuộc đối thoại
- Tự động tạo liên kết UTM để có thể sử dụng với các chương trình phân tích dữ liệu web nâng cao
- Tự động rút gọn liên kết với đuôi có ý nghĩa chứ không phải là những ký tự ngẫu nhiên 
- Tự động tạo nội dung sẽ được dùng để đối thoại dựa trên ghi chú của bạn
- Thống kê số lượng truy cập tới liên kết được chia sẻ

Hiện tại nhóm SNPO của chúng ta đã được nạp sẵn vào phần nơi đăng. Bạn chỉ cần kiếm là sẽ thấy. (Ảnh) 

# Triết lý chương trình
- Lấy nhu cầu của các tổ chức phi lợi nhuận làm trung tâm: thúc đẩy các cuộc đối thoại trong cộng đồng theo các mục tiêu phát triển bền vững, thúc đẩy sự hợp tác đa bên, liên ngành
- Dành cho người Việt: không gặp vấn đề với các ký tự tiếng Việt và kết quả được viết theo cách người Việt dùng ngôn ngữ
- Đảm bảo sự tự do và tự trị dữ liệu của người dùng: dễ dàng tích hợp với các hệ thống bạn đang dùng (VD: Obsidian)
- Hướng đến việc giáo dục công nghệ: có nhiều tài nguyên để nâng đỡ cho người còn cảm thấy lập trình là một thứ đáng sợ


Website của bạn cần có sẵn một dịch vụ phân tích web (VD: Google Analytics, Plausible) để có thể nhận dữ liệu.

---
# Lý do viết 

- Gom dữ liệu từ vault
- Việc tạo liên kết rút gọn trên bitly tốn thời gian và không bắt lỗi lúc nhập
- Copy quá nhiều

# UTM là gì
# Liên kết rút gọn
Như bạn thấy, liên kết UTM tuy giúp bạn biết được chi tiết, nhưng lại quá là dài. Các dịch vụ như bit.ly thì lại không có mẫu để quy chuẩn hoá
