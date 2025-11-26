# Boot-Process

## BIOS

- OpenBIOS

## UEFI

## Bootloader

### Linux
- GRUB
- LILO
- Syslinux

### Windows
- Windows Boot Manager

## Partition-Table

- GPT
- MBR

## Boot 过程的详细步骤：

1. **加电自检 (Power-On Self Test, POST)**
  当计算机被加电后，BIOS（或 UEFI，现代计算机多使用 UEFI）首先被加载。它会进行**自检**（POST），检查硬件是否正常工作（如内存、硬盘、显卡等）。如果硬件通过检查，BIOS 会发出信号表示硬件是正常的，若有问题，则会通过蜂鸣声或错误信息提示用户。
  
2. **初始化硬件**
  在自检完成后，BIOS 会初始化计算机的硬件组件，比如 CPU、内存、硬盘、键盘、显示器等。这个阶段确保计算机的硬件能够正常协作。
  
3. **查找启动设备**
  BIOS 会根据预设的启动顺序查找一个有效的启动设备。这个设备可能是硬盘、固态硬盘、光盘、USB 闪存盘等。启动顺序通常可以在 BIOS 设置界面中进行配置（例如，优先从 USB 启动，或者从硬盘启动）。
  
4. **加载 Bootloader**
  一旦 BIOS 找到一个有效的启动设备，它会读取该设备上的 **Bootloader**（引导程序）。Bootloader 是一个相对小的程序，负责将操作系统的核心部分加载到内存中，并启动操作系统的运行。
  
  - Bootloader 的类型和位置
    
    ：常见的 Bootloader 可能存储在硬盘的主引导记录（MBR）或 GUID 分区表（GPT）中。操作系统通常会提供一个 Bootloader。例如：
    
    - 对于 Windows 操作系统，Bootloader 通常是 `bootmgr`。
    - 对于 Linux 操作系统，Bootloader 通常是 **GRUB**（Grand Unified Bootloader）。
  
  该程序在 BIOS 加载后执行，并开始引导操作系统。
  
5. **引导操作系统**
  Bootloader 会开始加载操作系统的内核文件，并将控制权交给操作系统。具体来说，Bootloader 会：
  
  - 查找并加载操作系统的内核（例如，Linux 的 `vmlinuz` 或 Windows 的 `ntoskrnl.exe`）。
  - 设置操作系统所需的环境，完成操作系统内核的初始化。
  - 操作系统内核初始化后，控制权交给操作系统，之后计算机进入操作系统的运行状态。

### 总结：

- **BIOS** 负责硬件初始化和启动引导程序的加载。
- **Bootloader** 是操作系统提供的小程序，它负责引导操作系统内核的加载。
- **操作系统** 在 Bootloader 的帮助下被加载并运行。

这个过程确保了计算机从开机到操作系统完全启动并可使用的完整过程