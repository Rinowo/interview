## 1. IOC container tạo ra bean, quản lý bean bằng DI.

## 2. Các loại bean trong spring
- Singleton là 1 bean mặc định trong spring, đảm bảo mỗi class có 1 instance và cung cấp điểm truy cập toàn cục cho instance đấy.
- Prototype là loại bean tạo ra 1 instance cho 1 lần request.
- Request là loại bean chỉ tồn tại trong 1 request và sẽ bị hủy sau khi request được xử lý xong.
- Session là loại bean tồn tại trong session của 1 user và bị hủy khi kết thúc phiên làm việc của user đấy.
- Global session là loại bean tồn tại trong xuyên suốt phiên làm việc của tất cả user và bị hủy khi toàn bộ phiên làm việc kết thúc.

## 3. Vòng đời của bean
- IOC container sử dụng constructor hoặc factory method để tạo ra bean
- Các thuộc tính của bean sẽ được inject giá trị vào các bean khác trong container
- Sau khi các thuộc tính được inject thì các method được gọi để cấu hình bean
- Bean sẵn sàng được sử dụng bởi các thành phần khác
- Sau khi bean không còn cần thiết thì container sẽ gọi @Predestroy trước khi bean bị hủy
##
### 4. DI là inject đối tượng này vào đối tượng cần.


## 5. Hibernate là công nghệ ORM giúp mapping object với bảng trong db
- Dev có thể dựa trên object để làm việc với db
- Hibernate có HQL tức là có thể thay đổi db mà không phải sửa truy vấn bởi vì hibernate có thể tự thay đổi truy vấn cho phù hợp với db được sử dụng
- Nhược điểm của hibernate là những câu truy vấn không được tối ưu vì được tạo ra tự động

## 6. Các Annotation phổ biến trong spring
- @Component đánh dấu class là 1 bean thông thường, không thuộc loại nào cả
- @Service đánh dấu class chứa business logic
- @Repository Đánh dấu interface chứa DAO, giao tiếp với DB
- @Controller Đánh dấu class là 1 Spring MVC Controller, xử lý HTTP Request từ Client
- @RestController Đánh dấu class là 1 Restful Controller, xử lý Restful HTTP Request từ Client. Dữ liệu được trả về dưới định dạng xml hoặc json
- @Configuration Đánh dấu class là 1 class cấu hình, sử dụng method để cấu hình
- @Entity đánh dấu class là 1 entity
- @Autowired đánh dấu để spring tự động gán giá trị vào phương thức, thuộc tính hoặc là constructor của bean
##
### 7. Native Query là dev có thể tự viết query để tối ưu và tinh chỉnh query đó
- Ưu điểm của native query là có thể tinh chỉnh hiệu năng của query
- Nhược điểm của native query là nó dễ tạo ra lỗ hổng bảo mật
