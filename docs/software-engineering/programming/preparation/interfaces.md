# Interfaces

软件系统的交互接口（Interface）是用户、开发者或其他系统与程序进行沟通与操作的方式。在软件工程领域，常见的交互接口主要包括 **API、CLI、GUI** 三类。它们分别面向不同的使用场景，提供不同层次的控制方式和易用性。

------

## API
> API（Application Programming Interface）是一种面向程序之间或模块之间的交互接口。  
它允许其他程序、模块或函数以结构化的方式访问系统功能，而无需了解内部实现细节。

API 可以分为：

- **本地函数调用**：同一程序或模块内部的函数、类方法或模块接口调用。例如一个库提供的函数调用。  
- **远程调用**：跨进程或跨网络的调用，如 REST API、GraphQL、gRPC、WebSocket 等。

API 的典型特征包括：

- **面向程序**：由其他程序或模块调用，而非直接供人操作。  
- **标准化接口**：定义明确的输入、输出和行为契约。  
- **抽象内部逻辑**：调用者只需关注输入和输出，而无需了解实现细节。  

API 适合用于：

- 模块化应用开发
- 程序内部功能调用
- 系统之间的集成
- 脚本自动化与服务扩展

------

## CLI

> CLI（Command Line Interface）是通过文本命令与系统交互的方式，常用于开发、运维和自动化场景。

CLI 的典型特征包括：

- **高控制力**：支持参数化操作、批处理、流水线等。  
- **轻量且高效**：无需图形界面即可运行，适合远程服务器。 
- **可脚本化**：可通过 Shell 脚本实现自动化任务。  
- **更贴近底层功能**：常暴露较多系统级控制能力。

CLI 适合用于：

- 系统管理与部署
- 开发调试
- 批处理任务与自动化流程
- 资源受限或无图形界面的环境


```shell
CLI Environmental Development History:

Teletypewriter > Video Terminal > Terminal Emulator
```

- [Linux TTY/PTS概述](https://segmentfault.com/a/1190000009082089)
- [The TTY demystified](https://www.linusakesson.net/programming/tty/)
- [解密TTY](https://www.cnblogs.com/liqiuhao/p/9031803.html)
- [Linux 终端(TTY)](https://www.cnblogs.com/sparkdev/p/11460821.html)
- [Linux 伪终端(pty)](https://www.cnblogs.com/sparkdev/p/11605804.html)
- [Windows Pseudo Console (ConPTY)](https://learn.microsoft.com/zh-cn/windows/console/creating-a-pseudoconsole-session)

------

## GUI

> GUI（Graphical User Interface）是使用窗口、按钮、图标等可视化元素进行交互的图形界面，是最常见的面向最终用户的接口形式。

GUI 的典型特征包括：

- **易学易用**：视觉化的操作方式更直观。  
- **用户体验友好**：支持布局、图形、动画、交互反馈等。  
- **面向广泛用户群体**：无需专业技术背景即可操作。  
- **较高的构建成本**：需要额外的设计、前端开发与 UI 测试。

GUI 适合用于：

- 桌面应用程序
- 移动应用
- Web 前端界面
- 强调用户体验的系统

---

## Config Files

- JSON
- YAML

## DSL

- SQL
- Shell

这三类接口共同构成软件系统的人机交互与程序集成方式。具体系统可根据需求选择其中一种或多种交互接口，以平衡易用性、性能、扩展性和开发成本。