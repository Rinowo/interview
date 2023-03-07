1. IOC container tạo ra bean, quản lý bean bằng DI.

2. Vòng đời của bean
- IOC container sử dụng constructor hoặc factory method để tạo ra bean
- Các thuộc tính của bean sẽ được inject giá trị vào các bean khác trong container
- Sau khi các thuộc tính được inject thì các method được gọi để cấu hình bean
- Bean sẵn sàng được sử dụng bởi các thành phần khác
- Sau khi bean không còn cần thiết thì container sẽ gọi @Predestroy trước khi bean bị hủy

3. DI là inject đối tượng này vào đối tượng cần.

4. Hibernate là công nghệ ORM giúp mapping object với bảng trong db
- Dev có thể dựa trên object để làm việc với db
- Hibernate có HQL tức là có thể thay đổi db mà không phải sửa truy vấn bởi vì hibernate có thể tự thay đổi truy vấn cho phù hợp với db được sử dụng
- Nhược điểm của hibernate là những câu truy vấn không được tối ưu vì được tạo ra tự động

5. Các Annotation phổ biến trong spring
- @Component đánh dấu class là 1 bean thông thường, không thuộc loại nào cả
- @Service đánh dấu class chứa business logic
- @Repository Đánh dấu interface chứa DAO, giao tiếp với DB
- @Controller Đánh dấu class là 1 Spring MVC Controller, xử lý HTTP Request từ Client
- @RestController Đánh dấu class là 1 Restful Controller, xử lý Restful HTTP Request từ Client. Dữ liệu được trả về dưới định dạng xml hoặc json
- @Configuration Đánh dấu class là 1 class cấu hình, sử dụng method để cấu hình
- @Entity đánh dấu class là 1 entity
- @Autowired đánh dấu để spring tự động gán giá trị vào phương thức, thuộc tính hoặc là constructor của bean
