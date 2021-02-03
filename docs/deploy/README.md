### 临时部署方案

因为在开发中，暂时不适用脚本和docker自动化部署，下面是替代方案：

1. 安装mysql 5.7版本和golang1.15版本
2. 输入`go mod download`下载项目需要的所有依赖文件
3. 打开项目下的config/application.yml文件进行数据库配置，更改以下注释内容即可
```
datasource:
  driverName: mysql
  host: 127.0.0.1 
  port: 3306
  database: ginnessential //数据库名称，需要在本地提前创建好
  username: root // 数据库用户名
  password: xxxx // 数据库密码
  charset: utf8
```
4. 运行目录下的main.go文件

5. 使用postman对其进行post请求的测试