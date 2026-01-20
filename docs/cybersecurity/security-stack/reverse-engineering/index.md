# Reverse-Enginneering


## Resources

- [Reverse Engineering Resources](https://github.com/wtsxDev/reverse-engineering)

## Books

- RE4B | [CN/EPUB]({{ files_server }}/cybersecurity/reverse-engineering/RE4B/RE4B-CN.epub)
 | [CN/PDF]({{ files_server }}/cybersecurity/reverse-engineering/RE4B/RE4B-CN.pdf)
 | [EN/PDF]({{ files_server }}/cybersecurity/reverse-engineering/RE4B/RE4B-EN.pdf)
- 软件调试的艺术 | [CN/EPUB]({{ files_server }}/cybersecurity/reverse-engineering/current/%E8%BD%AF%E4%BB%B6%E8%B0%83%E8%AF%95%E7%9A%84%E8%89%BA%E6%9C%AF.epub)
 | [CN/PDF]({{ files_server }}/cybersecurity/reverse-engineering/current/%E8%BD%AF%E4%BB%B6%E8%B0%83%E8%AF%95%E7%9A%84%E8%89%BA%E6%9C%AF.pdf)
| [EN/PDF]({{ files_server }}/cybersecurity/reverse-engineering/current/The%20Art%20of%20Software%20Security%20Assessment.pdf)


## Use-Cases

### Security & Defense

这是目前逆向工程最主流的应用领域：

- **Malware Analysis：** 安全分析师需要逆向勒索软件、病毒或木马的二进制样本，分析其行为逻辑（如何传播、连接哪个C2服务器），以便编写查杀签名或解密工具。
  
- **Binary Analysis (Vulnerability Research)：** 在没有源代码的情况下（如闭源的Windows组件或固件），研究人员通过逆向分析寻找缓冲区溢出、逻辑错误等“零日漏洞”（0-day），既可以是黑客寻找攻击路径（如OSCP/OSEP涉及的内容），也可以是厂商进行安全审计。
  
- **Digital Forensics：** 在黑客入侵后，取证人员需要逆向分析被篡改的系统文件或攻击者留下的未知工具，以还原攻击链路。
  

### Interoperability

当你想让自己的软件或硬件与第三方系统配合工作，但对方没有提供文档或API时，逆向是唯一的出路：

- **驱动开发：** Linux社区经常通过逆向闭源的Windows驱动（如NVIDIA显卡驱动或无线网卡驱动），来编写开源的替代驱动（如Nouveau项目）。
  
- **协议分析：** 通过抓包和分析二进制客户端，推导出私有网络协议的通信格式。例如，第三方即时通讯客户端（如早期的Pidgin支持QQ/MSN）通常就是这样实现的。
  
- **未公开API调用：** 操作系统内部有很多未文档化的API（Undocumented APIs），为了实现某些底层功能（如系统监控工具），开发者需要通过逆向内核来找到这些接口。
  

### Legacy System Maintenance

这种情况在工业控制和老旧企业环境中非常常见：

- **源代码丢失：** 很多运行了几十年的关键软件（如银行核心、工控上位机），其原始开发商可能倒闭了，源代码也丢了。如果不进行逆向分析，就无法修复Bug或迁移到新平台。
  
- **系统移植：** 将基于旧架构（如PowerPC, MIPS）编写的软件移植到现代架构（x86_64, ARM64）上，可能需要先理解其底层的汇编逻辑。
  

### Competitive Analysis & Audit

- **竞品分析：** 公司分析竞争对手的产品，了解其核心算法、性能优化手段或具体实现逻辑（在法律允许的范围内）。
  
- **专利侵权验证：** 律师和技术专家通过逆向分析某款产品，来判断它是否使用了受专利保护的技术或代码。
  
- **审计与合规：** 验证购买的闭源软件是否包含后门，或者确认其加密算法是否如宣传那样安全。
  

### Hardware Reverse Engineering

- **PCB 抄板与复刻：** 通过通过去层拍摄、X光扫描等手段分析多层电路板的布线，还原原理图。
  
- **芯片级分析：** 使用电子显微镜观察芯片内部的晶体管布局（Decapping），以提取固件或破解硬件加密密钥。
  
### Education & Research

- **深入理解原理：** 对于想深入理解操作系统内核（如Windows/Linux内核机制）或编译器优化原理的开发者，直接看汇编代码是了解“机器到底在做什么”的最直接方式。