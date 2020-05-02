---
title: "Bài tập luyện tập CF-A-1"
categories: [Học thuật toán, học lập trình, C++]
tags: [học thuật toán và lập trình]
---
# CF-A.1. Vanya and Fence

([http://codeforces.com/contest/677/problem/A](http://codeforces.com/contest/677/problem/A))

Vanya và những người bạn của cậu đang đi bộ dọc theo hàng rào có độ cao h, họ không muốn để ông bảo vệ nhìn thấy và nhắc nhở. Do đó, độ cao đoàn người không được quá độ cao của hàng rào h. Nếu độ cao của một người nào mà lớn hơn h, người đó phải cúi thấp xuống dưới hàng rào để đảm bảo người bảo vệ khu vườn không nhìn thấy. Cho biết độ cao của người thứ i trong hàng là ai.

Giả sử mỗi người đi bình thường chiếm 1 đơn vị chiều rộng, trong khi của người phải cúi xuống là 2. Những người bạn muốn nói chuyện với nhau trong khi đi dọc hàng rào, nên họ không muốn đi theo hàng dọc. Hỏi độ rộng tối thiểu của con đường là bao nhiêu để những người bạn có thể đi bộ theo hàng mà không bị người bảo vệ phát hiện.

Input:

- Dòng đầu ghi hai số nguyên n và h (1 ≤ _n_ ≤ 1000, 1 ≤ _h_ ≤ 1000)
- Dòng thứ hai ghi n số nguyên

Output:

- In ra một số nguyên là kết quả của bài toán.

Ví dụ:

| Input | Output |
| --- | --- |
| 3 74 5 14 | 4 |
| 6 11 1 1 1 1 1 | 6 |
| 6 57 6 8 9 10 5 | 11 |

Giải thích test 1: chỉ người thứ 3 cần phải cúi xuống  độ rộng của đường sẽ là 1+1+2=4

Test2: Tất cả đội đều có độ cao nhỏ hơn hàng rào nên độ rộng của đường là 6