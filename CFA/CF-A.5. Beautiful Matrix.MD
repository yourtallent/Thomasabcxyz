---
title: "Bài tập luyện tập CF-A-1"
categories: [Học thuật toán, học lập trình, C++]
tags: [học thuật toán và lập trình]
---
# CF-A.5. Beautiful Matrix

([http://codeforces.com/contest/263/problem/A](http://codeforces.com/contest/263/problem/A) )

Cho ma trận kích thước 5x5, bao gồm 24 số 0 và duy nhất một số 1. Giả sử các dòng có chỉ số 1..5; các cột có chỉ số 1..5; Một bước đi hợp lệ là bước đi thỏa mãn điều kiện sau:

- Tráo đổi hai hàng cạnh nhau.
- Tráo đổi hai cột cạnh nhau.

Một ma trận được gọi là đẹp (beautiful matrix) nếu số 1 duy nhất được di chuyển về giữa ma trận. Đếm số lượng thao tác đổi để có được ma trận đẹp.

Input:

- Gồm 5 dòng chứa ma trận đã cho

Output:

- Một số duy nhất là số lượng bé nhất các thao tác cần được thực hiện để ma trận đã cho thành ma trận đẹp

Ví dụ:

| **Input** | **Output** |
| --- | --- |
| 0 0 0 0 00 0 0 0 10 0 0 0 00 0 0 0 00 0 0 0 0 | 3 |
| 0 0 0 0 00 0 0 0 00 1 0 0 00 0 0 0 00 0 0 0 0 | 1 |
