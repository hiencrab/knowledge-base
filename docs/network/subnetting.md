# Chia subnet

## Công thức
- Số địa chỉ trong subnet: `2^(32 - prefix)`
- Số host dùng được: `2^(32 - prefix) - 2` (trừ địa chỉ mạng và broadcast)

## Bảng nhanh

| Prefix | Subnet mask | Host dùng được |
|---|---|---|
| /24 | 255.255.255.0 | 254 |
| /25 | 255.255.255.128 | 126 |
| /26 | 255.255.255.192 | 62 |
| /27 | 255.255.255.224 | 30 |
| /28 | 255.255.255.240 | 14 |
| /30 | 255.255.255.252 | 2 |

## Ví dụ
Mạng `192.168.10.0/26`: dải host từ `.1` đến `.62`, broadcast `.63`, subnet kế tiếp bắt đầu `.64`.
