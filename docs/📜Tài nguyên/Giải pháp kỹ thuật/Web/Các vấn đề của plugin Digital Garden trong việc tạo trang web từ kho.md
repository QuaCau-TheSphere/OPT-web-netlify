---
share: true
created: 2024-08-17T11:00
updated: 2024-08-18T13:51
---
Để tạo một website từ kho của bạn thì bạn cần 3 thứ sau:
- Một plugin để đẩy ghi chú từ máy của bạn lên GitHub
- Một chương trình tạo website từ các ghi chú
- Một dịch vụ hosting để ai cũng có thể truy cập web của bạn

Qua buổi hướng dẫn tạo web từ kho đầu tiên thì mình thấy một điểm chung là dường như các bạn đều dùng plugin **[Digital Garden](https://github.com/oleeskild/obsidian-digital-garden "oleeskild/obsidian-digital-garden")** để tạo web. Có thể là vì cái tên của nó khiến cho nó dễ được tìm đến nhất. Tuy nhiên, plugin này sử dụng **11ty** làm chương trình tạo website, và **Vercel** làm dịch vụ hosting. Mình thấy chúng có những bất cập sau:

## Digital Garden ít chức năng và ít cập nhật
Vào thời điểm viết bài, hiện tại có tới [207 vấn đề được cộng đồng gửi đến](https://github.com/oleeskild/obsidian-digital-garden/issues "Issues · oleeskild/obsidian-digital-garden"). Gần như không có cái nào được tác giả phản hồi cả. Hồi mới tập tành làm web mình cũng bắt đầu với plugin này, nhưng không dùng được vì bị lỗi tiếng Việt. [Mình có gửi vấn đề lên](https://github.com/oleeskild/obsidian-digital-garden/issues/292 "Why are there so much 404 error? · Issue #292 · oleeskild/obsidian-digital-garden") nhưng cũng chịu số phận như rất nhiều vấn đề khác. 

Mình dùng plugin [Enveloppe](https://enveloppe.github.io/) để đưa ghi chú từ máy lên GitHub và chưa thấy có điểm gì để chê. Nó có nhiều tính năng để tuỳ chỉnh, và tác giả của nó rất nhiệt tình sửa lỗi và tương tác với người dùng. Mình cũng có đóng góp cho plugin này. 

## Có những chương trình tạo web mới khắc phục được những nhược điểm của 11ty
Thực ra với nhu cầu và trình độ của người mới thì vấn đề này không ảnh hưởng lắm, vì tất cả những gì bạn cần là đọc hướng dẫn sử dụng của người dùng và chỉnh sửa duy nhất một tập tin YAML để cấu hình cho web. Bạn có thể coi như không có vấn đề này cũng được. Tầm quan trọng của việc này sẽ chỉ trở nên rõ ràng khi tất cả các plugin do cộng đồng tạo không có cái nào đáp ứng được nhu cầu của bạn, và bạn bắt buộc phải tuỳ chỉnh code của chương trình tạo web. Nếu bạn muốn tìm hiểu vấn đề này sâu hơn thì có thể đọc bài này:

Thay vì dùng 11ty, mình dùng Mkdocs Material hoặc Lume. Mkdocs Material có cộng đồng lớn, nhiều plugin, dùng thiết kế Material của Google nên thấy có vẻ ngầu ngầu, và được viết bằng Python. Mình dùng nó khi trang web cần có một thanh điều hướng tiện lợi cho người dùng, hoặc cần gây ấn tượng về mặt thiết kế. Lume thì mới hơn, và dùng Deno, một môi trường thực thi cập nhật những công nghệ mới nhất của JavaScript. Nếu mình chỉ cần tạo một trang wiki đơn giản thì mình dùng nó. Nhược điểm là chúng không có cái đồ thị liên kết các nút cho người dùng. (Thực ra Mkdocs Material cũng có một plugin, do tác giả Enveloppe viết, nhưng hình như cũng không còn được cập nhật nữa.) Nếu bạn cần có tính năng này thì mình giới thiệu Quartz, một chương trình tạo web tĩnh được viết đặc biệt dành cho người dùng Obsidian. Tuy nhiên nhược điểm của nó là mãi mà vẫn không có nút hamburger để mở menu cho người dùng điện thoại.

## Dịch vụ hosting Vercel hoặc Netlify là những dao mổ trâu giết gà
GitHub Page đơn giản hơn và phù hợp cho nhu cầu cơ bản của bạn. Tất nhiên, sau khi thành thạo rồi bạn sẽ thấy các dịch vụ này cho bạn nhiều tính năng hay ho hơn rất nhiều. Đến cả mình, sau khi dùng Netlify một thời gian, đủ để tạm hiểu nó và thấy GitHub Page ít chức năng thật, thì mình vẫn chuyển các trang web của mình từ Netlify về lại GitHub Page, vì mình vẫn thấy chưa thực sự cần tới những tính năng mà chỉ chúng mới có. Hồi mới lớ ngớ làm web mình dùng Netlify không cẩn thận nên bị nó mổ mất mấy chục đô rồi. Ở GitHub Page thì không lo chuyện đó.

## Hướng dẫn sử dụng bỏ qua bước tạo website trên trên máy bạn
Nếu mục đích là làm sao để tạo website cho nhanh để mà còn làm việc khác thì đúng là bạn sẽ không cần phải tạo web trên máy mình. Nhưng theo mình thì đây là bước giúp bạn vỡ ra được nhiều thứ về cách hoạt động của một trang web, vì nó sẽ đòi hỏi bạn cần dùng Git để quản lý phiên bản và terminal để ra lệnh cho các tất cả các chương trình liên quan. Khi bạn tuỳ chỉnh website, bạn sẽ phải thao tác trên tập tin cấu hình (VD: `mkdocs.yaml`, `_config.js`) cũng như sắp xếp các thư mục cho các tập tin bổ trợ, và chắc chắn bạn sẽ phải xử lý nó trên máy của bạn trước. Kể cả khi bạn không cần làm việc đó thì nó cũng tiện lợi và an toàn hơn là đẩy trực tiếp lên hosting.