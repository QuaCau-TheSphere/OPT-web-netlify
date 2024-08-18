---
share: true
created: 2024-08-17T11:00
updated: 2024-08-18T21:41
---
Nếu bạn không muốn mua gói Publish nhưng vẫn muốn tạo một website từ kho của bạn thì bạn cần 3 thứ sau:
- Một plugin để đẩy ghi chú từ máy của bạn lên GitHub
- Một chương trình tạo website từ các ghi chú
- Một dịch vụ hosting để ai cũng có thể truy cập web của bạn

Qua buổi hướng dẫn tạo web từ kho đầu tiên thì mình thấy một điểm chung là dường như các bạn đều dùng plugin **[Digital Garden](https://github.com/oleeskild/obsidian-digital-garden "oleeskild/obsidian-digital-garden")** để tạo web. Có thể là vì cái tên của nó khiến cho nó dễ được tìm đến nhất. Tuy nhiên, plugin này sử dụng **11ty** làm chương trình tạo website, và **Vercel** làm dịch vụ hosting. Mình thấy chúng có những bất cập sau:

## Digital Garden ít chức năng và ít cập nhật
Vào thời điểm viết bài, hiện tại có tới [207 vấn đề được cộng đồng gửi đến](https://github.com/oleeskild/obsidian-digital-garden/issues "Issues · oleeskild/obsidian-digital-garden"). Gần như không có cái nào được tác giả phản hồi cả. Hồi mới tập tành làm web mình cũng bắt đầu với plugin này, nhưng không dùng được vì bị lỗi tiếng Việt. [Mình có gửi vấn đề lên](https://github.com/oleeskild/obsidian-digital-garden/issues/292 "Why are there so much 404 error? · Issue #292 · oleeskild/obsidian-digital-garden") nhưng cũng chịu số phận như rất nhiều vấn đề khác. 

Mình dùng plugin [Enveloppe](https://enveloppe.github.io/) để đưa ghi chú từ máy lên GitHub và chưa thấy có điểm gì để chê. Nó có nhiều tính năng để tuỳ chỉnh, và tác giả của nó rất nhiệt tình sửa lỗi và tương tác với người dùng. Mình cũng có đóng góp cho plugin này. 

## Dịch vụ hosting Vercel hoặc Netlify là những dao mổ trâu giết gà
GitHub Page đơn giản hơn và phù hợp cho nhu cầu cơ bản của bạn. Tất nhiên, sau khi thành thạo rồi bạn sẽ thấy các dịch vụ này cho bạn nhiều tính năng hay ho hơn rất nhiều. Đến cả mình, sau khi dùng Netlify một thời gian, đủ để tạm hiểu nó và thấy GitHub Page ít chức năng thật, thì mình vẫn chuyển các trang web của mình từ Netlify về lại GitHub Page, vì mình vẫn thấy chưa thực sự cần tới những tính năng mà chỉ chúng mới có. Hồi mới lớ ngớ làm web mình dùng Netlify không cẩn thận nên bị nó mổ mất mấy chục đô rồi. Ở GitHub Page thì không lo chuyện đó.

## Hướng dẫn sử dụng bỏ qua bước tạo website trên trên máy bạn
Nếu mục đích là làm sao để tạo website cho nhanh để mà còn làm việc khác thì đúng là bạn sẽ không cần phải tạo web trên máy mình. Nhưng theo mình thì đây là bước giúp bạn vỡ ra được nhiều thứ về cách hoạt động của một trang web, vì nó sẽ đòi hỏi bạn cần dùng Git để quản lý phiên bản và terminal để ra lệnh cho các tất cả các chương trình liên quan. Khi bạn tuỳ chỉnh website, bạn sẽ phải thao tác trên tập tin cấu hình cũng như sắp xếp các thư mục cho các tập tin bổ trợ, và chắc chắn bạn sẽ phải xử lý nó trên máy của bạn trước. Kể cả khi bạn không cần làm việc đó thì nó cũng tiện lợi và an toàn hơn là đẩy trực tiếp lên hosting. 

## Có những chương trình tạo web mới khắc phục được những nhược điểm của 11ty
11ty dùng một môi trường thực thi tên là Node và nhập plugin bằng CommonJS. CommonJS thì lạc hậu, Node thì bất tiện với người dùng mới. Dưới đây là 3 chương trình tạo web tĩnh mình nghĩ sẽ tốt hơn 11ty:

> [!Attention] Phạm vi các ưu điểm và nhược điểm
> Ưu điểm và nhược điểm của các chương trình mình giới thiệu chỉ ở vấn đề kỹ thuật, và hướng đến những người có nhu cầu tạo web cá nhân từ kho. Có thể còn nhiều ưu điểm và nhược điểm khác, hoặc là với người có nhu cầu này là ưu điểm còn với người có nhu cầu kia là nhược điểm, nhưng nếu mình xét thấy không hữu ích cho người có nhu cầu tạo web cá nhân từ kho thì mình sẽ không nhắc tới.

### Mkdocs
Mkdocs được viết bằng Python, một ngôn ngữ đề cao việc dễ đọc, dễ viết. Đặc biệt, theme Material của nó dùng thiết kế Material của Google, là một kiểu thiết kế phẳng theo nhiều lớp để tạo độ sâu. Nó phù hợp khi bạn cần một trang web có một thanh điều hướng với nhiều nút, đủ đơn giản để không làm rối, nhưng lại không quá đơn giản để tạo ra được một giao diện ấn tượng với người dùng. 

Ưu điểm:
- Tập tin cấu hình `mkdocs.yml` là một tập tin YAML quen thuộc, không phải code gì cả
- Số lượng tính năng phong phú, đặc biệt là có nhiều kiểu markdown cho các nhu cầu đặc thù

### Lume
Phù hợp cho các trang blog hoặc wiki đơn giản.

Ưu điểm:
- Với mỗi thư mục bạn có thể đặt một tập tin cấu hình `_data.yaml` để cấu hình cho toàn bộ thư mục. Nếu bạn muốn một thư mục con có cấu hình khác thì chỉ cần tạo một tập tin `_data.yaml` khác vào trong thư mục con đó
- Trong trường hợp bạn phải chỉnh code, thì Lume dùng Deno, một môi trường thực thi tích hợp sẵn những tiến bộ mới nhất của JavaScript, tiện lợi hơn Node nhiều

Nhược điểm:
- Số theme còn ít
- Không có đồ thị liên kết các nút cho người dùng

### Quartz
Đây là một chương trình tạo web tĩnh được viết đặc biệt cho người dùng Obsidian. Tác giả của nó muốn thúc đẩy *sự giải trung tâm hoá ở web*, hay còn gọi là *dweb* hoặc *web 3.0*. Mình đoán là cái gọi là khu vườn số cũng nằm trong dòng chảy này. Phù hợp cho người cần có đồ thị mạng lưới mối quan hệ giữa các ghi chú trên web.

Nhược điểm: 
- Không có nút ba que để mở menu cho người dùng điện thoại (có thể dùng các bản fork của cộng đồng). Tác giả hình như cũng đuối nên không tương tác nhiều với cộng đồng
- Tập tin cấu hình là `quartz.config.ts` hoặc `quartz.layout.ts`, nghĩa là để cấu hình là bạn phải dùng TypeScript để chỉnh
- Dùng Node

Nếu bạn muốn tìm hiểu thêm về môi trường thực thi Node và Deno thì có thể đọc bài này: [Code giống như các nốt nhạc, engine giống như nhạc công, còn runtime giống như nhạc cụ ](https://doi-thoai.deno.dev/We.48.1)