1 spring-data-jpa+mysql
2 添加mysql支持
    a 添加mysql-connector-java依赖
    b 修改配置文件 添加
        #spring.jpa.hibernate.ddl-auto=update
        spring.datasource.url=jdbc:mysql://localhost:3306/springBootDatabase
        spring.datasource.username=springBootUser
        spring.datasource.password=springBootUser
        spring.datasource.driver-class-name =com.mysql.jdbc.Driver
3 测试url
    浏览器
    http://localhost:8080/demo/all  #列出所有用户

    curl
        http://localhost:8080/demo/add -d name=lucia -d email=lucia@126.com #添加用户