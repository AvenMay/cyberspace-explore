# GNU/Linux

```
Shell/Utilities (bash, ls, ps, cd, etc.)
   |     |
   |     |
   |    Libc (POSIX | glibc,musl,etc.) 
   |     |
   V     V
  System-Call (open, read, write, mmap, fork, etc.)
       |
       V
   OS-Kernel (Linux-Kernel | Process, Memory, IPC, File-System, Network, Driver)
       |
       V
    Hardware (CPU, Memory, Disk, Network, Device, etc.)
```

## Shell/Bash

- [Linux Shell脚本攻略.第3版.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%20Shell%E8%84%9A%E6%9C%AC%E6%94%BB%E7%95%A5.%E7%AC%AC3%E7%89%88.pdf)
- [Linux 命令大全.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%20%E5%91%BD%E4%BB%A4%E5%A4%A7%E5%85%A8.pdf)
- [Linux 运维入门到高级全套系列.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%20%E8%BF%90%E7%BB%B4%E5%85%A5%E9%97%A8%E5%88%B0%E9%AB%98%E7%BA%A7%E5%85%A8%E5%A5%97%E7%B3%BB%E5%88%97.pdf)
- [Liux Command Line and Shell Scripting]({{ files_server }}/software-engineering/sysadmin/gnu-linux/linux-command-line-and-shell-scripting-bible-by-richard-blum-christine-bresnahan.pdf)
- [Linux命令行与shell脚本编程大全 4th.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%E5%91%BD%E4%BB%A4%E8%A1%8C%E4%B8%8Eshell%E8%84%9A%E6%9C%AC%E7%BC%96%E7%A8%8B%E5%A4%A7%E5%85%A8%204th.pdf)
- [Linux学习笔记.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0.pdf)
- [Linux就该这么学第2版.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%E5%B0%B1%E8%AF%A5%E8%BF%99%E4%B9%88%E5%AD%A6%E7%AC%AC2%E7%89%88.pdf)
- [Linux系统编程 2nd.epub]({{ files_server }}/software-engineering/sysadmin/gnu-linux/Linux%E7%B3%BB%E7%BB%9F%E7%BC%96%E7%A8%8B%202nd.epub)
- [鸟哥的 Linux 私房菜：基础学习篇.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/%E9%B8%9F%E5%93%A5%E7%9A%84%20Linux%20%E7%A7%81%E6%88%BF%E8%8F%9C%EF%BC%9A%E5%9F%BA%E7%A1%80%E5%AD%A6%E4%B9%A0%E7%AF%87.pdf)
- [鸟哥的Linux私房菜-基础 4th.pdf]({{ files_server }}/software-engineering/sysadmin/gnu-linux/%E9%B8%9F%E5%93%A5%E7%9A%84Linux%E7%A7%81%E6%88%BF%E8%8F%9C-%E5%9F%BA%E7%A1%80%204th.pdf)
- [鸟哥的Linux私房菜：服务器架设篇(第3版).epub]({{ files_server }}/software-engineering/sysadmin/gnu-linux/%E9%B8%9F%E5%93%A5%E7%9A%84Linux%E7%A7%81%E6%88%BF%E8%8F%9C%EF%BC%9A%E6%9C%8D%E5%8A%A1%E5%99%A8%E6%9E%B6%E8%AE%BE%E7%AF%87%28%E7%AC%AC3%E7%89%88%29.epub)

### System Internal

- [Linux TCP IP 协议栈分析.pdf]({{ files_server }}/computer-science/operating-system/linux/Linux%20TCP%20IP%20%E5%8D%8F%E8%AE%AE%E6%A0%88%E5%88%86%E6%9E%90.pdf)
- [Linux内核API完全参考手册.epub]({{ files_server }}/computer-science/operating-system/linux/Linux%E5%86%85%E6%A0%B8API%E5%AE%8C%E5%85%A8%E5%8F%82%E8%80%83%E6%89%8B%E5%86%8C.epub)
- [Linux内核设计与实现(原书第3版).pdf]({{ files_server }}/computer-science/operating-system/linux/Linux%E5%86%85%E6%A0%B8%E8%AE%BE%E8%AE%A1%E4%B8%8E%E5%AE%9E%E7%8E%B0%28%E5%8E%9F%E4%B9%A6%E7%AC%AC3%E7%89%88%29.pdf)
- [Linux网络编程.pdf]({{ files_server }}/computer-science/operating-system/linux/Linux%E7%BD%91%E7%BB%9C%E7%BC%96%E7%A8%8B.pdf)
- [Linux设备驱动程序(中文第三版).pdf]({{ files_server }}/computer-science/operating-system/linux/Linux%E8%AE%BE%E5%A4%87%E9%A9%B1%E5%8A%A8%E7%A8%8B%E5%BA%8F%28%E4%B8%AD%E6%96%87%E7%AC%AC%E4%B8%89%E7%89%88%29.pdf)
- [深入理解LINUX内核(第三版).pdf]({{ files_server }}/computer-science/operating-system/linux/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3LINUX%E5%86%85%E6%A0%B8%28%E7%AC%AC%E4%B8%89%E7%89%88%29.pdf)
- [深入理解LINUX网络技术内幕.pdf]({{ files_server }}/computer-science/operating-system/linux/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3LINUX%E7%BD%91%E7%BB%9C%E6%8A%80%E6%9C%AF%E5%86%85%E5%B9%95.pdf)

### Linux Syscall API

- [syscalls](https://www.man7.org/linux/man-pages/man2/syscalls.2.html)

### Linux Kernel

- [The Linux Kernel documentation¶](https://docs.kernel.org/next/index.html)
- [Linux Kernel](https://www.kernel.org/)

## GNU/Linux GUI

- X11 
- Wayland

## Distributions

- Debian
- RHEL
- SUSE
- Arch Linux
- Alpine OS