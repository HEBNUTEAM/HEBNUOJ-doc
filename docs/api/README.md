### 网站API接口文档

### 1.1 Register


##### 简要描述

- 用户注册接口

##### 请求URL
- ` http://xx.com/api/auth/register `
##### 请求方式
- POST 

##### 参数

|参数名|必选|类型|说明|
|-----    |:---|:----- |-----   |
| nickname |Y  |string | 昵称 |
| email |Y  |string | 邮箱  |
| verification | N    | string | 邮箱验证码 |
| pwd1         | Y    | string | 密码       |
| pwd2         | Y    | string | 密码       |

##### 返回示例 

``` 
{
    "code": 200,
    "data": null,
    "msg": "注册成功"
}
```

##### 返回参数说明 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
| code   |int   |状态码  |
| msg    |string |信息提示 |

##### 备注 

- 错误代码请看具体api实现的错误代码描述




