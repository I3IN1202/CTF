# EHC-Challenges
## Forensics
### - Dimension
### - Easy
### - 50 points
## Author:
  - Đỗ Minh Huy
## Problem
file: https://drive.google.com/file/d/1jtsa69LFk4-lqjEqQO9UK75QOwOgsRqU/view?usp=drive_link
  - Tổng quan về bài là: Là có một file ảnh ẩn chứa những bí ẩn gì, chúng ta hãy cùng đón xem!!
## Solution
Đầu tiên khi ta mở file đó lên thì ta nhận thấy đó là một file JPG bình thường! Không ẩn chưa gì 

![Screenshot 2023-12-08 213901](https://github.com/I3IN1202/CTF/assets/112995017/497b0026-eec6-440c-8222-58a492f8f63d)

Nhưng để ý một chút thì có vẻ như size của bức ảnh đang ẩn chứa điều gì đó. Mình đã thay đổi size width từ 0x9804 thành 0x0A20 và đã tìm ra được flag.

Flag: W1{tH3_he1gH7_I5_h1Din9_s0mETh!n6}

