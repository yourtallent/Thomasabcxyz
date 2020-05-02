---
title: "Bài tập luyện tập CF-A-1"
categories: [Học thuật toán, học lập trình, C++]
tags: [học thuật toán và lập trình]
---
# CF-A.11. Magnets

([http://codeforces.com/contest/344/problem/A](http://codeforces.com/contest/344/problem/A) )

Nhà khoa học điên Mike tự giải trí bằng cách sắp xếp các hàng domino. Tuy nhiên, anh không cần domino: anh sử dụng nam châm hình chữ nhật. Mỗi nam châm có hai cực, dương (một dấu &quot;+&quot;) và âm (một dấu &quot;-&quot;). Nếu hai nam châm được đặt lại với nhau ở khoảng cách gần, thì các cực giống nhau sẽ đẩy nhau và các cực đối diện sẽ hút nhau.

Mike bắt đầu bằng cách đặt một nam châm nằm ngang trên bàn. Trong mỗi bước tiếp theo, Mike thêm một nam châm khác theo chiều ngang vào đầu bên phải của hàng. Tùy thuộc vào cách Mike đặt nam châm lên bàn, nó bị hút vào bảng trước đó (tạo thành một nhóm nhiều nam châm liên kết với nhau) hoặc đẩy nó (sau đó Mike đặt nam châm ở khoảng cách nào đó phía phải của nam châm trước đó) . Chúng tôi giả định rằng một nam châm duy nhất không liên kết với nam châm khác tạo thành một nhóm riêng của nó (chỉ gồm 1 nam châm).

![](RackMultipart20200502-4-b5e5r2_html_5cce1653a667213e.png)

Mike xếp nhiều nam châm trên một hàng, bạn hãy đếm giúp có bao nhiêu nhóm nam châm được hình thành?

Input:

- Dòng đầu ghi số nguyên n (1 ≤ _n_ ≤ 100000) – là số lượng nam châm.
- N dòng tiếp theo mỗi dòng ghi trạng thái của một nam châm gồm hai cực +-; nếu nam châm đặt là &quot;+-&quot; biểu diễn bằng số &quot;10&quot;, nam châm đặt &quot;-+&quot; biểu diễn bằng số &quot;01&quot;

Output:

- Một số nguyên duy nhất là số lượng nhóm nam châm tạo thành.

Ví dụ:

| **Input** | **Output** |
| --- | --- |
| 6101010011010 | 3 |
| 401011010 | 2 |
