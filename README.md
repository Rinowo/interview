1. Vòng đời của bean
- IOC container sử dụng constructor hoặc factory method để tạo ra bean
- Các thuộc tính của bean sẽ được inject giá trị vào các bean khác trong container
- Sau khi các thuộc tính được inject thì các method được gọi để cấu hình bean
- Bean sẵn sàng được sử dụng bởi các thành phần khác
- Sau khi bean không còn cần thiết thì container sẽ gọi @Predestroy trước khi bean bị hủy
