# Từ khóa

C# chứa các từ dành riêng có ý nghĩa đặc biệt cho trình biên dịch. Những từ dành riêng này được gọi là "từ khóa". Từ khóa không thể được sử dụng như một định danh (tên của một biến (variable), lớp (class), giao diện (interface), v.v.).

Các từ khóa trong C# được phân phối theo các danh mục sau:

## Từ khóa sửa đổi (Modifier Keywords)
Từ khóa sửa đổi là những từ khóa cụ thể cho biết ai có thể sửa đổi loại và loại thành viên. Các bộ sửa đổi cho phép hoặc ngăn các phần nhất định của chương trình bị các phần khác sửa đổi.

Bao gồm các từ khóa: abstract, async, const, event, extern, new, override, partial, readonly, sealed, static, unsafe, virtual

## Từ khóa truy cập sửa đổi (Access Modifier Keywords) 
Các từ khóa sửa đổi truy cập được áp dụng cho việc khai báo lớp, phương thức (method), thuộc tính(property), trường (field) và các thành viên khác. Chúng xác định khả năng truy cập của lớp và các thành viên của nó.

Bao gồm các từ khóa: 
| Từ khóa truy cập (Access Modifiers) |	Quyền truy cập |
|----------------|-----------|
| public	    | Cho phép bất kỳ phần nào của chương trình trong cùng một lớp hoặc một lớp khác có thể truy cập, sửa đổi vào kiểu và các phương thức, thuộc tính, trường của nó. |
| private	    | Hạn chế các phần khác của chương trình truy cập vào loại và các phương thức, thuộc tính, trường của nó. Chỉ mã trong cùng một lớp hoặc cấu trúc mới có thể truy cập nó. |
| internal	    | Cho phép mã chương trình khác trong cùng một hội đồng truy cập vào kiểu hoặc các các phương thức, thuộc tính, trường của nó. Đây là từ khóa quyền truy cập mặc định nếu không có định nghĩa nào được chỉ định. |
| protected	    | Cho phép các mã trong cùng một lớp hoặc một lớp dẫn xuất được kế thừa từ lớp đó truy cập vào kiểu hoặc các phương thức, thuộc tính, trường của nó. |

## Công cụ sửa đổi Access
Cách sử dụng công cộng Công cụ sửa đổi công khai cho phép bất kỳ phần nào của chương trình trong cùng một hợp ngữ hoặc một hợp ngữ khác có thể truy cập vào kiểu và các thành viên của nó. private Công cụ sửa đổi Private hạn chế các phần khác của chương trình truy cập vào kiểu và các thành viên của nó. Chỉ mã trong cùng một lớp hoặc cấu trúc mới có thể truy cập nó. nội bộ Công cụ sửa đổi nội bộ cho phép mã chương trình khác trong cùng một hội đồng truy cập vào kiểu hoặc các thành viên của nó. Đây là công cụ sửa đổi quyền truy cập mặc định nếu không có công cụ sửa đổi nào được chỉ định. được bảo vệ Công cụ sửa đổi được bảo vệ cho phép các mã trong cùng một lớp hoặc một lớp dẫn xuất từ ​​lớp đó truy cập vào kiểu hoặc các thành viên của nó. Từ khóa câu lệnh Các từ khóa câu lệnh có liên quan đến luồng chương trình.

Tuyên bố Từ khóa nếu khác chuyển trường hợp làm cho foreach in while break continue mặc định goto trả lại lợi nhuận ném thử bắt cuối cùng đã kiểm tra khóa cố định không được kiểm tra Phương pháp Tham số Từ khóa Những từ khóa này được áp dụng cho các tham số của một phương pháp.

Tham số phương pháp Từ khóa tham số tham chiếu Từ khóa không gian tên Những từ khóa này được áp dụng với không gian tên và các toán tử liên quan.

Từ khóa không gian tên bằng cách sử dụng. operator :: operator extern alias QUẢNG CÁO Từ khóa Toán tử Từ khóa toán tử thực hiện các hành động khác.

Toán tử Từ khóa như đang chờ đợi là sizeof typeof stackalloc mới được kiểm tra đã bỏ chọn Từ khóa Access Từ khóa Access được sử dụng để truy cập lớp chứa hoặc lớp cơ sở của một đối tượng hoặc lớp.

Các từ khóa Access dựa trên các Từ khóa Nghĩa đen này Các từ khóa theo nghĩa đen áp dụng cho trường hợp hoặc giá trị hiện tại của một đối tượng.

Từ khóa theo nghĩa đen null false true value void Loại Từ khóa Loại từ khóa được sử dụng cho các kiểu dữ liệu.

Nhập từ khóa bool byte char class decimal double enum float int long sbyte short string struct uint ulong ushort QUẢNG CÁO Từ khóa theo ngữ cảnh Từ khóa theo ngữ cảnh được coi là từ khóa, chỉ khi được sử dụng trong ngữ cảnh cụ thể. Chúng không được bảo lưu và vì vậy có thể được sử dụng làm tên hoặc định danh.

Từ khóa theo ngữ cảnh thêm giá trị đặt toàn cục động var Từ khóa theo ngữ cảnh không được chuyển đổi thành màu xanh lam (màu mặc định cho từ khóa trong visual studio) khi được sử dụng làm mã nhận dạng trong Visual Studio. Ví dụ, var trong hình dưới đây không có màu xanh lam, trong khi màu của nó là màu xanh lam. Vì vậy, var là một từ khóa theo ngữ cảnh.

Màu từ khóa C# trong Visual Studio Từ khóa truy vấn C# Từ khóa truy vấn Từ khóa truy vấn là từ khóa theo ngữ cảnh được sử dụng trong truy vấn LINQ.

Truy vấn Từ khóa từ nơi chọn nhóm thành thứ tự theo thứ tự tham gia cho bằng bằng cách tăng dần giảm dần Như đã đề cập ở trên, một từ khóa không thể được sử dụng làm định danh (tên của biến, lớp, giao diện, v.v.). Tuy nhiên, chúng có thể được sử dụng với tiền tố '@'. Ví dụ, lớp là một từ khóa dành riêng, vì vậy nó không thể được sử dụng như một định danh, nhưng @class có thể được sử dụng như hình dưới đây.