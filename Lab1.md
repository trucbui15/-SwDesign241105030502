# LAB 1: Phân tích kiến trúc, cơ chế, ca sử dụng cho hệ thống "Payroll System"

## 1. Phân tích kiến trúc

### Kiến trúc đề xuất: Kiến trúc 3 lớp (Three-Tier Architecture)

#### a. Các thành phần trong kiến trúc:

1. **Presentation Layer (Lớp giao diện người dùng)**
   - **Mô tả:** Là lớp mà người dùng tương tác với hệ thống. Nó cung cấp giao diện để nhập dữ liệu và hiển thị kết quả.
   - **Ý nghĩa:** Tách biệt giao diện người dùng với các logic nghiệp vụ giúp dễ dàng bảo trì và nâng cấp.

2. **Business Logic Layer (Lớp logic nghiệp vụ)**
   - **Mô tả:** Chứa các quy tắc và logic để xử lý dữ liệu, bao gồm tính toán lương, xử lý phúc lợi, và quản lý thông tin nhân viên.
   - **Ý nghĩa:** Tăng cường khả năng tái sử dụng mã và đảm bảo rằng các quy tắc nghiệp vụ được thực thi nhất quán.

3. **Data Access Layer (Lớp truy cập dữ liệu)**
   - **Mô tả:** Đảm bảo các yêu cầu về lưu trữ và truy xuất dữ liệu từ cơ sở dữ liệu. Thực hiện các thao tác CRUD (Create, Read, Update, Delete) cho dữ liệu liên quan đến nhân viên và lương.
   - **Ý nghĩa:** Tách biệt việc quản lý dữ liệu khỏi logic ứng dụng, giúp dễ dàng thay đổi cơ sở dữ liệu mà không ảnh hưởng đến các lớp khác.

#### b. Giải thích lý do lựa chọn:

- **Tính linh hoạt:** Kiến trúc 3 lớp cho phép thay đổi từng thành phần mà không ảnh hưởng đến các thành phần khác.
- **Khả năng mở rộng:** Hệ thống dễ dàng mở rộng để đáp ứng nhu cầu tăng trưởng trong tương lai.
- **Bảo trì:** Dễ dàng bảo trì và phát triển thêm các tính năng mới do có sự phân tách rõ ràng giữa các thành phần.

## 2. Biểu Đồ Package



### Biểu đồ package mô tả kiến trúc:
vẽ sau
