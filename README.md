# RESTful服务最佳实践

## 书名
- RESTful服务最佳实践：创建Web服务时的一些建议

## 版本
- 1.2.1

## 关于作者
- [Todd Fredrich的Github](https://github.com/tfredrich)
- [Todd Fredrich的个人网站](http://toddfredrich.com)

## 原始资源
- [在线版本](https://www.restapitutorial.com)
- [电子书](https://github.com/heshengbang/RESTful-Service-Best-Practices/raw/master/original_version/RESTful%20Best%20Practices-v1_2_1.pdf)

## 目录
- 历史版本
- 谁应当阅读这本书
- 介绍
- 什么是REST?
	- 接口统一
		- 基于资源
		- 通过资源的表示来操作资源
		- 自描述性消息
		- 超媒体作为应用程序状态引擎（HATEOAS）
	- 无状态
	- 可缓存
	- 客户端-服务器模式
	- 系统分层
	- 按需编程（可选）
- REST 快速入门提示
	- 使用HTTP的动词来表示某事
	- 资源名应具备良好的可读性
	- XML和JSON
	- 创建细粒度的资源
	- 基于连通性的考虑
- 定义
	- 幂等
	- 安全
- HTTP的动词
	- GET
	- PUT
	- POST
	- 创建时使用PUT vs POST？
	- DELETE
- 资源命名
	- 资源URI示例
	- 资源命名反模式
	- 多元化
- Returning Representation
	- 通过链接发现资源（HATEOAS续）
		- 最小连接建议
		- 链接格式
	- 被包装的response
	- 处理跨域问题
		- 支持CORS
		- 支持JSONP
- 查询、过滤和分页
	- 限制结果
		- 通过Header中的Range参数限制
		- 通过查询字符串参数限制
		- 基于Range的response
	- 分页
	- 对结果过滤和排序
		- 过滤
		- 排序
- 服务的版本控制
	- 通过内容协商支持版本控制
		- 没有版本被指定时返回什么版本信息？
		- 不支持的版本被请求
	- 什么时候应该创建一个新版本
		- 会改变协商约定的变更
		- 变更被视为不间断
	- 应该在什么级别进行版本控制？
	- 使用Content-Location去提升response
	- 与Content-Type的连接
	- 找出支持的版本
		- 一次应该支持多少个版本？
		- 弃用
		- 如何通知client已经弃用的资源？
- 日期/时间处理
	- Body Content中日期/时间的序列化
	- HTTP Headers中日期/时间的序列化
- 安全服务
	- 认证
	- 传输安全
	- 授权
	- 应用安全性
- 缓存与可扩展性
	- 关于ETag Header
- HTTP 状态码(Top 10)
- 其他的资源
	- 书籍
	- 站点




# RESTful Service Best Practices

## Book Name
- RESTful Service Best Practices: Recommendations for Creating Web Services

## Version
- 1.2.1

## About Author
- [Todd Fredrich's Github](https://github.com/tfredrich)
- [Todd Fredrich's website](http://toddfredrich.com)

## Original Resource
- [online](https://www.restapitutorial.com)
- [eBook](https://github.com/heshengbang/RESTful-Service-Best-Practices/raw/master/original_version/RESTful%20Best%20Practices-v1_2_1.pdf)

## Table of Contents
- Document History
- Who Should Read This Document
- Introduction
- What is REST?
	- Uniform Interface
		- Resource-Based
		- Manipulation of Resources Through Representations
		- Self-descriptive Messages
		- Hypermedia as the Engine of Application State(HATEOAS)
	- Stateless
	- Cacheable
	- Client-server
	- Layered system
	- Code on demand(optional)
- REST Quick Tips
	- Use HTTP Verbs to Mean Something
	- Sensible Resource Names
	- XML and JSON
	- Create Fine0Grained Resources
	- Consider Connectedness
- Definitions
	- Idempotence
	- Safety
- HTTP Verbs
	- GET
	- PUT
	- POST
	- PUT vs POST for Creation
	- DELETE
- Resource Naming
	- Resource URI Example
	- Resource Naming Anti-Patterns
	- Pluralization
- Returning Representation
	- Resource Discoverability Through Links(HATEOAS cont'd)
		- Minimal Linking Recommendations
		- Link Format
	- Wrapped Responses
	- Handling Cross-Domain Issues
		- Supporting CORS
		- Supporting JSONP
- Querying,Filtering and Pagination
	- Limiting Results
		- Limiting via the Range Header
		- Limiting via Query-String Parameters
		- Range-Based Responses
	- Pagination
	- Filtering and Sorting Results
		- Filtering
		- Sorting
- Service Versioning
	- Support Versioning via Content Negotiation
		- what version is returned when no version is specified?
		- Unsupported Versions Requested
	- When Should I Create a New Version?
		- Changes that will break contracts
		- Changes considered non-breaking
	- At What Level Should Versioning Occur?
	- Use Content-Location to Enhance Responses
	- Links with Content-Type
	- Finding Out What Versions are Supported
		- How many versions should I support at once?
		- Deprecated
		- How do I inform clients about deprecated resources?
- Date/Time Handling
	- Date/Time Serialization In Body Content
	- Date/Time Serialization In HTTP Headers
- Securing Services
	- Authentication
	- Transport Security
	- Authorization
	- Application Security
- Caching and Scalability
	- The ETag Header
- HTTP Status Code(Top 10)
- Additional Resources
	- Books
	- Websites