
## Projects

### Identity Server

> 认证服务。<br/>
> 支持使用用户名+密码、电子邮件+验证码、第三方认证等。<br/>
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

响应结果

```json
{
  "accessToken": "Token内容",
  "refreshToken": "刷新Token",
  "tokenType": "Bearer",
  "expiresIn": 1000, /*过期时间*/
  "issuedAt": 1000, /*令牌颁发时间*/
  "userId": "用户ID",
  "username": "用户名"
}
```

### Registry Server

### Account Server

### Finance Server

### Message Server

> 消息服务，用于发送短信、邮件及微信推送消息等。
> 基于Java Spring Boot开发，数据库采用MySql。
