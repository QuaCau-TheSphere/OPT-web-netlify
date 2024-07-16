---
share: true
created: 2023-09-05T16:17
updated: 2024-04-02T12:58
---
# Mô tả chung
Nhu cầu: người khuyết tật khi có nhu cầu di chuyển chi phí tốn kém
Giải pháp: viết app kết nối họ evà người sẵn sàng hỗ trợ, tương tự như Grab

## Câu hỏi
### Câu hỏi về chiến lược
- Tại sao đối tượng thụ hưởng lại là nkt mà không phải cái khác? 
	- Vì nhà đầu tư tiếp xúc với họ nhiều hơn 
- Tại sao lại là về hỗ trợ di chuyển cho họ mà không phải là cái khác?
	- ❓Vì đây là nhu cầu họ cần nhất
- Tại sao không dành nguồn lực để vận động chính sách cho việc cải thiện dịch vụ công cho họ?
	- Không đủ nguồn lực vận động chính sách
- Khả năng điều phối hiện nay là thế nào? Vì sao phải cần tới app mà không thuê một người để điều phối thủ công?
- Có những loại xe máy 3 bánh được thiết kế cho người khuyết tật, sao họ không mua về dùng?
- Viết xong rồi thì sẽ duy trì việc vận hành nó thế nào?

### Câu hỏi về sản phẩm
- Khác gì với WeShare? Khác gì Dichung?
- Có cần làm app cho đt ko hay làm web app là được?
- Có cần phải có bản đồ không hay có thể mặc định là người dùng chỉ cần đọc địa chỉ là đã biết là mình có thể đến được rồi?
	- ❓Người ở trọ mới lên HN 

### Câu hỏi về hành vi người dùng
- Tài xế có lý do gì để mở app để đón khách?
- Nếu trên bản đồ có nhiều người cùng thể hiện sẵn sàng giúp đỡ thì họ có [Hiện tượng khuếch tán trách nhiệm, người ngoài đứng nhìn](Hi%E1%BB%87n%20t%C6%B0%E1%BB%A3ng%20khu%E1%BA%BFch%20t%C3%A1n%20tr%C3%A1ch%20nhi%E1%BB%87m,%20ng%C6%B0%E1%BB%9Di%20ngo%C3%A0i%20%C4%91%E1%BB%A9ng%20nh%C3%ACn.md) không?

# Yêu cầu
## Yêu cầu chức năng
- Có bản đồ thể hiện vị trí các bên
- Cập nhật thời gian thực
- Có tài khoản cho người khuyết tật và tài khoản cho tài xế:
    - Tài khoản cho người khuyết tật:
        - Thông tin cá nhân
        - Loại phương tiện phù hợp cho loại khuyết tật của mình
        - Đặt chuyến:
            - Xác định điểm đi, điểm đến
            - Thời gian chờ trước khi huỷ
    - Tài khoản cho tài xế:
        - Thông tin cá nhân
        - Loại phương tiện mình có
        - Nhận chuyến:
            - Điểm đi, điểm đến của khách
            - Xác nhận chuyến
- Thông báo:
    - Với tài khoản người dùng:
        - Có tài xế nhận chở 
        - Tài xế huỷ chuyến
    - Với tài khoản tài xế:
        - Có người cần chở
        - Người dùng huỷ chuyến

## Yêu cầu phi chức năng
Thời gian khởi động dưới 5s

# Nhân sự 
- Lộc: viết chính
- Nhật: hướng dẫn lập trình và kiểm tra code của Lộc, nhận yêu cầu và tư vấn giải pháp cho anh Lâm

