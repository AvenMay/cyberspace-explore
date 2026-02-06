# HomeLab Setup

HomeLab架构集中在一个 **10英寸 x 9U 迷你机柜** 中，作为一个Private Cloud环境运行。通过结合Public-Cloud VPS可以扩展为Hybrid Cloud

<!-- **Project MINI RACK**项目旨在为紧凑型家庭实验室提供微型机柜构建指南，我的设置遵循了这一理念。 -->

![homelab](./images/homelab.jpg)

## Infrastructure Overview

### Rack Stack

#### 10” Mini Rack

这是整个家庭实验室的核心，许多制造商已经统一了 10 英寸机柜的 1U 高度标准（44.45mm 或 1.75 英寸）。

| 型号  | 单元高度 (Unit Height) | 附加信息 |
| --- | --- | --- |
| **金属机柜** | 9U  | 10 英寸 x 9U 机柜 |

#### Power

电源分配单元（PDU）负责将单一电源转换为多个插座，以供机柜内设备使用。

| 型号  | 单元高度 (Unit Height) | 附加信息 |
| --- | --- | --- |
| PDU | N/A | 4端口 PDU x 2 |

#### Panels

跳线面板有助于整理 RJ45 网线、USB、HDMI 等信号线缆，以实现整洁的安装和维护。全部使用开源的3D 打印部件。

| 设备类型 | 数量  | 材质/型号 | 附加信息 |
| --- | --- | --- | --- |
| **Patch Panel** | 2 | 12/12 | 3D 打印 |
| **RJ45 Keystone** | 16 | 12+4 端口跳线 | 3D 打印 |
| **Patch Panel** | 2   | 12 端口跳线面板 | 3D 打印 |
| **Rack Panels** | 1   | Netgear 机架面板 | 3D 打印 |
| **Rack Panels** | 1   | Beelink EQ12 机架面板 | 3D 打印 |
| **Rack Panels** | 1   | Dell OptiPlex MFF 机架面板 | 3D 打印 |
| **Rack Panels** | 1   | LabStack (Pi Cluster) 机架面板 | 3D 打印，用于 SBC 集群, |
| **Ventilation Panels** | 1   | N/A | 3D 打印 |

#### Cable Management

如果没有适当的配件，迷你机柜很容易从“美观”变成“混乱”，因此需要线缆管理配件来整理凌乱的线缆。

- 1.5cm 蓝色网线 x 7
- 1.5cm 红色网线 x 1
- 2cm 黄色网线 x 1


[--Image of: --机柜内部正面图占位符]

### Network Stack

网络交换机或路由器是家庭实验室的核心。由于许多小型设备不原生支持 10 英寸机架安装，通常需要使用货架或 3D 打印适配器,。

| 型号  | 单元高度 (Unit Height) | 附加信息 |
| --- | --- | --- |
| **交换机** | N/A | Netgear GS108E 8 端口千兆交换机 |
| **无线路由器** | N/A | Netgear RAX20 无线路由器 |

#### PVE Networking Stack

该服务器主要负责网络功能虚拟化。

- **硬件:** Intel N150 PC + Proxmox-VE
- **规格:** 16G RAM / 256G SSD
- **运行服务:** Openwrt, OPNsense, Debian/Docker

### Compute Resources

微型 PC 和单板计算机（SBC）因其低功耗、低散热需求和紧凑的尺寸，是迷你机柜的理想选择。


#### PVE Main Server

该服务器提供了主要的计算和开发环境。

- **硬件:** Dell OptiPlex MFF + Proxmox-VE
- **规格:** 16G RAM / 1T SSD
- **运行服务:** Debian/Docker, Debian 开发服务器, Kali Linux, Windows 10/11

#### Pi K8S Cluster

这是一个由 **4 节点 Raspberry Pi 5 8G** 组成的 Kubernetes 集群。许多迷你机柜设置都围绕 SBC 集群展开。

| 节点  | 角色  | 硬件配置 | 存储  |
| --- | --- | --- | --- |
| **Node-1** | Master Node, Stateless Node | Raspberry Pi 5 8G | USB to Sata 2.5 SSD 128G |
| **Node-2** | Worker Node, Persistence Node | Raspberry Pi 5 8G | USB to Sata 2.5 HDD 128G |
| **Node-3** | Worker Node, Stateless Node | Raspberry Pi 5 8G | A3U2 TF-Card 64G |
| **Node-4** | Worker Node, Stateless Node | Raspberry Pi 5 8G | A3U2 TF-Card 64G |

[--Image of: --Pi K8S 集群特写占位符]

## Applications Overview

家庭实验室中可以运行许多软件，这些软件在迷你 PC 或 SBC 上运行良好。我的应用主要包括管理和监控界面。

| 应用类别 | 应用名称 | 需求/用途 |
| --- | --- | --- |
| **主页/仪表盘 (Home Page/Dashboards)** | Dashy, Homer, Homarr | 各个 HomeLab 应用的 URL 入口, Free Dashbroad Icons, Proxy |


## References

- [Project MINI RACK [Jeff Geerling]](https://mini-rack.jeffgeerling.com/)
- [LabStack [JaredC01]](https://github.com/JaredC01/LabStack)