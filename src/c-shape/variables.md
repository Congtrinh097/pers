# Biến (Variables) trong C#

Trong C #, một biến chứa giá trị dữ liệu của kiểu dữ liệu (Data Type) cụ thể
```
<data type> <variable name> = <value>;
```
* Sau đây là khai báo và khởi tạo một biến kiểu int.
```
int number = 10;
```
Như ví dụ trên, *int* là kiểu dữ liệu, *number* là tên biến, *=* là toán từ gán giá trị, *10* là giá trị được gán cho biến.

* Sau đây khai báo và khởi tạo các biến của các kiểu dữ liệu khác nhau.
```
int num = 100;
float rate = 10.2f;
decimal amount = 100.50M;
char code = 'C';
bool isValid = true;
string name = "Steve";
```
* Sau đây là các quy ước đặt tên để khai báo các biến trong C #:
  - Tên biến phải là duy nhất.
  - Tên biến chỉ có thể chứa các chữ cái, chữ số và dấu gạch dưới _.
  - Tên biến phải bắt đầu bằng một chữ cái.
  - Tên biến có phân biệt chữ hoa chữ thường, num và Num được coi là các tên khác nhau.
  - Tên biến không được chứa các từ khóa (key words) dành riêng. Phải đặt tiền tố @ trước từ khóa nếu muốn đặt trước từ khóa làm tên biến.
* C # là ngôn ngữ định kiểu. Nó có nghĩa là bạn chỉ có thể gán một giá trị của kiểu dữ liệu được chỉ định. Bạn không thể gán giá trị số nguyên cho kiểu chuỗi hoặc ngược lại.
``` 
//compile error
int num = "Steve";
```
* Biến có thể được khai báo trước và khởi tạo sau.
```
int num;
num = 100;
```
* Một biến phải được gán một giá trị trước khi sử dụng nó, nếu không, C # sẽ đưa ra lỗi thời gian biên dịch.
```
int i;
int j = i; //compile-time error: Use of unassigned local variable 'i'
```
* Giá trị của một biến có thể được thay đổi bất cứ lúc nào sau khi khởi tạo nó.
```int num = 100;
num = 200;
num = 300;
Console.WriteLine(num); //output: 300
```
* Nhiều biến của cùng một kiểu dữ liệu có thể được khai báo và khởi tạo trong một dòng duy nhất được phân tách bằng dấu phẩy.
```
int i, j = 10, k = 100;
```
* Nhiều biến cùng kiểu cũng có thể được khai báo trên nhiều dòng cách nhau bằng dấu phẩy. Trình biên dịch sẽ coi nó là một câu lệnh cho đến khi nó gặp dấu chấm phẩy ;
```
    int i = 0, 
    j = 10, 
    k = 100;
```
* Giá trị của một biến có thể được gán cho một biến khác có cùng kiểu dữ liệu. Tuy nhiên, một giá trị phải được gán cho một biến trước khi sử dụng nó.
```
  int i = 100;
  int j = i; // value of j will be 100
```
* Trong C #, các biến được phân loại dựa trên cách chúng lưu trữ giá trị của chúng trong bộ nhớ. Các biến có thể là kiểu giá trị hoặc kiểu tham chiếu hoặc kiểu con trỏ.

* Không nhất thiết phải chỉ định kiểu cụ thể khi khai báo biến. Sử dụng từ khóa *var* thay vì một kiểu dữ liệu.
