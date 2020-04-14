
---
title: "Hàm trong C++"
categories: [Học lập trình, C++]
tags: [học lập trình]
---
# 1. Giới thiệu về hàm

Một chương trình C++ được cấu trúc từ nhiều hàm, trong đó hàm main là hàm bắt buộc cần phải có. Việc viết mọi lệnh vào chung hàm main chỉ phù hợp với các chương trình đơn giản, có số lượng câu lệnh nhỏ. Khi chương trình phức tạp hơn, cần thiết phải chia nhỏ bài toán thành các phần độc lập và có thể quản lí được.

**Hàm**: Một hàm là một nhóm các câu lệnh cùng nhau thực hiện một nhiệm vụ. Hàm có thể nhận giá trị vào (input) và trả về giá trị (output).

**Một số lợi ích khi sử dụng hàm trong lập trình:**

 - Tái sử dụng mã chương trình
 - Làm cho chương trình sáng sủa hơn, dễ đọc, dễ sửa
 - Có thể phân chia công việc cho nhiều người bằng cách chia nhỏ thành nhiều hàm

# 2. Một số hàm có sẵn trong thư viện

Thư viện chuẩn C++ cung cấp nhiều hàm được tích hợp sẵn mà chương trình của bạn có thể gọi. Ví dụ,  **sqrt**(x) để tính giá trị căn bậc 2 của x,  **pow**(x,y) để tính giá trị x mũ y.

Dưới đây là mô tả về một số hàm có sẵn trong C++. Ngoài những hàm này, trong thư viện của NNLT còn cung cấp rất nhiều hàm khác, việc sử dụng các hàm có sẵn rất thuận tiện trong việc thiết kế, xây dựng chương trình.

- abs(x): Trả về giá trị tuyệt đối của x
- ceil(x): trả về số thực (không có phần thập phân) lớn hơn gần x nhất
- floor(x): trả về số thực (không có phần thập phân) bé hơn gần x nhất
- exp(x): trả về e mũ x
- sqrt(x): trả về căn bậc hai của x
- pow(x,y): trả về x mũ y
- islower(x): trả về true nếu x là kí tự thường, ngược lại trả về false
- isupper(x): trả về true nếu x là kí tự hoa, ngược lại trả về false
- tolower(x): trả về kí tự thường của x
- toupper(x): trả về kí tự hoa của x

# 3. Hàm do người dùng định nghĩa

Do thư viện không cung cấp đủ các hàm cần thiết phục vụ quá trình giải quyết vấn đề nên thông thường người lập trình cần thiết phải viết riêng các hàm phục vụ nhu cầu cá nhân của mình. Việc viết chương trình bằng cách phân rã chương trình thành các hàm, mỗi hàm thực hiện một công việc cụ thể sẽ giúp chương trình sáng sủa, dễ đọc, dễ chỉnh sửa hơn.

## 3.1. Cấu trúc hàm

**Cú pháp:**
```cpp
<kiểuDL_trả_về> <tên_hàm>(<danh_sách_tham_số>){
	<các_lệnh_thân_hàm>;
}
```
**Phần đầu hàm:** 
```cpp 
<kiểuDL_trả_về> <tên_hàm>(<danh_sách_tham_số>)
```
Trong đó <danh_sách_tham_số> được xem như input của hàm, được trình bày theo cú pháp dưới đây, hàm có thể gồm 0 hoặc nhiều tham số:
```cpp
<kiểuDL> <tham_số1>, <kiểuDL> <tham_số2>,... 
```
Phần <kiểuDL_trả_về> được xem như output của hàm, xác định kiểu dữ liệu trả về của hàm. Nếu hàm không trả về giá trị, <kiểuDL_trả_về> sẽ có kiểu *void*. Nếu hàm có trả về giá trị, trong thân hàm bắt buộc phải có câu lệnh *return*.

**Ví dụ:**

Hàm *Cong* tính tổng ba số nguyên, trả về giá trị là một số nguyên:
```cpp
int Cong(int a, int b, int c){
	return a + b +c;
}
```
Hàm *HienThi* nhận dữ liệu đầu vào là một xâu kí tự, chỉ thực hiện việc in ra màn hình xâu kí tự đó:
```cpp
void HienThi(string s){
	cout << s << endl;
}
```
**Phần thân hàm:**
```cpp
{
	<các_lệnh_thân_hàm>;
}
```
Các lệnh thân hàm tập trung giải quyết mục đích của hàm đó. Nếu hàm có trả về giá trị, trong thân hàm phải chứa câu lệnh *return*.

## 3.2. Ví dụ về cách viết và sử dụng hàm

*Các biến trong danh sách tham số phần đầu hàm còn gọi là tham số hình thức*

**Ví dụ 1:** Hàm so sánh hai số nguyên a, b nếu a>b trả về true, ngược lại trả về false?
```cpp
bool SoSanh(int a, int b){
	if (a>b) return true;
	else return false;
}
```
**Ví dụ 2:** Hàm đánh giá điểm TB, nếu điểm TB thuộc [0,5) loại D; [5,6.5) C; [6.5,8) B; [8,10] A --> nhận vào số thực TB, trả về một kí tự tương ứng với TB:
```cpp
char DanhGia(double TB){
	if (TB>=8) return 'A';
	else if (TB>=6.5) return 'B';
	else if (TB>=5) return 'C';
	else return 'D';
}
```
**Ví dụ 3:** Hàm thực hiện việc thông báo ra màn hình một mảng A1, A2,...,AN có kích thước N các số nguyên --> Tham số là mảng số nguyên A, số nguyên N; không trả về giá trị:
```cpp
void InMang(int A[], int N){
	for (int i=1; i<=N; i++)
		cout << A[i] << " ";
}
```
**Sử dụng hàm:**
Gọi hàm thông qua tên và danh sách tham số theo cú pháp sau:
```cpp
<tên_hàm>(<danh_sách_đối_số>);
```

