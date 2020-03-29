---
title: "Cấu trúc rẽ nhánh trong C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---
Khi thực hiện việc lựa chọn thông qua ra quyết định, ta sử dụng cấu trúc rẽ nhánh để điều khiển. Ví dụ:
> 1. Nếu trời mưa thì ta sẽ ở nhà, ngược lại sẽ đi đá bóng
> 2. Nếu A là số chẵn thì thông báo "EVEN" ngược lại thông báo "ODD"
> 3. Nếu i>N thì kết thúc chương trình

# 1. Cấu trúc if-else

Mô hình cấu trúc rẽ nhánh dạng khuyết **if (<đk>) <công_việc>;**

![Mô hình cấu trúc rẽ nhánh dạng khuyết](http://thomasabc.xyz/assets/img/if.png)

Cấu trúc rẽ nhánh dạng đầy đủ **if (<đk>) <công_việc_1>; else <công việc 2>;**

![Mô hình cấu trúc rẽ nhánh dạng đầy đủ](http://thomasabc.xyz/assets/img/if-else.png)

Ví dụ 1: Nếu x là số chẵn thì thông báo EVEN, ngược lại thông báo ODD
```cpp
if (x%2==0) cout << "EVEN";
else cout << "ODD";
```
Ví dụ 2: Nếu k > 10 thì kết thúc chương trình
```cpp
if (k>10) return 0;
```
# 2. Cấu trúc switch
