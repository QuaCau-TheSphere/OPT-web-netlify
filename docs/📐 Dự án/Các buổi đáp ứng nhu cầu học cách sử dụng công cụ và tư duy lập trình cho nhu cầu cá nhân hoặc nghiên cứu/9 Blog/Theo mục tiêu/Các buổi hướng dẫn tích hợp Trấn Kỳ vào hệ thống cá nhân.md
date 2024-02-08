---
share: true
created: 2023-09-05T16:17
updated: 2024-02-07T00:52
title: Tích hợp Trấn Kỳ vào hệ thống của bạn
description: Nhập dữ liệu và tạo bảng phân loại ngay trên hệ thống bạn đang dùng
alias:
  - Tích hợp Trấn Kỳ vào hệ thống cá nhân
  - Nhập dữ liệu và tạo bảng phân loại ngay trên hệ thống bạn đang dùng
  - Các buổi hướng dẫn tích hợp Trấn Kỳ vào hệ thống cá nhân
---

Nếu bạn đang tìm một chương trình:
- [x] Tự động phân loại, gắn nhãn thông tin chứ không bắt bạn phải tự xử lý
- [x] Cho phép bạn khai báo dữ liệu theo thói quen và cách phân loại của chính mình
- [x] Tích hợp được vào hệ thống vận hành hiện tại của bạn:
  - Đầu vào: báo cáo ngân hàng, hoá đơn bán lẻ, Google Keep, Discord, Telegram, Zalo, Messenger, v.v.
  - Đầu ra: Google Sheet, Notion, Obsidian, Fibery, Odoo, SQL, v.v. 
- [x] Không giam dữ liệu của bạn tại chương trình 
- [x] Không có bất cứ quảng cáo mời mọc hoặc theo dõi dữ liệu nào
- [x] Dùng được trên điện thoại khi không có mạng
- [x] Là phần mềm tự do và mã nguồn mở

Thì Trấn Kỳ CLI là dành cho bạn.

