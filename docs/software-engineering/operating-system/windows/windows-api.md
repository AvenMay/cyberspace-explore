# Windows API

- [Windows API List](https://learn.microsoft.com/zh-cn/windows/win32/apiindex/windows-api-list)

## Windows Programming

| **环境** | **核心技术** | **适用人群** | **哲学倾向** |
| --- | --- | --- | --- |
| **Win32 API** | C 语言接口 | 系统级开发者 | 原始、底层、性能至上 |
| **COM** | 二进制接口标准 | 组件开发者、系统架构师 | 万物皆对象、跨语言 |
| **WMI** | WQL (类 SQL 查询) | 运维、SRE | 系统状态即数据 |
| **WSH** | VBScript / JScript | 历史脚本维护者 | 简单、快速、易滥用 |
| **WinRT** | 现代 API 指针 | 应用开发者 | 安全、异步、现代感 |
| **WSL** | Linux 内核 | 全栈/后端开发者 | 拥抱开源、POSIX 兼容 |


## **Windows Core API**

```
          [ 高层：应用 & GUI ]
 WinRT / WinUI / UWP / WPF / Windows Forms / MFC ...

          [ 核心用户态 API ]
 Win32 API（User32 / GDI / Kernel32 / Advapi32 / ...）

          [ Native NT API ]
 ntdll.dll 里的 Nt*/Zw* 函数（未完全公开）

          [ 内核模式 API ]
 WDK / 驱动里的 Io*/Zw*/Ke* 等
```

**定位：**

- Windows 系统的“骨架”，底层系统调用接口
  
- 提供对内核对象、进程、线程、内存、文件、设备、GUI 消息循环的访问
  

**主要包含：**

- **Win32 API**（kernel32, user32, gdi32, advapi32, ws2_32 等）
  
- **Native NT API**（ntdll.dll 中的 Nt*/Zw* 系列）
  
- **内核模式 API**（WDK 驱动 API，如 Io*, Ke*, Mm*）
  

**特点：**

- 稳定、跨版本
  
- 直接操作系统资源
  
- 安全/攻防/漏洞分析的核心依赖
  

**示例用途：**

- 进程/线程管理、文件 I/O、内存管理、GUI 窗口、句柄操作
  
- 系统级工具、底层监控、Rootkit/EDR 内核模块
  

---

## **Windows-App API/Framework**

**定位：**

- 面向应用开发的高级封装和运行时
  
- 抽象底层 API，提供现代 GUI、组件化、跨语言、跨平台的开发接口
  

**主要包含：**

- **WinRT / Windows App SDK / WinUI / UWP**
  
- **WPF / Windows Forms / MFC**
  
- **COM / Shell API**（GUI/组件对象接口）
  
- **DirectX / GDI+ / Media Foundation**（专用子系统封装）
  

**特点：**

- 面向对象、事件驱动、语言无关或托管语言支持
  
- 底层仍然依赖 Core Windows API
  
- 稳定性主要针对应用开发而非安全研究
  

**示例用途：**

- 桌面现代应用
  
- 图形/音视频应用
  
- 跨语言组件开发
  

---

## **Windows Extensions API**

**定位：**

- 为兼容、移植、管理、运维提供的附加接口
  
- 不直接操控系统核心资源，而是封装 Core 或 App API
  

**主要包含：**

- **POSIX 兼容层**（Cygwin / MSYS2 / WSL 用户态）
  
- **.NET Base Class Library (BCL)**
  
- **WMI / PowerShell API**（系统管理、信息查询）
  
- **其他高层 SDK 或扩展库**
  

**特点：**

- 离内核最远，抽象度最高
  
- 主要作用是方便开发、跨平台或系统管理
  
- 对安全研究/攻击/漏洞分析意义有限
  

**示例用途：**

- 移植 Unix/Linux 工具
  
- 系统管理脚本/远程管理
  
- 高层应用逻辑封装