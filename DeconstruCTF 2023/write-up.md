# DeconstruCT.F
## Forensics
### - Two paths
### - Easy
### - 100 points
## Author:
  - Đỗ Minh Huy
## Problem
file: 
  - Tổng quan về bài là: Logan gave me this image file before disappearing.. I've been breaking my head over it for long. Can you decode it? Đơn giản là có một file ảnh có dạng JDP, chúng ta thử xem sao!!!
## Solution
Đầu tiên chúng ta hãy thử check file ảnh đó xem có gì không. Và mình nhận thấy đây không phải là một ảnh bình thường, vậy nên chũng ta hãy dùng một số tools như zsteg, 7z, unzip,binwalk... để mở thử xem ẩn sau bức ảnh đó là gì.

  <img width="370" alt="Screenshot 2023-08-09 133848" src="https://github.com/I3IN1202/CTF/assets/112995017/09586602-e29c-4461-a19a-7a4aba1de732">

Và đúng như mình đã dự đoán, sau khi unzip có 2 bức ảnh nữa đó là repill.jpg và greenpill.jpg. 
Mình tiếp tục mở bức ảnh greenpill.jpg ra trước thì thấy có một file flag.jpg. Tưởng chừng như thử thách đã kết thúc ở đây nhưng không đó chỉ là fake flag và dường như đó là một con đường cụt.

  <img width="366" alt="Screenshot 2023-08-09 134009" src="https://github.com/I3IN1202/CTF/assets/112995017/c98ae7e2-aaef-4465-97f8-5bc8d0408eef">

Thử tiếp đến bức ảnh redpill.jpg thì xuất hiện 2 file: file âm thanh morse.wav và file secret.zip có pass khóa. Dần dần có vẻ hướng đi của mình đã đúng.

  <img width="366" alt="Screenshot 2023-08-09 134023" src="https://github.com/I3IN1202/CTF/assets/112995017/afea0b1d-ca9f-469f-9e16-a0414c7b743c">

Mình thử sử dụng tools https://morsecode.world/international/decoder/audio-decoder-adaptive.html để decode file morse.wav thì đã ra được một đoạn password có thể là dùng để mở file secret.

  <img width="501" alt="Screenshot 2023-08-09 134159" src="https://github.com/I3IN1202/CTF/assets/112995017/72d88dd7-54ba-4c23-9483-1a772143928a">
  
        THE HOVERCRAFT OF MORPHUES 

Nhưng thật không may mắn đó không phải là password chính xác, mình thử lên search GG thì ra đây có là tên của một con tàu của Morphues trong phim The Matrix có tên là

        Nebuchadnezzar

Và đó cũng chính là password để mở file secret.zip. Và khi mở ra thì lại là một file deep_secret.wav.
Mình có thử dùng một số tool để check và đọc file âm thanh đó nhưng không có kết quả gì. Sau một hồi mình nghĩ có thể đây lại là một file ẩn gì đó chăng và search tool deep sound was steg https://wiki.bi0s.in/steganography/deep-sound/

  <img width="594" alt="Screenshot 2023-08-09 130238" src="https://github.com/I3IN1202/CTF/assets/112995017/bd155178-5c1b-40e6-b85f-f242cc375c2c">

Thì thật may mắn mình đã tìm ra được flag

Flag: dsc{u_ch053_THE_cOrr3Ct_pill!}


  











