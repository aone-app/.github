## About

> A.one是一个先进的智能化互联网应用，旨在优化用户在书签、笔记、订阅、任务等方面的组织、共享与管理流程。
使用A.one可以显著提升了团队知识的整合与共享能力，促进了协作效率。

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

> 一个用 **Golang** 实现的轻量级 **注册中心**，同时支持 **HTTP** 和 **ConnectRPC** 调用。  
> 提供了 **Go / C# / Java** 三个版本的 SDK，方便跨语言的服务注册、心跳和服务发现。

#### ✨ Features | 功能特点

- ✅ Service register (注册服务)  
- ✅ Service deregister (注销服务)  
- ✅ Heartbeat to keep alive (心跳保活)  
- ✅ Query registered services (查询服务列表)  
- ✅ SDKs for Go / C# / Java (跨语言 SDK)  


### Account Server

### Finance Server

### Message Server

> 消息服务，用于发送短信、邮件及微信推送消息等。
> 基于Java Spring Boot开发，数据库采用MySql。
