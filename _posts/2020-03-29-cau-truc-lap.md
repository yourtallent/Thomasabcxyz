---
title: "Cấu trúc lặp trong C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---

Ngôn ngữ lập trình cung cấp cho chúng ta nhiều cấu trúc điều khiển và cho phép bạn thực hiện những phần phức tạp.

Vòng lặp cho phép thực hiện một lệnh và một nhóm lệnh nhiều lần.

Có hai mô hình cấu trúc lặp: 

* Lặp với điều kiện trước 

![Lặp với điều kiện trước](http://thomasabc.xyz/assets/img/while.png)

* Lặp với điều kiện sau

![Lặp với điều kiện trước](http://thomasabc.xyz/assets/img/dowhile.png)

C++ hỗ trợ ba loại vòng lặp

## 1. Vòng lặp while

**Cú pháp:**

```cpp
while(dieu_kien)  
{ 
	cac_lenh;  
}
```

**Hoạt động:**

Ở đây, **cac_lenh** có thể là lệnh đơn hoặc một khối các lệnh. **dieu_kien** có thể là bất kỳ biểu thức nào, và giá trị *true* là bất kỳ giá trị nào khác 0. Vòng lặp lặp đi lặp lại trong khi **dieu_kien** là *true*.

Hoạt động vòng lặp while là thể hiện của mô hình lặp với điều kiện trước ở trên.

## 2. Vòng lặp for

Vòng lặp for là một thể hiện của mô hình lặp với điều kiện trước, tương tự như while nhưng với cú pháp ngắn gọn hơn.  

**Cú pháp:**

```cpp
for  ( bien; dieu_kien; tang_giam )  { 
	cac_lenh;  
}
```

**Hoạt động:**

![Hoạt động vòng lặp for](https://vietjack.com/cplusplus/images/vong_lap_for_trong_cpp.jpg)

## 3. Vòng lặp do...while

Không giống như các vòng lặp  **for**  và  **while**, mà kiểm tra điều kiện vòng lặp ở ngay bước đầu tiên của vòng lặp, vòng lặp  **do…while**  trong Ngôn ngữ C++ kiểm tra điều kiện của nó tại phần cuối của vòng lặp.

Một vòng lặp  **do…while**  là tương tự như vòng lặp while, ngoại trừ ở điểm một vòng lặp do…while bảo đảm *thực hiện vòng lặp ít nhất một lần*

**Cú pháp:**
```cpp
do  { 
	cac_lenh;  
} while( dieu_kien );
```

**Hoạt động:**

![Hoạt động của vòng lặp do-while](https://vietjack.com/cplusplus/images/vong_lap_do_while_trong_cpp.jpg)
