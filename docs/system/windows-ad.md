# Windows và Active Directory

## Khái niệm chính
- **Domain**: ranh giới quản trị, do Domain Controller (DC) quản lý.
- **OU**: đơn vị tổ chức để nhóm user, máy tính và áp dụng GPO.
- **GPO**: chính sách áp dụng tự động cho user hoặc máy.

## Tác vụ thường làm
- Reset mật khẩu, mở khóa tài khoản trong *Active Directory Users and Computers*.
- Áp dụng GPO ngay: `gpupdate /force`
- Xem GPO đã áp dụng: `gpresult /r`
- Kiểm tra tài khoản máy với domain: `Test-ComputerSecureChannel` (PowerShell)

## Lỗi hay gặp
| Lỗi | Hướng xử lý |
|---|---|
| Không join được domain | Kiểm tra DNS trỏ về DC, đồng bộ giờ |
| Đăng nhập báo sai mật khẩu dù đúng | Tài khoản bị khóa hoặc giờ lệch |
| GPO không áp dụng | `gpresult`, kiểm tra OU và lọc bảo mật |
