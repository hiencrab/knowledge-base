# Xử lý sự cố mạng

## Quy trình
1. Xác định phạm vi: một máy, một phòng hay toàn bộ?
2. Kiểm tra vật lý: cáp, đèn cổng, Wi-Fi.
3. Kiểm tra IP: có nhận IP đúng dải không?
4. Ping gateway, rồi ping IP ngoài, rồi ping tên miền.
5. Nếu ping IP được mà tên miền không: lỗi DNS.

## Lệnh thường dùng

=== "Windows"
    ```
    ipconfig /all
    ipconfig /release && ipconfig /renew
    ipconfig /flushdns
    ping 8.8.8.8
    tracert example.com
    nslookup example.com
    netstat -ano
    ```

=== "Linux"
    ```
    ip a
    ip route
    ping -c 4 8.8.8.8
    traceroute example.com
    dig example.com
    ss -tulpn
    ```

## Dấu hiệu nhanh

| Triệu chứng | Nghi ngờ |
|---|---|
| IP dạng 169.254.x.x | Không nhận được DHCP |
| Ping IP được, tên miền không | DNS |
| Vào được web nội bộ, không ra Internet | Gateway hoặc firewall |
| Chập chờn | Cáp lỗi, nhiễu Wi-Fi, trùng IP |
