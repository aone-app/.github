
## Projects

### Identity Server

> 认证服务。
> 基于Java Spring Boot开发，数据库采用MySql。

#### 接口列表

##### 获取Token

> 接口地址 /api/identity/token/grant

请求参数

```json
{
  "provider": "github|google|microsoft|username|email",
  "password": "密码|验证码|oauth提供商的code",
  "username": "用户名|邮箱",
  "requestId": "请求ID"
}
```

### Registry Server

### Account Server

### Finance Server

### Message Server

> 消息服务，用于发送短信、邮件及微信推送消息等。
> 基于Java Spring Boot开发，数据库采用MySql。
