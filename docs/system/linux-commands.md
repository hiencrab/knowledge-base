# Lệnh Linux thường dùng

| Mục đích | Lệnh |
|---|---|
| Xem dung lượng đĩa | `df -h` |
| Xem dung lượng thư mục | `du -sh *` |
| Xem tiến trình | `top`, `ps aux` |
| Xem RAM | `free -h` |
| Xem log dịch vụ | `journalctl -u <service> -f` |
| Quản lý dịch vụ | `systemctl status\|start\|stop\|restart <service>` |
| Tìm file | `find / -name "<tên>"` |
| Tìm trong nội dung | `grep -rn "<chuỗi>" <thư mục>` |
| Phân quyền | `chmod`, `chown` |
| Xem cổng đang mở | `ss -tulpn` |

!!! tip
    Trước khi sửa file cấu hình, luôn sao lưu: `cp file file.bak`.
