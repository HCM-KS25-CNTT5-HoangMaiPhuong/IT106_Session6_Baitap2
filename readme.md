# Bài tập 2: Xây dựng Prioritized Product Backlog bằng kỹ thuật MoSCoW

## 1. Mục tiêu và cơ sở ưu tiên

Trong vai trò Product Owner, tôi ưu tiên Release 1 theo mục tiêu: độc giả có thể tìm sách, đặt mượn online và đến quầy nhận sách giấy; thủ thư có thể quản lý danh mục và kho sách phục vụ việc mượn. Thời gian thực hiện dự kiến là 3 sprint, mỗi sprint 2 tuần, với năng lực khoảng **20 điểm**.

Các hạng mục được phân loại theo giá trị cốt lõi đối với MVP, khả năng xử lý tạm thời, mức độ phụ thuộc, rủi ro và công sức triển khai. Trong cùng một nhóm, tôi ưu tiên các chức năng nền tảng trước, sau đó đến chức năng tạo giá trị cao với công sức thấp; những chức năng phức tạp hoặc có thể thay thế bằng xử lý tại quầy đứng sau.

Quy đổi công sức: **S = 1 điểm, M = 2 điểm, L = 3 điểm**. Product Owner chịu trách nhiệm sắp xếp Product Backlog; thứ tự dưới đây là thứ tự ưu tiên, không phải cam kết phân chia từng sprint.

## 2. Bảng phân loại 12 hạng mục

| Mã gốc | Hạng mục | Kích thước | Điểm | Nhóm MoSCoW | Lý do phân loại |
| --- | --- | :---: | ---: | --- | --- |
| 1 | Đăng nhập/đăng ký tài khoản độc giả | M | 2 | Must have | Đây là nền tảng xác định độc giả để ghi nhận lượt mượn và kiểm soát giới hạn số sách mượn cùng lúc. |
| 2 | Tìm kiếm sách theo tên/tác giả | M | 2 | Must have | Độc giả cần tìm được sách muốn mượn để hoàn thành luồng sử dụng cốt lõi của MVP. |
| 3 | Mượn sách online (có giới hạn số sách mượn cùng lúc) | L | 3 | Must have | Đây là chức năng tạo giá trị chính của hệ thống, đồng thời phụ thuộc vào tài khoản độc giả và dữ liệu kho sách. |
| 4 | Gia hạn mượn sách online | S | 1 | Should have | Gia hạn online thuận tiện và ít công sức nhưng độc giả vẫn có thể nhờ thủ thư xử lý tại quầy trong Release 1. |
| 5 | Đặt trước sách khi hết (kèm thông báo khi sách có sẵn) | M | 2 | Should have | Chức năng giúp độc giả tiếp cận sách đang hết nhưng có thể tạm nhờ thủ thư ghi nhận yêu cầu và chỉ triển khai sau chức năng mượn online. |
| 6 | Đánh giá & bình luận sách sau khi đọc | M | 2 | Could have | Nhận xét hỗ trợ lựa chọn sách nhưng không quyết định khả năng mượn sách của MVP và cần có dữ liệu mượn để xác định độc giả đã đọc. |
| 7 | Gợi ý sách theo sở thích cá nhân (recommendation) | L | 3 | Won't have (this time) | Gợi ý cá nhân cần dữ liệu sở thích hoặc lịch sử đủ hữu ích, có rủi ro chất lượng và công sức lớn nên hoãn sang bản phát hành sau. |
| 8 | Thông báo email khi sắp đến hạn trả sách | S | 1 | Should have | Nhắc hạn trả giúp giảm quên trả với công sức nhỏ nhưng có thể tạm dựa vào hạn trả được cung cấp khi nhận sách. |
| 9 | Xem lịch sử mượn sách của bản thân | S | 1 | Should have | Lịch sử giúp độc giả kiểm tra các lượt mượn với công sức thấp nhưng có thể tạm tra cứu qua thủ thư nếu chưa triển khai. |
| 10 | Thủ thư quản lý kho sách (thêm/sửa/xóa sách) | L | 3 | Must have | Quản lý kho cung cấp dữ liệu sách cho tìm kiếm và mượn online, giúp thư viện duy trì thông tin phục vụ vận hành MVP. |
| 11 | Chat trực tiếp với thủ thư | L | 3 | Won't have (this time) | Độc giả có thể trao đổi tại quầy, trong khi chat trực tiếp tốn nhiều công sức và cần bố trí người hỗ trợ nên chưa làm ở Release 1. |
| 12 | Tích hợp đăng nhập bằng Google/Facebook | M | 2 | Could have | Đăng nhập mạng xã hội giảm thao tác nhưng tài khoản thông thường đã đáp ứng MVP, nên chỉ triển khai khi còn năng lực sau các chức năng quan trọng hơn. |

