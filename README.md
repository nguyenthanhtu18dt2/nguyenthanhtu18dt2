POITER AND REFERENCE
1.	Poiter
-	Con trỏ là biến dùng để lưu trữ địa chỉ bộ nhớ của biến khác (or function) 
a)	Con trỏ và mảng
-	Address: Địa chỉ của mảng là địa chỉ phần tử đầu tiên trong mảng
-	Poiter Arithmetic: Sử dụng con trỏ để truy cập vào các phần tử trong mảng *(arr + i) = arr[i]
-	Decay (phân rã): Có thể truyền mảng vào hàm dưới dạng con trỏ hoặc ngược lại
-	Size: Kích thước mảng là cố định, sử dụng con trỏ để phân bổ động 	
2.	Reference
-	Tham chiếu là bí danh cho biến hiện tại, nó dùng cùng địa chỉ bộ nhớ. KHÔNG có tham chiếu NULL, PHẢI khởi tạo ngay khi khai báo
MEMORY MODEL IN C++
1.	Stack Memory
-	Lưu trữ các local variable and function call data. Nó phân bổ và hủy phân bổ tự động. Nó là LIFO
2.	Heap Memory
-	Dùng để lưu trữ các dynamic variables. 
3.	Data Segment
-	Có hai loại: initialized data segment and uninitialized data segment
o	Initialized data segment: lưu trữ biến global, static, constant variables
o	Uninitialized data segment: lưu trữ biến global, static variables.
4.	Code Segment
-	Lưu trữ excutable code 
STRUCT AND CLASSES
	STRUCT	CLASS
GIỐNG	-	Both are container types, meaning that they contain other types as members.
-	Both have members, which can include constructors, methods, properties, fields, constants, enumerations, events, and event handlers.
-	Members of both can have individualized access levels. For example, one member can be declared Public and another Private.
-	Both can implement interfaces.
-	Both can have shared constructors, with or without parameters.
-	Both can expose a default property, provided that property takes at least one parameter.
-	Both can declare and raise events, and both can declare delegates.

KHÁC	-	Value types 
-	Stack allocation
-	Elements of struct is public
-	Struct are not inheritance
-	Struct does not require constructor	-	Reference type
-	Heap allocation
-	Elements of class is private
-	Class use to inheritance
-	Class require constructor

OOP (OBJECT-ORIENTED PROGRAMMING)
-	OOP là mô hình lập trình sử dụng các object để thực hiện các tương tác với nhau
1.	Classes
-	Struct (data member)
-	Behavior (function member)
2.	Encapsulation
-	Nó dùng để ẩn các thông tin bên trong một class
3.	Inheritance
-	Tạo ra lớp mới từ lớp đã có. Cho phép tái sử dụng code từ lớp base
4.	Polymorphism
-	Tính đa hình cho phép sử dụng một interface duy nhất để thể hiện các các loại khác. Trong C++ thường sử dụng overloading, overiding and function virutal
OVERLOADING FUNCTIONS
-	Nạp chồng toán tử là một loại static polymorphism có nhiều hàm cùng tên nhưng khác tham số.
1.	Static Polymorphism
-	Static Polymorphism có được trong thời gian compile-time khi sử dụng function overloading and templates
2.	Dynamic Polymorphism
-	Dynamic Polymorphism có được khi sử dụng virtual function
a)	Virtual Methods
-	Cho phép subclass method override lên method của baseclass
b)	Virtual Tables
-	Là một cấu trúc dữ liệu lưu giữ địa chỉ của các virtual methods
EXCEPTION HANDLING
-	Try, Catch, Throw
1.	Access Violation (Truy cập bất hợp pháp)
-	Dereferencing null or invalid pointer
-	Accessing Array out of bounds
-	Reading or writing to freed memory
LANGUAGE CONCEPT IN C++
-	Variables and Data Types: int, float, double, char, bool ….
-	Control Structures:
o	Conditional Statement: if, else, and else if
o	Loop: for, while, do-while
o	Switch-case
-	Function
-	Arrays and Vectors
-	Pointer
-	Structures and Classes
-	Inheritance and Polymorphism
-	Exception Handling
1.	Auto (Automatic Type Deduction)
2.	Type Casting
a.	Static_cast: convert giữa các lại dữ liệu khác nhau như int, float, hoặc giữa các dữ liệu kiểu poniter
b.	Dynamic_cast: dùng cho polymorphism. Dùng để convert pointer, reference của base class sang derived class
c.	Const_cast: cho phép remove hoặc add thêm hằng vào biến
d.	Reinterpret_cast: cho phép thay đổi pointer hoặc integer mà không thay đổi cách biểu diễn dữ liệu
3.	Macros
-	Macros là preprocess. Sử dụng từ khóa #define. Macros sử dụng để định nghĩa constant, function-like macros, conditional compilation #ifdef, #ifndef, #if, #elif, #endif 
C++ STANDARD TEMPLATE LIBRARY (STL)
-	Container: có 4 loại: sequence container, associative container, unordered associative container, container adaptors
-	Vector: là mảng động có thể thay đổi kích thước
 
-	List: là danh sách liên kết đôi cho phép các chèn, xóa phần tử bất kỳ vị trí nào trong constant time. Không hỗ trợ random access.
 
-	Map: lưu trữ theo kiểu key-value. Trích xuất value dựa vào key. Key được sắp xếp theo thứ tứ tăng dần
 
INTERATORS
-	Là một object trong STL giúp duyệt qua các container như array, list, vector. Bridge giữa container class và algorithms.
-	Các loại interators:
1.	Input interators: sử dụng để đọc các elements trong container chỉ một lần. Không thể modify elements
2.	Output interators: Write once only. Can’t modify elements
3.	Forward interators: multiple elements in a container. Không thể move backward (lùi lại)
4.	Reverse interators: multiple elemements. Không thể move forward
STL ALGORITHMS
-	Sorting:  std::sort();
 
-	Searching: std::find()
 
-	Modifying Sequences
 
 
MULTITHREADING IN C++	

