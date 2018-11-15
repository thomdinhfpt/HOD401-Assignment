# HOD401-Assignment
Lời giải:
Khi truy cập vào trang https://www.hackthebox.eu/
Chuyển hướng tới trang yêu cầu Invite Code để Sign up.
Khi inspect ở trang này, ta thấy một script có source là /js/inviteapi.min.js.
Trong file js, ta thấy hàm makeInviteCode(). Quay ngược lại trang Sign up, ta mở console của chrome lên và chạy makeInviteCode().
Kết quả trả về là một đoạn data được mã hóa với kiểu mã hóa hiện ở dòng dưới. 
Sau khi decode data, ta được chỉ dẫn "In order to generate the invite code, make a POST request to /api/invite/generate.
Sau khi gửi request, ta nhận lại được một đoạn data được encode Base64.
Sau khi decode ta nhận được Invite Code.
Sign up thành công.
