---
title: "Bài tập luyện tập CF-A-1"
categories: [Học thuật toán, học lập trình, C++]
tags: [học thuật toán và lập trình]
---
# CF-A.6. Gravity Flip

([http://codeforces.com/contest/405/problem/A](http://codeforces.com/contest/405/problem/A) )

Little Chris cảm thấy buồn chán trong các giờ vật lý, cậu ta tạo cho mình một hộp đồ chơi đặc biệt, hộp này có khả năng làm thay đổi lực hấp dẫn của trái đất. Hộp gồm có n cột chứa các hình lập phương được xếp theo hàng, cột thứ i gồm có ai hộp. Ban đầu trọng lực của hộp có hướng xuống dưới. Khi Chris thay đổi trọng lực, trọng lực đổi hướng bắt đầu kéo các hình lập phương sang phía phải của hộp. Dưới đây là hình thể hiện lúc ban đầu và thời điểm cuối cùng của các khối hộp: những khối hộp đã thay đổi vị trí được đánh dấu màu cam.

![](RackMultipart20200502-4-b5e5r2_html_f550b1a525f88842.png)

Cho cấu hình hộp ban đầu và kết thúc. Bạn hãy tìm số lượng các khối lập phương ở mỗi cột sau khi thay đổi hướng của trọng lực sang phải.

Input:

- Dòng đầu ghi số nguyên n (1 ≤ _n_ ≤ 100)
- Dòng tiếp theo ghi n số nguyên, các số cách nhau bởi dấu cách; số thứ i là ai(1 ≤ _a__i_ ≤ 100) thể hiện số lượng khối lập phương ở cột thứ i

Output:

- Gồm n số nguyên, thể hiện số lượng các khối lập phương ở mỗi cột

Ví dụ:

| **Input** | **Output** |
| --- | --- |
| 43 2 1 2 | 1 2 2 3 |
| 32 3 8 | 2 3 8 |

