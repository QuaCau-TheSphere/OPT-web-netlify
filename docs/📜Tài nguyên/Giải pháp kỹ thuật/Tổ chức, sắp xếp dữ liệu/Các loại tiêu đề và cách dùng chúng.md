---
share: true
created: 2023-10-27T18:59
updated: 2024-09-22T14:33
alias: heading
---
Lý tưởng nhất thì chỉ cần dùng một thứ để đặt cho tất cả những cái này. Và đó là filename. Chính vì như vậy, nên filename nên là thứ mặc định. Nhưng có những lúc nó chứa ký tự đặc biệt hoặc đường dẫn quá dài thì Windows hoặc Git sẽ không chịu, nên nên có một trường khác có chức năng làm mặc định cho những thứ còn lại. Đó chính là `title`. 

Nếu tiêu đề Khi truy cập từ cây thư mục thì đang đinh ninh tiêu đề phải giống, nếu khác thì sẽ bị khựng. Nhưng nếu để nguyên tiêu đề của cây thư mục thì sẽ bị lệch so với nội dung, nên cần phải có thể một tiêu đề khác để chuẩn bị cho mình rằng nội dung mới có tiêu đề khác với tiêu đề từ cây thư mục (VD: [WordPress giúp việc tạo web dễ dàng nhất, chứ không phải là thứ tạo web hiệu quả nhất](../Web/WordPress%20gi%C3%BAp%20vi%E1%BB%87c%20t%E1%BA%A1o%20web%20d%E1%BB%85%20d%C3%A0ng%20nh%E1%BA%A5t,%20ch%E1%BB%A9%20kh%C3%B4ng%20ph%E1%BA%A3i%20l%C3%A0%20th%E1%BB%A9%20t%E1%BA%A1o%20web%20hi%E1%BB%87u%20qu%E1%BA%A3%20nh%E1%BA%A5t.md))

| Vai trò                                                                                                            | Vị trí xuất hiện                                                    | Cách điều chỉnh | Nếu không điều chỉnh thì mặc định sẽ lấy giá trị từ | Lý do cần điều chỉnh mà không dùng mặc định được                                   |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | --------------- | --------------------------------------------------- | ---------------------------------------------------------------------------------- |
| Quản lý tập tin từ hệ điều hành. Tạo slug                                                                          | filename: lúc xuất file, terminal, Windows Explorer                 | filename        | Luôn có                                             | Không có                                                                           |
| Cho phép filename không phải slugify quá nhiều ký tự đặc biệt                                                      | Enveloppe tạo git                                                   | `filename`      | filename                                            | Tìm filename có ký tự đặc biệt bằng đúng với ký tự được nhập ở bàn phím            |
| Nhận diện bài viết, tóm tắt nội dung, quản lý theo cấu trúc của tác giả hoặc người đang tìm kiếm theo một cấu trúc | Tiêu đề: trên cao, file explorer, breadcrumb, menu, navigation pane | `title`         | filename                                            | filename không được chứa ký tự đặc biệt hoặc quá dài, nhưng tiêu đề lại có         |
| Tạo dự đoán cho người đọc về nội dung bên trong, làm cho họ thấy vì sao họ cần đọc bài đó, đáp ứng câu hỏi của họ  | Headline (`<title>`, `<h1>`)                                        | Markdown `#`    | `title`, filename                                   | Mental model của người đã hiểu nó rồi khác với mental model của người chưa hiểu nó |
| Nối tiếp dòng suy nghĩ                                                                                             | Liên kết (`[[]]`, `<a>`)                                            | `alias`         | `title`, filename                                   |                                                                                    |
|                                                                                                                    | Search autocomplete, kết quả Google                                 | Không cần chỉnh | `alias`, `title`, filename                          |                                                                                    |
| Tiêu đề lúc chia sẻ trên Facebook                                                                                  | Tiêu đề trong Open Graph (`meta property="og:title"`)               | `ogTitle`       | `title`, filename                                   |                                                                                    |

Plugin [Front Matter Title](https://github.com/snezhig/obsidian-front-matter-title) có thể đọc những cái này để thay đổi trên Obsidian.

Xem thêm:: [Các loại alias](./C%C3%A1c%20lo%E1%BA%A1i%20alias.md)
## Path
Giữ nguyên path?
Phản đối:
- Không đáng kể
- Người muốn tìm đến thì sẽ tìm được thôi. Search cũng không khó


Có lúc chỉ muốn đặt tiêu đề là câu hỏi, dù có thể đặt theo chủ đề: [Làm sao để tìm được thứ cần tìm khi không biết từ khoá chính xác của nó?](../../L%C3%A0m%20sao%20%C4%91%E1%BB%83%20t%C3%ACm%20%C4%91%C6%B0%E1%BB%A3c%20th%E1%BB%A9%20c%E1%BA%A7n%20t%C3%ACm%20khi%20kh%C3%B4ng%20bi%E1%BA%BFt%20t%E1%BB%AB%20kho%C3%A1%20ch%C3%ADnh%20x%C3%A1c%20c%E1%BB%A7a%20n%C3%B3.md). Có lúc thì chỉ muốn đặt theo chủ đề, dù có thể đặt theo câu hỏi: [Các loại tiêu đề và cách dùng chúng](C%C3%A1c%20lo%E1%BA%A1i%20ti%C3%AAu%20%C4%91%E1%BB%81%20v%C3%A0%20c%C3%A1ch%20d%C3%B9ng%20ch%C3%BAng.md)