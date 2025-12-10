# Security Skills
> From binary to source code, from binary to protocol

### Analysis Matrix

| **目标** | **黑盒分析 (无源码)** | **灰盒分析 (有二进制)** | **白盒分析 (有源码)** |
|---|---|---|---|
| **Static** | 无法进行。 | **逆向工程**（分析二进制文件结构、反汇编）。 | **代码审计**（人工或工具扫描源代码）。 |
| **Dynamic** | **网络渗透测试/Fuzzing**（盲目输入，观察网络响应）。 | **调试和监控**（运行二进制文件，观察内存/行为）。 | **动态应用安全测试 (DAST)**（运行源代码，观察运行时行为）。 |
| **Hybrid** | 几乎不可能。 | **混合逆向工程**（动态调试脱壳后，静态分析转储的代码）。 | **污点分析**（Taint Analysis，同时追踪源代码中的数据流和运行时执行路径）。 |


### Core

- Obfuscations Confrontation
- Code Review
- Software Reverse Engineering
- Network Traffic Analysis
- Dynamic/Staic/Hybrid Analysis

### Practiac

- Behavioral Analysis
- Vulnerability Analysis
- Malware Analysis
- Secure-Development
  - DevSecOps