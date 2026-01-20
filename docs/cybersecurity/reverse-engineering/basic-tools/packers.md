# Packers

### 1. 查壳工具 (Detectors / Identifiers)

在脱壳之前，首先需要识别程序加了什么壳。

- **Detect It Easy (DiE):** 目前最推荐的查壳工具。开源、特征库更新快，能识别各种编译器、链接器和壳，支持脚本编写。
  
- **PEiD:** 虽然是经典老牌工具，但早已停止维护，对现代壳的识别率较低（常作为备用）。
  
- **Exeinfo PE:** 类似于 PEiD，但更新更频繁，识别率较高，通常会给出脱壳建议。
  

### 2. 常见的 Packers (加壳器)

加壳器通常分为“压缩壳”和“加密/保护壳”两类。

#### **A. 压缩壳 (Compression Packers)**

这类壳主要为了减小体积，解压逻辑相对简单。

- **UPX (Ultimate Packer for eXecutables):** 最著名的压缩壳。开源、跨平台。
  
  - *特点:* 几乎所有逆向工程师的“入门壳”。
- **ASPack:** 经典的压缩壳，比 UPX 稍微复杂一点，但原理类似。
  

#### **B. 加密与虚拟化壳 (Protectors / Virtualizers)**

这类壳通过反调试、代码虚拟化（Virtualization）、混淆（Obfuscation）来对抗逆向。

- **VMProtect (VMP):** 业界标杆。它将 x86 指令转换为自定义的虚拟指令集，并在其私有虚拟机中运行。
  
  - *特点:* 极难还原代码逻辑，通常只能分析其行为。
- **Themida / WinLicense (by Oreans):** 拥有极强的反调试和反 dump 机制，代码混淆非常复杂（如 Code Morphing）。
  
- **Enigma Protector:** 提供强大的许可管理和反逆向功能。
  
- **Vullup / MPRESS:** 常见的恶意软件或小型软件使用的壳。