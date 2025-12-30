# Best-Practice

## Style Guides

| **语言**       | **权威指南**           | **核心特点**                                           |
| -------------- | ---------------------- | ------------------------------------------------------ |
| **Python**     | **PEP 8**              | 官方标准，强调可读性（如使用 4 个空格，类名大驼峰）。  |
| **JavaScript** | **Airbnb Style Guide** | 极其流行，对 ES6+ 特性有非常细致的规定。               |
| **Java**       | **Google Java Style**  | 谷歌内部标准，被全球许多大型互联网公司效仿。           |
| **C++**        | **Google C++ Style**   | 针对复杂特性（如多重继承、异常）提供了严格的限制建议。 |
| **Go**         | **Effective Go**       | 强调 Go 语言特有的“惯用法”（Idiomatic Go）。           |


## Security Guidelines

- OWASP Top 10: 针对 Web 开发的最权威指南，列出了十大最严重的漏洞（如 SQL 注入、跨站脚本 XSS）。

- SEI CERT Coding Standard: 针对 C、C++、Java 等语言的高安全性标准，常用于航空航天、医疗等对安全极度敏感的项目。

- Google Secure Coding Guidelines: 侧重于在工程实践中如何通过库和框架的设计来预防安全风险。

## API Design Guidelines

- Microsoft REST API Guidelines: 被公认为设计企业级 RESTful API 的“金标准”。

- Google API Design Guide: 详细介绍了基于 gRPC 和 REST 的网络 API 设计哲学。

- PayPal API Style Guide: 非常实用的接口命名和版本管理参考。

## 架构与设计原则指南

- SOLID 原则: 解决软件可维护性的五大核心对象设计原则。

- 云原生 12 因素 (The Twelve-Factor App): 构建 SaaS（软件即服务）应用的 12 条方法论，涉及配置管理、状态存储、并发等方面。

- Clean Architecture (整洁架构): 由 Robert C. Martin 提出，核心思想是业务逻辑应与框架、数据库等底层细节解耦。

## 工程流程与协作指南


- Conventional Commits (约定式提交): 规定了 Git 提交信息的格式（如 feat: add login, fix: handle null pointer），方便自动化生成版本记录。

- Google Code Review Guide: 详细说明了作为 Reviewer（评审者）和 Author（作者）应该如何沟通，是目前最好的代码评审指南。

- GitHub Flow / Git Flow: 关于分支管理（Branching Strategy）的实践，决定了团队如何进行功能开发、测试和发布。

## 总结 

不重复造轮子： 选一个成熟的（如 Google 或 Airbnb），根据团队情况做微调。

强制执行（自动化）：

使用 Linter（如 ESLint, Pylint）在保存代码时自动纠正风格。

使用 Prettier 进行全自动格式化。

在 CI/CD 流程中加入静态代码检查。