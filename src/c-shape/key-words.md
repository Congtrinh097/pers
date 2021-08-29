# Từ khóa (Keywords) trong C#

C# chứa các từ dành riêng có ý nghĩa đặc biệt cho trình biên dịch. Những từ dành riêng này được gọi là "từ khóa". Từ khóa không thể được sử dụng như một định danh (tên của một biến (variable), lớp (class), giao diện (interface), v.v.).

Các từ khóa trong C# được phân phối theo các danh mục sau:

## Từ khóa sửa đổi (Modifier Keywords)
Từ khóa sửa đổi là những từ khóa cụ thể cho biết ai có thể sửa đổi loại và loại thành viên. Các bộ sửa đổi cho phép hoặc ngăn các phần nhất định của chương trình bị các phần khác sửa đổi.

Bao gồm: abstract, async, const, event, extern, new, override, partial, readonly, sealed, static, unsafe, virtual

## Từ khóa quyền truy cập (Access Modifier Keywords) 
Các từ khóa quyền truy cập được áp dụng cho việc khai báo lớp, phương thức (method), thuộc tính(property), trường (field) và các thành viên khác. Chúng xác định khả năng truy cập của lớp và các thành viên của nó.

Bao gồm: 
| Từ khóa truy cập (Access Modifiers) |	Quyền truy cập |
|----------------|-----------|
| public	    | Cho phép bất kỳ phần nào của chương trình trong cùng một lớp hoặc một lớp khác có thể truy cập, sửa đổi vào kiểu và các phương thức, thuộc tính, trường của nó. |
| private	    | Hạn chế các phần khác của chương trình truy cập vào loại và các phương thức, thuộc tính, trường của nó. Chỉ mã trong cùng một lớp hoặc cấu trúc mới có thể truy cập nó. |
| internal	    | Cho phép mã chương trình khác trong cùng một hội đồng truy cập vào kiểu hoặc các các phương thức, thuộc tính, trường của nó. Đây là từ khóa quyền truy cập mặc định nếu không có định nghĩa nào được chỉ định. |
| protected	    | Cho phép các mã trong cùng một lớp hoặc một lớp dẫn xuất được kế thừa từ lớp đó truy cập vào kiểu hoặc các phương thức, thuộc tính, trường của nó. |

## Từ khóa tập lệnh (Statement Keywords)

Các từ khóa liên quan đến luồng xử lí của chương trình.

Bao gồm: if, else, switch, case, do, for, foreach, in, while, break, continue, default, goto, return, yield, throw, try, catch, finally, checked, unchecked, fixed, lock.

## Từ khóa tham số (Method Parameter Keywords)

Các từ khóa này được áp dụng cho các tham số của một phương pháp.

Bao gồm: params, ref, out

## Từ khóa không gian tên (Namespace Keywords)

Các từ khóa này được áp dụng với không gian tên và các toán tử liên quan.Bao gồm: using, toán từ dấu chấm (.), toán từ dấu hai chấm (::).

## Từ khóa truy cập (Access Keywords)
Các từ khóa truy cập được sử dụng để truy cập lớp chứa hoặc lớp cơ sở của một đối tượng hoặc lớp.

Bao gồm: base, this.

## Từ khóa định kiểu (Type Keywords)
Từ khóa loại được sử dụng cho các loại dữ liệu.

Bao gồm: bool, byte, char, class, decimal, double, enum, float, int, long, sbyte, short, string, struct, uint, ulong, ushort

## Từ khóa ngữ cảnh (Contextual Keywords)
Từ khóa theo ngữ cảnh được coi là từ khóa, chỉ khi được sử dụng trong các ngữ cảnh cụ thể. Chúng không được bảo lưu và vì vậy có thể được sử dụng làm tên hoặc định danh.

Bao gồm: add, var, dynamic, global, set, value

## Từ khóa truy vấn (Query Keywords)
Từ khóa truy vấn là các từ khóa theo ngữ cảnh được sử dụng trong các truy vấn LINQ.

Bao gồm: from, where, select, group, into, orderby, join, let, in, on, equals, by, ascending, descending

Như đã đề cập ở trên, một từ khóa không thể được sử dụng làm định danh (tên của biến, lớp, giao diện, v.v.). Tuy nhiên, chúng có thể được sử dụng với tiền tố '@'. Ví dụ, class là một từ khóa dành riêng, vì vậy nó không thể được sử dụng như một định danh, nhưng @class có thể được sử dụng như hình dưới đây.

```
public class @class
{
    public static int MyProperty { get; set; }
}

@class.MyProperty = 100;
```