# Thời gian hoàn thành và giá
 Thời gian hoàn thành dự kiến (giả sử ngày làm 10 tiếng): 
 - Cho toàn bộ dự án (top-down): 5 tuần
 - Cho từng chức năng (bottom-up): 1 tuần nếu chưa có sẵn kiến thức về chức năng đó, 2 ngày nếu đã có sẵn kiến thức
 
 Giá: 80k/h
 [90% lượng code ban đầu tốn 90% thời gian lập trình. 10% lượng code còn lại tốn thêm 90% thời gian lập trình](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/C%C3%B4ng%20ngh%E1%BB%87%20th%C3%B4ng%20tin/K%E1%BB%B9%20thu%E1%BA%ADt%20ph%E1%BA%A7n%20m%E1%BB%81m/Th%E1%BB%9Di%20gian%20ho%C3%A0n%20th%C3%A0nh/90%25%20l%C6%B0%E1%BB%A3ng%20code%20ban%20%C4%91%E1%BA%A7u%20t%E1%BB%91n%2090%25%20th%E1%BB%9Di%20gian%20l%E1%BA%ADp%20tr%C3%ACnh.%2010%25%20l%C6%B0%E1%BB%A3ng%20code%20c%C3%B2n%20l%E1%BA%A1i%20t%E1%BB%91n%20th%C3%AAm%2090%25%20th%E1%BB%9Di%20gian%20l%E1%BA%ADp%20tr%C3%ACnh.md)
 [Điều nhà đầu tư quan tâm và điều muốn nhà đầu tư quan tâm](../Tr%E1%BA%A5n%20K%E1%BB%B3/4%20Th%C3%A0nh%20ph%E1%BA%A9m/Qu%E1%BB%B9/%C4%90i%E1%BB%81u%20nh%C3%A0%20%C4%91%E1%BA%A7u%20t%C6%B0%20quan%20t%C3%A2m%20v%C3%A0%20%C4%91i%E1%BB%81u%20mu%E1%BB%91n%20nh%C3%A0%20%C4%91%E1%BA%A7u%20t%C6%B0%20quan%20t%C3%A2m.md)
 [Nếu bạn nghĩ rằng bạn có thể hoàn thành đúng kế hoạch, có thể bạn đang ngộ nhận](../../%E2%9A%A1Hi%E1%BB%83u%20bi%E1%BA%BFt%20s%C3%A2u/Qu%E1%BA%A3n%20l%C3%BD%20d%E1%BB%B1%20%C3%A1n,%20ph%C3%A1t%20tri%E1%BB%83n%20s%E1%BA%A3n%20ph%E1%BA%A9m,%20x%C3%A2y%20d%E1%BB%B1ng%20t%E1%BB%95%20ch%E1%BB%A9c/C%C3%B4ng%20vi%E1%BB%87c/Th%E1%BB%9Di%20gian%20l%C3%A0m%20vi%E1%BB%87c/N%E1%BA%BFu%20b%E1%BA%A1n%20ngh%C4%A9%20r%E1%BA%B1ng%20b%E1%BA%A1n%20c%C3%B3%20th%E1%BB%83%20ho%C3%A0n%20th%C3%A0nh%20%C4%91%C3%BAng%20k%E1%BA%BF%20ho%E1%BA%A1ch,%20c%C3%B3%20th%E1%BB%83%20b%E1%BA%A1n%20%C4%91ang%20ng%E1%BB%99%20nh%E1%BA%ADn.md)
 
# Nền tảng cần dùng
## Cơ sở dữ liệu
- Một graph database như Neo4j
- Một hệ thống bản đồ:

| Giải pháp gợi ý | Điểm mạnh                                                      | Giá                                        |
| --------------- | -------------------------------------------------------------- | ------------------------------------------ |
| Google Map      | Nhiều chức năng, dữ liệu phong phú và chính xác, cộng đồng lớn | Nếu dùng dưới $200/tháng thì được miễn phí |
| Open Street Map |                                                                | Miễn phí                                   |

## Ngôn ngữ, framework
Ngôn ngữ TypeScript với runtime Deno là thích hợp nhất cho những app còn nhỏ. Nếu viết app mobile thì có thể dùng framework Capacitor để có thể viết một lần mà có cả app Android và iOS, nhưng như vậy thì có thể sẽ phải đổi runtime sang Node. 

## Máy chủ
Firebase/Deno Deploy

## Thiết bị
Nếu làm app cho iOS thì cần mở tài khoản Apple Development giá $99/năm

# Thời hạn bảo hành phần mềm
Tuỳ vào loại vấn đề mà sẽ xem xét nó có phải là lỗi hay không. Nếu nó không phải là yêu cầu đã được thống nhất trước mà là tính năng mới thì tính phí theo giờ như bình thường.
- Nếu lúc còn ít người dùng thì app không có vấn đề gì mà đến lúc người dùng tăng cao thì có vấn đề thì sẽ xét là một tính năng