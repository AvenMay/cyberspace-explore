# Desgin Patterns

## Books

- [大话设计模式 EPUB]({{ files_server }}/software-engineering/programming/design-patterns/大话设计模式.epub)
- [设计模式-可复用面向对象软件的基础 PDF]({{ files_server }}/software-engineering/programming/design-patterns/设计模式-可复用面向对象软件的基础.pdf)
- [面向对象分析与设计 PDF]({{ files_server }}/software-engineering/programming/design-patterns/面向对象分析与设计.pdf)


## Programming Paradigm

- 过程式（Imperative/Procedural）
- 面向对象（OOP）
- 函数式（Functional）
- 逻辑/声明式（Declarative/Logic）
- 事件驱动（Event-Driven）
- 并发/Actor 式（Concurrent/Actor）
- 数据流/反应式（Dataflow/Reactive）

## OOP

### 1. 企业级应用是 OOP 的主战场

- **典型语言/技术栈**：Java、C#、Python（面向对象风格）、Spring、.NET
  
- **典型场景**：ERP、CRM、金融系统、保险、电信后台
  
- **原因**：
  
  - 复杂业务建模：类和对象可以直观映射业务实体和流程
    
  - 长期维护需求：封装、多态、继承帮助代码模块化和可扩展
    
  - 团队协作：统一的 OOP 设计规范方便大型团队协作
    

---

### 2. OOP 很少出现的领域

| 领域  | 主流范式 | OOP 使用情况 |
| --- | --- | --- |
| 操作系统内核 | 过程式 + 模块化 | 几乎没有 |
| 数据库/缓存 | 过程式 + 数据驱动 | 很少  |
| 高性能服务器（Nginx、Redis） | 事件驱动/过程式 | 几乎没有 |
| 云原生/容器/编排（Docker、K8s） | 数据驱动 + 组合接口 | OOP 成分有限 |
| 前端现代框架（React/Vue） | 函数式 + 组合模式 | OOP 少数历史遗留 |
| 数据科学/AI | 函数式/脚本式 | OOP 很少 |

✅ **结论**：

- 企业级应用 → OOP 占多数
  
- 其他几乎所有领域 → OOP 占少数甚至几乎没有
  

---

### 3. 为什么 OOP 在其他领域不适用

1. **性能敏感** → OOP 的动态分派、继承、多态带来的开销不划算
  
2. **高度并发/分布式系统** → 数据驱动和组合模式更自然
  
3. **简单/短期逻辑** → 过度 OOP 会增加复杂度
  
4. **函数式风格更适合流式处理、事件驱动和 UI 组件化**