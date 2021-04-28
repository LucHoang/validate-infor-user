# validate-infor-user
Trong phần này chúng ta sẽ phát triển chức năng cho phép validate thông tin của người dùng.

Chức năng này cho phép nhập vào thông tin người dùng và hiển thị các thông báo tương ứng với giá trị của các trường dữ liệu.

Yêu cầu đối với dữ liệu người dùng bao gồm:

Tên bắt buộc, có độ dài tối thiểu là 2 ký tự, tối đa là 30 ký tự

Tuổi bắt buộc, có giá trị nhỏ nhất là 18

@NotEmpty: không để trống

@Size(min = 2, max = 30): độ dài từ 2 đến 30

@Min(18): Giá trị nhỏ nhất là 18

Thêm: @Validated @ModelAttribute("user") User user để xác thực Model User

Thêm: 
BindingResult bindingResult giữ kết quả xác nhận và ràng buộc User có xảy ra lỗi không.
