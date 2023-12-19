# BackdoorCTF 2023
## Forensics
### - Sonic-Hide_and-Seek
### - Easy
### - 300 points
## Author:
  - Đỗ Minh Huy
## Problem
file: 
  - Tổng quan về bài là: From the apollo moon landing in 1969 to people using Deepfake to fool others, the use of technology has changed. Anyways, use your skills to uncover the deep secrets of the moon landing from the given data. Adios amigo. Là có một file audio .wav, chúng ta thử xem sao!!!
## Solution
Sau khi phân tích đề bài ta nhận thấy bài này hoàn toàn chúng ta có thể dùng tool để tìm ra flag. Mình đã sử dụng Sonic Visualier và đã tìm được part 1 của flag.

  ![image](https://github.com/I3IN1202/CTF/assets/112995017/c0b69d38-ba54-4bb2-b68d-f9a4a0445348)
  
        Part 1: flag{aud105

Sau khi mình tìm ra part 1 thì mình đã tiếp tục sử dụng 1 phần mềm nữa để phân tích file .wav là DeepSound thì đã ra được part 3

  ![image](https://github.com/I3IN1202/CTF/assets/112995017/96f84d6e-47ca-4b1e-9157-163e9bc2fced)

Và đó cũng là part cuối của flag vậy còn thiếu part 2 và mình vẫn chưa thể tìm ra!

        Part3: 4r5n't_th3y?}

Sau một thời gian tìm hiểu và mình đã nhớ đến 1 tool trong bài Moonwalk trong picoCTF là SSTV (Slow-Scan-TV). Và đã tìm ra được flag 

  ![image](https://github.com/I3IN1202/CTF/assets/112995017/82a104b4-a5b2-423b-b115-d5db04d5df97)

        Part 2: 4r3_c00l

Flag: flag{aud105_4r3_c00l_4r5n't_th3y?}


  












