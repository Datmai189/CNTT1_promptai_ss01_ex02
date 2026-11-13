Phần 1 – Vì sao tiếng Việt tốn nhiều token hơn?
Vốn dĩ bộ đếm ko bị lỗi do BPE chia văn bản thành những mảnh ký tự thường gặp, chứ không đếm theo quy tắc 1 từ = 1 token, từ tiếng Việt có dấu có thể bị chia thành nhiều mảnh hơn.vì vậy nên cùng 100 từ, mẫu B dùng 285 token còn mẫu A dùng 118 token: 285 ÷ 118 xấp xỉ 2,4 lần
Phần 2 – Hai cách tiết kiệm token
-Viết hướng dẫn gọn : Ví dụ đổi “Hãy vui lòng đọc kỹ đoạn văn sau và thực hiện việc tóm tắt…” thành “Tóm tắt đoạn sau thành 3 ý”
-Đầu ra ngắn : Ví dụ thêm “Chỉ trả lời 3 gạch đầu dòng, mỗi dòng tối đa 15 từ” nếu bài toán không cần giải thích dài
Hai cách này giữ nguyên nội dung cần xử lý, nhưng không có mức tiết kiệm 30–40% cố định. Hoàng cần đo lại bằng só token đã sử dụng trước và sau khi sửa prompt để biết con số chuẩn