## 3. Tính công sức và giới hạn Release 1

Nhóm Must gồm **4 hạng mục: 1, 2, 3 và 10**, đáp ứng quy tắc không vượt quá 5 hạng mục.

- Tổng điểm Must: **2 + 2 + 3 + 3 = 10 điểm**.
- Ngưỡng tham chiếu 60% năng lực: **20 × 60% = 12 điểm**.
- Tỷ lệ thực tế của Must: **10 / 20 × 100% = 50%**.

Như vậy, nhóm Must **nằm dưới ngưỡng tham chiếu khoảng 12/20 điểm**. Tỷ lệ 50% thấp hơn mốc 60%; tôi giữ mức này vì bốn chức năng đã tạo thành luồng cốt lõi và không cần nâng một chức năng có cách xử lý tạm lên Must chỉ để đủ 12 điểm.

| Nhóm | Số hạng mục | Tổng điểm | Cách xử lý trong Release 1 |
| --- | ---: | ---: | --- |
| Must have | 4 | 10 | Bảo vệ phạm vi cốt lõi để MVP sử dụng được. |
| Should have | 4 | 5 | Ưu tiên tiếp theo; có thể cắt nếu tiến độ không đáp ứng. |
| Could have | 2 | 4 | Chỉ thực hiện khi còn năng lực sau Must và Should. |
| Won't have (this time) | 2 | 6 | Không thực hiện ở Release 1; giữ trong backlog cho các bản sau. |
| **Tổng** | **12** | **25** | |

Tổng công sức các mục có thể thực hiện ở Release 1 là **10 + 5 + 4 = 19 điểm**, còn **1 điểm dự phòng** so với năng lực khoảng 20 điểm. Hai mục Won't có tổng 6 điểm được hoãn; không cần sử dụng hết 20 điểm vì ước lượng và năng lực đều có độ bất định. Should và Could vẫn là vùng đệm có thể cắt, không phải cam kết phải hoàn thành toàn bộ.

## 4. Product Backlog có thứ tự từ 1 đến 12

| Thứ tự | Mã gốc | Hạng mục | MoSCoW | Điểm | Cơ sở sắp thứ tự |
| ---: | ---: | --- | --- | ---: | --- |
| 1 | 1 | Đăng nhập/đăng ký tài khoản độc giả | Must | 2 | Xây dựng nền tảng định danh trước các chức năng gắn với từng độc giả. |
| 2 | 10 | Thủ thư quản lý kho sách (thêm/sửa/xóa sách) | Must | 3 | Chuẩn bị dữ liệu kho sách trước tìm kiếm và mượn, đồng thời xử lý sớm rủi ro của chức năng lớn. |
| 3 | 2 | Tìm kiếm sách theo tên/tác giả | Must | 2 | Dựa trên dữ liệu kho để giúp độc giả chọn sách trước khi đặt mượn. |
| 4 | 3 | Mượn sách online (có giới hạn số sách mượn cùng lúc) | Must | 3 | Hoàn thiện luồng cốt lõi sau khi có tài khoản, kho sách và tìm kiếm. |
| 5 | 9 | Xem lịch sử mượn sách của bản thân | Should | 1 | Tạo giá trị tra cứu nhanh với chi phí thấp ngay khi hệ thống đã ghi nhận lượt mượn. |
| 6 | 4 | Gia hạn mượn sách online | Should | 1 | Tiếp tục xử lý vòng đời lượt mượn với chi phí nhỏ, sau khi có dữ liệu mượn và hạn trả. |
| 7 | 8 | Thông báo email khi sắp đến hạn trả sách | Should | 1 | Giảm quên trả sách; làm sau gia hạn để thông báo dựa trên hạn trả đã được cập nhật. |
| 8 | 5 | Đặt trước sách khi hết (kèm thông báo khi sách có sẵn) | Should | 2 | Làm sau mượn online và ưu tiên sau các mục Should ít công sức hơn vì cần xử lý hàng chờ và thời điểm sách có sẵn. |
| 9 | 6 | Đánh giá & bình luận sách sau khi đọc | Could | 2 | Bổ sung thông tin lựa chọn sách sau khi đã có dữ liệu lượt mượn hoàn tất. |
| 10 | 12 | Tích hợp đăng nhập bằng Google/Facebook | Could | 2 | Tăng tiện lợi sau đăng nhập thông thường; xếp sau đánh giá vì còn phụ thuộc tích hợp với bên thứ ba. |
| 11 | 7 | Gợi ý sách theo sở thích cá nhân (recommendation) | Won't (this time) | 3 | Giữ cho bản sau khi có dữ liệu lịch sử và phản hồi để hỗ trợ cá nhân hóa. |
| 12 | 11 | Chat trực tiếp với thủ thư | Won't (this time) | 3 | Xếp cuối vì có cách hỗ trợ tại quầy và cần thêm năng lực vận hành dịch vụ chat. |

