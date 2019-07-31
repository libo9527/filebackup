## MySql

### 安装

> [mysql 8.0.11 macos10.13安装配置方法图文教程](<http://www.manongjc.com/article/4358.html>)
>
> 注意：关于环境变量配置的部分，一般 Mac 下 `.bash_profile` 文件放在用户目录下，即 `~` 目录下。

#### Navicat连接数据库MySQL报错2059

原因：mysql8 之前的版本中加密规则是 mysql_native_password，而在 mysql8 之后，加密规则是 caching_sha2_password。

解决方法：

1. 第一种是升级 navicat 驱动

2. 第二种是把mysql用户登录密码加密规则还原成 mysql_native_password

   ```mysql
   ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
   -- password 是你要设置的密码
   ```


### 查看版本

```mysql
mysql -V
```

