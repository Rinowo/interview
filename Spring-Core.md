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

5. 
