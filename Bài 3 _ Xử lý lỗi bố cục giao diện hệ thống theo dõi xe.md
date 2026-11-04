Phần 1: Phân tích  
Dùng F12 (Inspect Element) tìm thẻ HTML bị lỗi; mở tab Computed để phân tích sơ đồ CSS Box Model hiện tại (gồm 4 lớp từ trong ra ngoài: Content, Padding, Border, Margin).  
Phần 2: Triển khai  
Chỉnh sửa trực tiếp thông số trên tab Styles (không sửa mã nguồn). Cụ thể, tăng thông số Margin (như margin-bottom cho khung trên hoặc margin-top cho khung dưới) để đẩy hai khung "Thông tin tài xế" và "Danh sách trạm" ra xa nhau, triệt tiêu việc chồng lấn.  
Phần 3: Kiểm thử  
Nếu thay đổi Margin mà phần tử không di chuyển, nguyên nhân do các thuộc tính định vị đang ghi đè luồng hiển thị (normal flow) ở tầng Browser Engine. Cần kiểm tra thẻ đó có đang bị gắn position: absolute, position: fixed, hoặc float hay không