*Khi đó <danh_sách_đối_số> được gọi là tham số thực sự*

Ví dụ: Gán biến nguyên c bằng tổng của hai số 7,9 bằng hàm Cong ở trên
```cpp
int c = Cong(7,9);
```
Ví dụ: Có mảng B kích thước 5 phần tử, tiến hành in ra mảng B sử dụng hàm InMang ở trên
```cpp
InMang(B,5);
```

# 4. Cách truyền tham số cho hàm

Tham số của hàm là những biến được khai báo trong việc khai báo hàm. Tham số đóng vai trò tiếp nhận giá trị đầu vào cho hàm mỗi khi hàm được gọi.  Ta tìm hiểu 2 kiểu truyền đối số cơ bản: truyền giá trị và truyền tham chiếu.

## 4.1. Truyền giá trị

Truyền đối số vào hàm là giá trị có nghĩa là chúng ta sẽ đưa giá trị vào hàm và các tham số sẽ tiếp nhận những giá trị được truyền vào.
```cpp
void TraoDoi(int x, int y)
{
	int tmp = x; 
	x = y;
	y = tmp;
}
int main(){
	int a = 10, b = 15;
	TraoDoi(a,b);
	cout << a << " " << b;
}
```

Ở đây, khi thực hiện hàm main sẽ gọi đến hàm TraoDoi, giá trị x sẽ được gán bằng a tức là x = 10, y được gán bằng b tức là y = 8 làm input cho hàm TraoDoi; hàm TraoDoi thực hiện việc tráo đổi giá trị hai biến x, y và hai biến này sẽ bị vô hiệu hóa khi kết thúc hàm TraoDoi. Bởi vậy, giá trị được in ra màn hình vẫn là giá trị của a, b tức là 10 và 15. Cách truyền này được gọi là truyền bằng giá trị. 

## 4.2. Truyền tham chiếu

Để có thể làm thay đổi giá trị hai biến a, b ở ví dụ trên; tức là giá trị in ra sau khi tráo đổi phải là 15 và 10 ta tiến hành truyền bằng tham chiếu như sau:
```cpp
void TraoDoi(int &x, int &y)
{
	int tmp = x; 
	x = y;
	y = tmp;
}
int main(){
	int a = 10, b = 15;
	TraoDoi(a,b);
	cout << a << " " << b;
}
```
Một tham chiếu được xem như một cái tên khác của một biến khác có cùng kiểu dữ liệu. Sau khi biến tham chiếu được khai báo và khởi tạo, nó sử dụng chung vùng nhớ với biến mà nó tham chiếu đến.

Khi một trong hai biến bị hủy (biến tham chiếu hay biến gốc bị hủy do ra khỏi khối lệnh mà nó được khai báo), vùng nhớ mà 2 biến này kiểm soát vẫn chưa bị hủy nếu còn ít nhất 1 biến quản lý nó, cái bị hủy sẽ chỉ là tên biến.

Như vậy, sau khi thực hiện hàm TraoDoi, giá trị của hai ô nhớ a, b đã được thay đổi do quá trình tráo đổi trong hàm TraoDoi ở trên. Bởi thế, giá trị được in ra màn hình tương ứng a, b là 15 và 10.

**Vậy khi nào dùng cách truyền giá trị, khi nào dùng cách truyền tham chiếu?**

-   Khi truyền đối số cho hàm là giá trị, cách duy nhất để có được đầu ra là trả về giá trị thông qua từ khóa return.  
-   Khi truyền đối số cho hàm là giá trị, hảm chỉ có thể trả về 1 giá trị duy nhất tại 1 lần gọi hàm (nếu hàm có kiểu trả về).
- Dùng cách truyền tham chiếu khi muốn thay đổi nhiều giá trị thông qua nhiều tham số trong hàm.

# 5. Biến toàn cục và biến cục bộ
## 5.1. Biến cục bộ

Các biến được khai báo bên trong một hàm hoặc khối là các biến cục bộ (local). Chúng chỉ có thể được sử dụng bởi các lệnh bên trong hàm hoặc khối code đó. Ví dụ, hàm main có 3 biến cục bộ là a, b, c:
```cpp
int main ()  {  
	int a, b;  
	int c;  

	a =  10; 
	b =  20; 
	c = a + b; 
	
	cout << c;  
	return  0;  
}
```
Biến cục bộ x, y, tmp chỉ tồn tại trong khi hàm TraoDoi hoạt động, biến a,b là biến cục bộ thuộc hàm main:
```cpp
void TraoDoi(int &x, int &y)
{
	int tmp = x; 
	x = y;
	y = tmp;
}
int main(){
	int a = 10, b = 15;
	TraoDoi(a,b);
	cout << a << " " << b;
}
```
## 5.2. Biến toàn cục

Biến toàn cục (global) trong C++ được định nghĩa bên ngoài các hàm, thường ở phần đầu chương trình. Các biến toàn cục giữ giá trị của nó trong suốt quá trình chạy chương trình. Các biến toàn cục có thể được truy cập ở mọi vị trí trong chương trình.

Ví dụ: biến g là biến toàn cục, có thể được sử dụng trong các hàm khác, trong hàm main...
```cpp
int g;
void Xuli(){
	g++;
}
int main (){
  int a, b;
  a = 10;
  b = 20;
  Xuli();
  g = a + b;
  cout << g;
 return 0;
}
```
Một chương trình có thể có các biến toàn cục và biến cục bộ cùng tên với nhau, nhưng trong một hàm thì giá trị của biến cục bộ sẽ được ưu tiên.