### Kiểm tra phụ thuộc

Các phụ thuộc dưới đây là giả định triển khai dùng để sắp thứ tự, không bổ sung hạng mục mới:

- **Quản lý kho (10) → Tìm kiếm (2):** có dữ liệu sách trước khi tìm kiếm; cả hai thuộc Must.
- **Đăng nhập (1), quản lý kho (10), tìm kiếm (2) → Mượn online (3):** các nền tảng của luồng đặt mượn đều thuộc Must và đứng trước mục 3.
- **Mượn online (3) → Lịch sử (9), gia hạn (4), nhắc hạn (8), đặt trước (5):** dữ liệu và quy tắc mượn được xây dựng trước các chức năng Should này.
- **Gia hạn (4) → Nhắc hạn (8):** theo thứ tự triển khai đã chọn, hoàn thiện cập nhật hạn trả trước khi xử lý email nhắc hạn.
- **Mượn online (3) → Đánh giá (6):** dữ liệu mượn hỗ trợ xác định độc giả được nhận xét sau khi đọc; Must đứng trước Could.
- **Đăng nhập thông thường (1) → Đăng nhập Google/Facebook (12):** có tài khoản nội bộ trước khi liên kết đăng nhập bên thứ ba; Must đứng trước Could.
- **Lịch sử (9), đánh giá (6) → Gợi ý cá nhân (7):** nếu tận dụng các dữ liệu này để gợi ý, chúng đều thuộc nhóm cao hơn và đứng trước mục 7.

Mỗi hạng mục xuất hiện đúng một lần, có thứ tự duy nhất, và các nhóm được sắp theo **Must → Should → Could → Won't**. Các mục Won't vẫn giữ trong Product Backlog nhưng không được đưa vào phạm vi Release 1.

## 5. Tự phản biện

Một Product Owner khác có thể xếp gợi ý sách (mục 7) vào Should nếu thư viện có sẵn dữ liệu sở thích và coi việc giúp độc giả khám phá sách là mục tiêu quan trọng của Release 1; tôi vẫn chọn Won't vì đề bài chưa xác nhận các điều kiện đó và công sức là 3 điểm. Với chat trực tiếp (mục 11), người khác có thể chọn Should nếu độc giả thường cần hỗ trợ trước khi đến quầy và thư viện có nhân sự trực chat; lựa chọn Won't của tôi dựa trên khả năng hỗ trợ tại quầy và giới hạn năng lực phát triển. Đăng nhập Google/Facebook (mục 12) có thể được nâng lên Should nếu dữ liệu cho thấy độc giả thường bỏ đăng ký vì quá nhiều thao tác; tôi chọn Could vì đăng nhập thông thường đã đáp ứng luồng mượn cốt lõi. Khi có bằng chứng mới về nhu cầu hoặc rủi ro, tôi sẽ điều chỉnh phân loại và thứ tự, đồng thời kiểm tra lại tổng điểm và phụ thuộc để giữ phạm vi Release 1 khả thi.
