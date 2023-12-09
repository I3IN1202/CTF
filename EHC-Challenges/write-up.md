# EHC-Challenges
## Forensics
### - whereIsMySwan
### - Easy
### - 30 points
## Author:
  - Đỗ Minh Huy
## Problem
file: https://drive.google.com/file/d/1-tkpAl-FPEtTWo5SGnR800UsJV5Y8yZN/view?usp=drive_link
  - Tổng quan về bài là: Là có một file PCAP nhưng thực hư ra sao, chúng ta hãy cùng đón xem!!
## Solution
Đầu tiên khi ta mở file đó lên thì ta nhận thấy đó không phải là một file PCAP bình thường!

![Screenshot 2023-12-08 210858](https://github.com/I3IN1202/CTF/assets/112995017/6f41c38e-c1e8-44fc-882f-36d6c8bd38a8)

Để ý một chút thì có đuôi là FF D9, đó là dấu hiệu nhận biết đó là một file JPEG chứ không phải file PCAP.

Sau khi chỉnh sửa một số byte thì ta nhận được một bức ảnh: 

![Screenshot 2023-12-08 211105](https://github.com/I3IN1202/CTF/assets/112995017/16ba9e31-4e40-467a-9c0e-25502e8bc2a9)

Có vẻ như bức ảnh này không đúng với size của nó. Mình đã thay đổi size từ 0x0140 thành 0x0190 và đã tìm ra được flag.

Flag: EHC{1_l0v3_5w4n_4nd_tul1p}

