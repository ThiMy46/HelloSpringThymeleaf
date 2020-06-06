# HelloSpringThymeleaf

Tạo một project sử dụng Spring MVC và Thymeleaf (Template engine)

Config như cũ và thay đổi viewResolver mặc định(.jsp) sang khai báo SpringTemplateEngine (.html)

Để sử dụng Thymeleaf trong Spring MVC

1. templateResolver(SpringResourceTemplateResolver) cấu hình location của các tập tin template(prefix & suffix(.html))

2. templateEngine(SpringTemplateEngine) sử dụng đối tượng templateResolver

3. Đối tượng SpringTemplateEngine này sẽ giúp chúng ta khai báo ViewResolver của Thymeleaf với Spring

thông qua ThymeleafViewResolver sẽ sử dụng đối tượng templateEngine trên

==> SpringResourceTemplateResolver(khai báo đường dẫn) - SpringTemplateEngine(template) - ThymeleafViewResolver(View)

