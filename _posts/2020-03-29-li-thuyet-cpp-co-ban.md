---
title: "Kiểu dữ liệu, biến, hằng, phép gán C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---
# 1. Chương trình C++
## 1.1. Chương trình C++ đơn giản
In ra dòng chữ Hello World
```cpp 
#include  <iostream>  
using  namespace std;  

int main()  { 
	cout <<  "Hello World";    
	return  0;  
}
```
## 1.2. Dấu chấm phảy (;) và khối (block) trong C++
Trong C++, dấu chấm phảy là ký tự kết thúc lệnh (statement terminator). Nghĩa là, mỗi lệnh đơn phải kết thúc bởi một dấu chấm phảy. Nó chỉ dẫn sự kết thúc của một thực thể logic.

Dưới đây là ví dụ về 3 lệnh khác nhau:
```cpp
x = y; 
y = y+1; 
add(x, y);
```
Một khối (block) là một tập hợp các lệnh được kết nối một cách logic, mà được bao quanh bởi các dấu ngoặc móc mở và đóng. Ví dụ:
```cpp
{ 
	cout <<  "Hello CPP!";  
	return  0;  
}
```
## 1.3. Định danh (tên) trong C++
Một tên (Identifier) bắt đầu với một chữ cái từ A tới Z hoặc từ a tới z hoặc một dấu gạch dưới (_) được theo sau bởi 0 hoặc nhiều chữ cái, dấu gạch dưới và chữ số (từ 0 tới 9)
```cpp
hoang       nam    abc   sinh_vien  a_123
caogia50   _nhanvien   j     a23b9     
```
## 1.4. Comment trong C/C++
Comment của chương trình là các lời diễn giải, giúp cho bất kỳ ai đọc chương trình dễ dàng hơn.
```cpp
/* Day la mot comment don dong */  
/* C/C++ cung ho tro cac comment
 * ma co nhieu dong
 */
```
# 2. Kiểu dữ liệu, biến, hằng, phép gán
## 2.1. Kiểu dữ liệu
Các biến, không gì khác ngoài các vị trí bộ nhớ được dành riêng để lưu giá trị. Nghĩa là, khi bạn tạo một biến, bạn dành riêng một số không gian trong bộ nhớ cho biến đó.
## 2.2. Kiểu dữ liệu nguyên thủy trong C++
Một số kiểu dữ liệu nguyên thủy phổ biến:

|Kiểu dữ liệu|Từ khóa|
|--- |--- |
|Boolean|bool|
|Ký tự|char|
|Số nguyên|int|
|Số thực|float|
|Số thực dạng Double|double|
|Kiểu không có giá trị|void|

## 2.3. Khai báo biến
Định nghĩa biến trong C/C++ nghĩa là nói cho compiler nơi và lượng bộ nhớ cần tạo để lưu giữ biến đó.

Cú pháp khai báo biến:
```cpp
kieu_du_lieu danh_sach_bien;
```
Ví dụ:
```cpp
int j, q, k;  
char v, viet;  
float x, diemthi;  
double luong;
```
Có thể khởi tạo giá trị cho biến trong lệnh khai báo biến. Ví dụ:
```cpp
int d =  3, f =  5;  // dinh nghia va khoi tao bien d va f.  
char x =  'A';  // bien x co gia tri la 'A'.
```
## 2.4. Phạm vi biến
Một phạm vi là một khu vực của chương trình nơi biến hoạt động. 

Ví dụ 1: Biến cục bộ
Các biến được khai báo bên trong một hàm hoặc khối là các biến cục bộ (local). Chúng chỉ có thể được sử dụng bởi các lệnh bên trong hàm hoặc khối code đó.
```cpp
#include  <iostream>  
using  namespace std;  
int main ()  {  
	// Khai báo biến cục bộ a, b, c chỉ hoạt động trong hàm main  
	int a, b;  int c;  
	a =  10; b =  20; c = a + b; 
	cout << c;  
	return  0;  
}
```
Ví dụ 2: Biến toàn cục
Biến toàn cục (global) trong C++ thường được khai báo ở phần đầu chương trình. Các biến toàn cục giữ giá trị của nó trong suốt vòng đời chương trình của bạn.
```cpp
#include  <iostream>  
using  namespace std;  
// phan khai bao bien toan cuc
int g;  
int main ()  {  
	// phan khai bao bien cuc bo
	int a, b;  
	a =  10; b =  20; 
	g = a + b; 
	cout << g;  
	return  0;  
}
```
## 2.5. Hằng
Hằng là đối tượng được đối xử giống như các biến thông thường, ngoại trừ việc giá trị của chúng là không thể thay đổi sau khi định nghĩa.
Cú pháp khai báo hằng:
```cpp
const <kieu_du_lieu> <TÊN_HẰNG> = <giá_trị>;
```
Ví dụ:
```cpp
const int maxN = 1000;
const double PI = 3.14;
const char ok = 'Y';
const string name = "THPT CBN";
```
## 2.6. Phép gán
Phép gán thực hiện gán giá trị cho một biến.
Cú pháp phép gán:
```cpp
<biến> = <biểu_thức>;
```
Hoạt động của phép gán: tính toán giá trị <biểu_thức>, sau đó gán giá trị cho <biến>
Ví dụ:
```cpp
int x = 4;
int d = PI*x+32;
bool ok = NOT(3>2);
```
