---
title: "Một số toán tử trong C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---
Một toán tử là một biểu tượng, mà nói cho trình biên dịch thực hiện các thao tác toán học và logic cụ thể. C++ cung cấp nhiều loại toán tử có sẵn:
* Toán tử số học
* Toán tử quan hệ
* Toán tử logic
* Toán tử so sánh bit
* Toán tử gán
* Toán tử hỗn hợp

# 1. Toán tử số học

Giả sử biến A giữ giá trị 10, biến B giữ 20 thì:

| Toán tử | Miêu tả | Ví dụ |
|--|--|--|
| + | Cộng hai toán hạng |A + B kết quả là 30
| - | Trừ toán hạng thứ hai từ toán hạng đầu |A - B kết quả là -10
| * | Nhân hai toán hạng |A * B kết quả là 200
| / | Phép chia |B / A kết quả là 2
| % | Phép lấy số dư |B % A kết quả là 0
| ++ | Tăng giá trị toán hạng thêm một đơn vị |A++ kết quả là 11
| -- | Giảm giá trị toán hạng đi một đơn vị |A-- kết quả là 9

(Nguồn vietjack)

# 2. Toán tử quan hệ

Toán tử quan hệ thể hiện mối quan hệ giữa hai biểu thức, giá trị. Các toán tử quan hệ chính: >,<,>=,<=,==,!=

|Toán tử|Miêu tả|Ví dụ|
|--- |--- |--- |
|==|Kiểm tra nếu 2 toán hạng bằng nhau hay không. Nếu bằng thì điều kiện là true.|(A == B) là không đúng|
|!=|Kiểm tra 2 toán hạng có giá trị khác nhau hay không. Nếu không bằng thì điều kiện là true.|(A != B) là true|
|>|Kiểm tra nếu toán hạng bên trái có giá trị lớn hơn toán hạng bên phải hay không. Nếu lớn hơn thì điều kiện là true.|(A > B) là không đúng|
|<|Kiểm tra nếu toán hạng bên trái nhỏ hơn toán hạng bên phải hay không. Nếu nhỏ hơn thì là true.|(A < B) là true|
|>=|Kiểm tra nếu toán hạng bên trái có giá trị lớn hơn hoặc bằng giá trị của toán hạng bên phải hay không. Nếu đúng là true.|(A >= B) là không đúng|
|<=|Kiểm tra nếu toán hạng bên trái có giá trị nhỏ hơn hoặc bằng toán hạng bên phải hay không. Nếu đúng là true.|(A <= B) là true|

# 3. Toán tử logic

Giả sử biến A có giá trị 1 (true) và biến B có giá trị 0 (false):

|Toán tử|Miêu tả|Ví dụ|
|--- |--- |--- |
|&&|Được gọi là toán tử logic AND (và). Nếu cả hai toán tử đều có giá trị khác 0 thì điều kiện trở lên true.|(A && B) là false.|
|\|\||Được gọi là toán tử logic OR (hoặc). Nếu một trong hai toán tử khác 0, thì điều kiện là true.|(A || B) là true.|
|!|Được gọi là toán tử NOT (phủ định).  Sử dụng để đảo ngược lại trạng thái logic của toán hạng đó. Nếu điều kiện toán hạng là true thì phủ định nó sẽ là false.|!(A && B) là true.|

# 4. Toán tử gán

Thực hiện việc gán giá trị. Trong C++ có nhiều thể hiện của phép gán, nhưng cơ bản hoạt động của nó giống như phép gán được mô tả trong bài trước.

|Toán tử|Miêu tả|Ví dụ|
|--- |--- |--- |
|=|Toán tử gán đơn giản. Gán giá trị toán hạng bên phải cho toán hạng trái.|C = A + B sẽ gán giá trị của A + B vào trong C|
|+=|Thêm giá trị toán hạng phải tới toán hạng trái và gán giá trị đó cho toán hạng trái.|C += A tương đương với C = C + A|
|-=|Trừ đi giá trị toán hạng phải từ toán hạng trái và gán giá trị này cho toán hạng trái.|C -= A tương đương với C = C - A|
|*=|Nhân giá trị toán hạng phải với toán hạng trái và gán giá trị này cho toán hạng trái.|C *= A tương đương với C = C * A|
|/=|Chia toán hạng trái cho toán hạng phải và gán giá trị này cho toán hạng trái.|C /= A tương đương với C = C / A|
|%=|Lấy phần dư của phép chia toán hạng trái cho toán hạng phải và gán cho toán hạng trái.|C %= A tương đương với C = C % A|

