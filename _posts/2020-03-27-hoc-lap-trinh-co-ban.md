---
title: "Hướng dẫn học lập trình cơ bản với C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---
# Giới thiệu

Cô liệt kê danh sách bài tập ở đây, theo thứ tự các em đã, đang và sẽ được thực hành trên lớp. Các em có thể làm và nộp bài bất cứ lúc nào tại địa chỉ cô để ở mỗi phần *(trang này cô sẽ tiếp tục cập nhật)*

Tài khoản đăng nhập: các em phải tạo tài khoản tại trang [Hackerrank](https://www.hackerrank.com). Có thể đăng nhập ngay bằng tài khoản Facebook hoặc Gmail sẽ nhanh hơn. Để thuận tiện cho việc kiểm soát việc học của các em, các em [điền thông tin đăng nhập vào form này](https://drive.google.com/open?id=1vZFQnoB2N8z_9tf54WIlX_30CI9bWdMWDvZiXWq3ylw) (*bắt buộc*).

Thuật toán và lập trình là kĩ năng cơ bản của thời đại công nghệ, nếu có nền tảng tốt các em sẽ có cơ hội phát triển cao hơn ở các bậc học sau này. Cô hy vọng các em tìm được niềm vui trong quá trình học thuật toán và lập trình, đừng quá lo lắng về điểm số. Trong quá trình học lập trình cơ bản, các em có thể ít nhiều gặp khó khăn, nhưng hãy bình tâm, dành thời gian suy nghĩ thêm, làm lại các bài tập (tốt nhất là theo thứ tự mà cô đề xuất).  

Những bài tập các em làm rồi, các em không nhất thiết phải làm lại. Nếu bạn nào còn cảm thấy chưa nhớ, chưa sử dụng thành thục được cú pháp ngôn ngữ thì nên làm lại các bài lần lượt từ đầu.

Các em có thể hỏi về các nội dung liên quan qua [facebook của cô](https://www.facebook.com/hoang.ha.3914). Các em có thể trao đổi với nhau, hướng dẫn nhau học, tuy nhiên với mục đích để hiểu và sau đó tự mình làm được.

# Danh sách bài tập thực hành

## 1. Kiểu dữ liệu, biến, hằng, phép gán, phép toán

[Link bài tập tối thiểu](https://www.hackerrank.com/co-ban-1)

[Lí thuyết: kiểu dữ liệu, biến, hằng, phép gán](http://thomasabc.xyz/posts/li-thuyet-cpp-co-ban/)

[Lí thuyết: phép toán trong C++](http://thomasabc.xyz/posts/toan-tu-cpp/)

* TONGAB
* TINHTOAN
* HCN
* DUONGTRON
* DODAI
* NHIETDO
* NHIETDO1

## 2. Cấu trúc rẽ nhánh

[Link bài tập tối thiểu](https://www.hackerrank.com/cau-truc-re-nhanh)

[Lí thuyết: cấu trúc rẽ nhánh](http://thomasabc.xyz/posts/cau-truc-re-nhanh/)

* MAX2
* CHANLE
* AMDUONG
* HOURS
* MAX3
* PTBACHAI
* XEPLOAI
* DAY
* DIGIT

## 3. Cấu trúc lặp

[Lí thuyết cấu trúc lặp](http://thomasabc.xyz/posts/cau-truc-lap/)

### 3.1. Lặp P1

[Link bài tập tối thiểu](https://www.hackerrank.com/cau-truc-lap-1)

* 1TON
* ATOB
* DOWNTO
* BANGNHAN
* EVEN
* EVENCNT
* SUM
* SUMN
* GIAITHUA
* UOCSO
* NUMBERTYPE
* SUMODDS
* SOHOANHAO
* NGUYENTO
* MAXX

### 3.2. Lặp P2

[Link bài tập tối thiểu](https://www.hackerrank.com/cau-truc-lap-2)

* DAONGUOC
* AMSTRONG
* SODAONGUOC
* PALINDROME
* DOCSO
* **VIETBANGCHU (Bài tập thêm)**

### 3.3. Lặp P3

[Link bài tập tối thiểu](https://www.hackerrank.com/cau-truc-lap-3)

* LKNGUYENTO
* LKSOHOANHAO
* LKAMSTRONG
* SQUARESTARS
* HOLLOWSTARS
* RTRIANGLE
* LTRIANGLE
* RETRIANGLE
* LETRIANGLE

## 4. Kiểu mảng

* [Lí thuyết kiểu mảng 1 chiều, 2 chiều](http://thomasabc.xyz/posts/kieu-mang/)


### 4.1. Mảng một chiều

[Video bài giảng mảng 1 chiều](https://youtu.be/5bazasTqi3E)

[Link bài tập tối thiểu](https://www.hackerrank.com/mang-mot-chieu)

* REVERSE
* SUMATION
* SUMODDS
* REPLACEMENT
* FINDMAX
* POSITION
* FIRSTLAST
* SWAPMINMAX
* MAXPAIR
* INSERTX
* DECTOBIN
* SEARCHING
* **DELETEX (Bài tập làm thêm)**
* **SELECTIONSORT (Bài tập làm thêm)**

### 4.2. Mảng hai chiều

[Video bài giảng mảng 2 chiều](https://youtu.be/BQqBoKbxAOE)

[Link bài tập tối thiểu](https://www.hackerrank.com/mang-hai-chieu)

Các em nên khai báo các mảng bên ngoài hàm main. Như ví dụ:
```cpp
#include <bits/stdc++.h>
using namespace std;

//Nên khai báo như thế này
const int maxN=1000;
int A[maxN][maxN];

int main(){
  //Không nên khai báo trong hàm main thế này
  int N; cin >> N;
  int a[N][N];
  
}
```

* 2DARRAY
* MATRIXSUM
* MAINDIAGONAL
* MINORDIAGONAL
* SWAPDIAGONAL
* UPPERMATRIX
* LOWERMATRIX
* TRANSPOSE
* **AMATRIX (bài tập thêm)**
* **MATRIXADD (bài tập thêm)**
* **MATRIXMUL (bài tập thêm)**
* **MATRIX (bài tập thêm)**
* **BINARYMATRIX (bài tập thêm)**
* **CARO (bài tập thêm)**

## 5. Hàm (Functions)

### 5.1. Sử dụng hàm có sẵn trong thư viện

[Video bài giảng hàm P1](https://youtu.be/7BkGPlVgw-8)

[Lí thuyết hàm](http://thomasabc.xyz/posts/ham-function/)

Do có chút vấn đề trên Hackerrank nên cô phải đưa 4 bài Hàm (P1) vào thành bài 8, 9, 10, 11 của phần Cơ bản 1. Các em vào làm ở link dưới đây.

[Link bài tập hàm P1](https://www.hackerrank.com/co-ban-1)

* UPPERLOWER
* TOLOWER
* COUNTABCDEF
* **COUNTAZ (bài tập làm thêm)**

### 5.2. Hàm do người dùng tự định nghĩa

* [Video bài giảng: cách viết và sử dụng hàm](https://youtu.be/3v9g50A5VQU)
* [Video bài giảng: cách truyền tham số cho hàm](https://youtu.be/jxyPtkiNHS4)
* [Video bài giảng: cách truyền tham số là mảng cho hàm](https://youtu.be/GHhPvj_hkyg)
* [Video bài giảng: Biến cục bộ và biến toàn cục](https://youtu.be/F7URg7dTlz4)

[Link bài tập hàm P2](https://www.hackerrank.com/co-ban-1)

* CONG
* MAXI
* TRAODOI
* CUBE
* ISEVEN
* CIRCLE
* ISPRIME
* ISPERFECT
* FACT
* FUNC
* **SEARCHFORX (bài tập làm thêm)**
* **RUTGONPS (bài tập làm thêm)**
* **Trò chơi Tic-Tac-Toe (bài tập làm thêm)** [Đề và nộp bài này ở đây - bạn phải có tài khoản ở Codeforces](https://codeforces.com/group/bDOIjJTvcH/contest/275680/problem/C)

### 5.3. Hàm đệ quy

[Danh sách bài tập luyện tập hàm đệ quy](https://www.hackerrank.com/ham-de-quy)

[Video bài giảng hàm đệ quy]()

* FACT
* INHELLO
* FIBO1
* EXPO
* FASTEXP
* GCD
* PRINTARR
* CKN
* MAXIMUM **(Làm thêm)**
* BINARYSEARCH **(Làm thêm)**
* HANOITOWER **(Làm thêm)**

## 6. Các thuật toán cơ bản

[Video hướng dẫn thuật toán]()

[Danh sách bài tập](https://www.hackerrank.com/ham-de-quy/)

* ERATOS
* SELECTIONSORT
* SELECTIONSORT1
* BUBBLESORT
* INSERTIONSORT

## 7. Ôn kiểm tra học kì 2

[Danh sách bài tập: bài 17, 18, 19, 20, 21](https://www.hackerrank.com/ham-de-quy/)

* COMPARE
* ONES
* HEXA
* KPRIME
* COCKTAILSORT
