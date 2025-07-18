# Bộ dữ liệu gốc bao gồm 119390 dòng và 32 cột (biến) bao gồm:

- hotel: Cho biết đặt phòng thuộc loại khách sạn nào (City Hotel hay Resort Hotel).
- is_canceled: Biến nhị phân quan trọng, cho biết đặt phòng có bị hủy hay không (1 = Đã hủy, 0 = Chưa hủy).
- lead_time: Số ngày giữa ngày đặt phòng và ngày khách đến nhận phòng.
- arrival_date_year, arrival_date_month, arrival_date_week_number, arrival_date_day_of_month: Các thông tin chi tiết về ngày khách đến.
- stays_in_weekend_nights, stays_in_week_nights: Số đêm khách ở lại vào cuối tuần (Thứ Bảy hoặc Chủ Nhật) và trong tuần (Thứ Hai tới Thứ Sáu).
- adults, children, babies: Số lượng người lớn, trẻ em và em bé trong mỗi đặt phòng.
- meal: Loại bữa ăn được đặt. Các danh mục được trình bày theo gói dịch vụ ăn uống tiêu chuẩn trong ngành khách sạn: Undefined/SC - Self Castering (tự phục vụ - không bao gồm gói bữa ăn), BB - Bed & Breakfast (nghỉ qua đêm kèm bữa sáng), HB - Half Board (bữa sáng và một bữa khác, thường là bữa tối), FB – Full board (bữa sáng, bữa trưa và bữa tối).
- country: Quốc gia của khách hàng (dưới dạng mã).
- market_segment: Kênh thị trường mà qua đó việc đặt phòng được thực hiện. Ví dụ: Online TA (Travel Agents) - Đại lý du lịch trực tuyến, Direct - Trực tiếp, TO (Tour Operators) - Nhà điều hành tour du lịch,...
- distribution_channel: Kênh phân phối của đặt phòng. Ví dụ: TA/TO - Đại lý/Nhà điều hành du lịch, Direct - trực tiếp,...
- is_repeated_guest: Cho biết khách hàng có phải là khách đã từng ở trước đây hay không (1 = Có, 0 = Không).
- previous_cancellations: Số lần hủy đặt phòng trước đó của khách hàng này.
- previous_bookings_not_canceled: Số lần đặt phòng không bị hủy trước đó của khách hàng này.
- reserved_room_type: Mã loại phòng khách đã đặt.
- assigned_room_type: Mã loại phòng thực tế khách được nhận.
- booking_changes: Số lần thay đổi được thực hiện đối với đặt phòng.
- deposit_type: Loại tiền đặt cọc (ví dụ: No Deposit, Non Refund, Refundable).
- agent: ID của đại lý du lịch thực hiện đặt phòng.
- company: ID của công ty/tổ chức thực hiện đặt phòng hoặc thanh toán.
- days_in_waiting_list: Số ngày đặt phòng nằm trong danh sách chờ trước khi được xác nhận.
- customer_type: Loại khách hàng (loại đặt phòng) bao gồm 4 nhóm: Contract - Đặt phòng theo hợp đồng, Group - Đặt phòng cho đoàn khách, Transient - hách lẻ không thuộc nhóm/hợp đồng nào, Transient-party - Khách lẻ nhưng đặt cùng lúc nhiều phòng.
- adr (Average Daily Rate): Giá trung bình mỗi ngày, được tính bằng cách chia tổng doanh thu phòng cho số đêm lưu trú.
- required_car_parking_spaces: Số lượng chỗ đậu xe khách yêu cầu.
- total_of_special_requests: Tổng số các yêu cầu đặc biệt từ khách hàng (ví dụ: giường đôi hoặc tầng cao).
- reservation_status: Trạng thái cuối cùng của đặt phòng (Canceled - Khách hàng đã hủy đặt phòng, Check-Out - Khách đã nhận phòng và hoàn tất thời gian lưu trú. , No-Show - Khách không đến nhận phòng).
- reservation_status_date: Ngày cập nhật trạng thái cuối cùng. Biến này giúp xác định thời điểm chính xác khi đặt phòng bị hủy hoặc ngày khách trả phòng sau khi hoàn tất lưu trú.

# Bộ dữ liệu sạch sau khi tiền xử lý bao gồm 86244 dòng và 35 cột, bao gồm thêm:

- total_nights: tổng số đêm lưu trú của khách
- arrival_date_month_num: tháng dạng số
- arrival_date: năm-tháng-ngày khách đến.
