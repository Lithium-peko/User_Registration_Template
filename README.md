### 使用Servlet构建的Java Web用户注册模板

数据库文件 

`user.sql`
```mysql
-- 创建用户表
CREATE TABLE user(
    id int primary key auto_increment,
    username varchar(20) unique,
    password varchar(32) 
);

-- 添加数据
INSERT INTO user(username,password) values('zhangsan','123'),('lisi','234');

SELECT * FROM user;
```

使用mysql运行user.sql文件创建数据库

>mysql -u用户名 -p密码 < user.sql