![Giao diện khởi động của Trấn Kỳ CLI](https://i.imgur.com/rBe2iQ9.png)

## Nhập dữ liệu và tạo bảng phân loại ngay trên hệ thống bạn đang dùng
Ví dụ, Google Keep là một phần mềm ghi chú rất phổ biến với mọi người. Nó:
- Có trên iOS, Android và web
- Mở rất nhanh và có thể mở trong tình trạng không có mạng
- Đồng bộ nhanh chóng trên tất cả các thiết bị
- Hoàn toàn miễn phí
- Cho phép nhiều người cùng chỉnh sửa một ghi chú
- Sử dụng giọng nói
- Nhập số lượng lớn

Việc có thể nhập liệu từ Google Keep sẽ giúp cho bạn có thể nhập nhanh những khoảng chi tiêu chung với khối lượng lớn vào lúc bạn không có đầu óc để phân loại, phù hợp cho gia đình, nhóm bạn, công ty những lúc chợ búa, du lịch, tổ chức sự kiện, v.v.

Hiện tại đã có sẵn plugin nhập dữ liệu từ Google Keep và tạo bảng phân loại trên Fibery. Bạn có thể tự viết những plugin khác cho phù hợp với bạn.
![Keep to Fibery.png](../../../../assets/attachments/Keep%20to%20FIbery.png)

## Các tính năng hỗ trợ khác (a.k.a. yêu cầu phi chức năng) 
- **Viết cho người Việt** nên:
	- Xử lý được từ ghép và [các cách đặt dấu thanh khác nhau](Ti%E1%BA%BFng%20Vi%E1%BB%87t%20c%C3%B3%202%20c%C3%A1ch%20%C4%91%E1%BA%B7t%20d%E1%BA%A5u%20thanh.md)
	- Tên biến, tên hàm hoàn toàn bằng tiếng Việt
- **Viết cho người cần sử dụng trên các webapp khác** như Fibery, Google Sheet nên:
	- Chỉ sử dụng JavaScript thuần 
	- Đảm bảo regex không chạy lâu
	- Có sẵn build script để chuyển từ TypeScript sang JavaScript
- **Viết cho người không muốn bị ràng buộc vào một nền tảng nào** nên sẽ là một chương trình mã nguồn mở và tự do
- **Viết cho người phải tự học lập trình** nên:
	- Có rất nhiều ghi chú, hướng dẫn để cung cấp các khái niệm thiết yếu, giúp bạn xây dựng mental model cho code, để bạn hiểu được cái cách một lập trình viên kiến trúc nên một chương trình thế nào
	- Tên commit cố gắng tuân thủ [conventional commit](https://www.conventionalcommits.org/en/v1.0.0/)
	- Có script kiểm thử

> [!Important] Vault Obsidian *Tiếp thị số, xử lý dữ liệu và lập trình*
> Trong quá trình viết Trấn Kỳ, Đây là vault bổ sung cho [Obsidian, quản lý dự án và công cụ nghĩ](https://obsidian.xn--qucu-hr5aza.cc/?utm_source=CW+%C2%BB+X%E1%BB%AD+l%C3%BD+d%E1%BB%AF+li%E1%BB%87u+v%C3%A0+l%E1%BA%ADp+tr%C3%ACnh&utm_campaign=C+H%E1%BB%97+tr%E1%BB%A3+ng%C6%B0%E1%BB%9Di+t%E1%BB%B1+h%E1%BB%8Dc+qu%E1%BA%A3n+l%C3%BD+d%E1%BB%B1+%C3%A1n+ho%E1%BA%B7c+ki%E1%BA%BFn+th%E1%BB%A9c&utm_term=%C4%90%E1%BB%8Dc+b%C3%A0i+vi%E1%BA%BFt+tr%C3%AAn+web "Obsidian, quản lý dự án và công cụ nghĩ"), tập trung vào việc xử lý dữ liệu và lập trình. Nó được sinh ra trong quá trình bọn mình viết [Trấn Kỳ]([https://xn--lptrnh-zva6402d.xn--qucu-hr5aza.cc/👏Trấn](https://xn--lptrnh-zva6402d.xn--qucu-hr5aza.cc/%F0%9F%91%8FTr%E1%BA%A5n) Kỳ/ "Trấn Kỳ"), và cũng được sử dụng như tài liệu hướng dẫn cho nó. Nếu bạn muốn tìm một nguồn tài liệu để học một cách bài bản thì không nên vào đây. Nhưng nếu mục tiêu của bạn là làm xong những công việc khác, mà để làm được chúng trôi chảy bạn phải học lập trình, và bạn muốn tìm những bài viết thật ngắn nhưng đủ để hiểu khái niệm để còn làm việc được tiếp (như khi bọn mình cần phải học để còn viết xong Trấn Kỳ), thì có thể một số thứ trong đây sẽ hữu ích cho bạn.

## Các buổi hướng dẫn sử dụng Trấn Kỳ CLI
Vậy, nếu bạn có mong muốn hiện thực hoá điều này, Quả Cầu sẽ cung cấp cho bạn cơ hội để hợp tác thực hiện thông qua việc đăng ký nhu cầu và tự định giá nhu cầu trong phiếu đăng ký dưới đây. 

Về vấn đề đăng ký nhu cầu, Quả Cầu khuyến khích bạn nêu rõ lý do bạn muốn tham gia và đồng thời **thiết kế lộ trình làm việc và kết quả đầu ra** phù hợp với nhu cầu phát triển dự án cá nhân của bạn (nếu có) dựa trên gợi ý như sau:
- Thời gian: 1 buổi (3-4 tiếng online/offline) để bạn cài đặt và hiểu công cụ + 2 tuần sau buổi đào tạo đầu tiên (hỗ trợ qua chat mỗi ngày và 2 buổi gặp mặt online/offline) để Quả Cầu trao đổi, tư vấn với bạn trong việc ứng dụng công cụ cho dự án cá nhân. 
- Nội dung:
    - Cài đặt và sử dụng các công cụ, ngôn ngữ lập trình (VS Code, Git, PowerShell, TypeScript) 
    - Chạy Trấn Kỳ trên terminal
    - Hiểu về vật thể và API
    - Viết API để tích hợp vào hệ thống của bạn. Hiểu điều IDE đang cố gắng nói cho mình

Về vấn đề tự định giá, Quả Cầu cho rằng **bạn nên được quyền quyết định giá trị của buổi hướng dẫn** vì đây là dự án phục vụ nhu cầu và dựa trên thiết kế lộ trình làm việc của bạn. Với nhu cầu và thiết kế đó, Quả Cầu khuyến khích bạn đề xuất giá trị của buổi hướng dẫn này với đa dạng hình thức chi trả/trao đổi nhu cầu (ví dụ: tiền hoặc các tác vụ hỗ trợ Quả Cầu theo thoả thuận).

Sau khi xem xét các đăng ký, Quả Cầu sẽ lựa chọn để trao đổi và hợp tác với những nhu cầu phù hợp.

Đọc thêm các bài sau đây để hiểu hơn về ý tưởng này:
- [Khi nào thì chiến lược định giá "trả tuỳ tâm" đạt được sự bền vững?](../M%C3%B4%20h%C3%ACnh%20kinh%20doanh%20c%E1%BB%A7a%20c%C3%A1c%20bu%E1%BB%95i%20%C4%91%C3%A1p%20%E1%BB%A9ng%20nhu%20c%E1%BA%A7u%20h%E1%BB%8Dc%20c%C3%A1ch%20s%E1%BB%AD%20d%E1%BB%A5ng%20c%C3%B4ng%20c%E1%BB%A5%20v%C3%A0%20t%C6%B0%20duy%20l%E1%BA%ADp%20tr%C3%ACnh.md)
- [Các buổi đáp ứng nhu cầu học cách sử dụng công cụ và tư duy lập trình cho nhu cầu công việc](../C%C3%A1c%20bu%E1%BB%95i%20%C4%91%C3%A1p%20%E1%BB%A9ng%20nhu%20c%E1%BA%A7u%20h%E1%BB%8Dc%20c%C3%A1ch%20s%E1%BB%AD%20d%E1%BB%A5ng%20c%C3%B4ng%20c%E1%BB%A5%20v%C3%A0%20t%C6%B0%20duy%20l%E1%BA%ADp%20tr%C3%ACnh%20cho%20nhu%20c%E1%BA%A7u%20c%C3%B4ng%20vi%E1%BB%87c.md)
- [Lý do viết Trấn Kỳ](../../../Tr%E1%BA%A5n%20K%E1%BB%B3/9%20Blog/L%C3%BD%20do%20vi%E1%BA%BFt%20Tr%E1%BA%A5n%20K%E1%BB%B3.md)

Thông tin liên hệ:

- **Facebook:** [https://www.facebook.com/qua.cau.the.sphere](https://www.facebook.com/qua.cau.the.sphere)
- **Email:** quacau.thesphere@gmail.com

Rất mong được đồng hành cùng bạn.

[Giả thiết về tiếp nhận của người đọc bài giới thiệu buổi hướng dẫn cụ thể](../../2%20Gi%E1%BA%A3%20thuy%E1%BA%BFt/Gi%E1%BA%A3%20thi%E1%BA%BFt%20v%E1%BB%81%20ti%E1%BA%BFp%20nh%E1%BA%ADn%20c%E1%BB%A7a%20ng%C6%B0%E1%BB%9Di%20%C4%91%E1%BB%8Dc%20b%C3%A0i%20gi%E1%BB%9Bi%20thi%E1%BB%87u%20bu%E1%BB%95i%20h%C6%B0%E1%BB%9Bng%20d%E1%BA%ABn%20c%E1%BB%A5%20th%E1%BB%83.md)