# Mô hình OSI và TCP/IP

| Tầng OSI | Tên | Ví dụ giao thức / thiết bị |
|---|---|---|
| 7 | Application | HTTP, DNS, SMTP |
| 6 | Presentation | TLS, mã hóa, nén |
| 5 | Session | Quản lý phiên |
| 4 | Transport | TCP, UDP |
| 3 | Network | IP, ICMP, router |
| 2 | Data Link | Ethernet, MAC, switch |
| 1 | Physical | Cáp, sóng Wi-Fi |

TCP/IP gộp thành 4 tầng: Application (OSI 5-7), Transport, Internet, Network Access (OSI 1-2).

## Mẹo khi xử lý sự cố
Đi từ dưới lên: kiểm tra cáp và đèn cổng (tầng 1), rồi IP và gateway (tầng 3), rồi cổng dịch vụ (tầng 4), cuối cùng mới tới ứng dụng.
