# DPDK简易协议栈项目简介
- 项目名称: Gangan_DPDK_Demo
- 项目描述:
本项目旨在利用DPDK (Data Plane Development Kit) 实现一个高效、轻量级的TCP/UDP协议栈，以加速数据平面处理并降低延迟。DPDK提供了高性能的数据包处理能力，通过旁路内核协议栈，直接在用户态进行数据包的收发，从而显著提升网络应用的吞吐量和响应速度。

# 主要功能:
- ARP协议: 实现地址解析协议，用于在网络中查找对应IP地址的硬件地址（MAC地址）。
- ICMP协议: 实现Internet控制消息协议，用于发送错误消息和控制信息，如ping命令。
- TCP协议: 提供面向连接的、可靠的字节流服务，支持数据包的顺序传输和错误恢复。
- UDP协议: 提供无连接的、不可靠的服务，适合对延迟敏感的应用场景。
# 技术栈:
- DPDK: 数据平面开发工具包，用于高速数据包处理。
- C语言: 主要编程语言，用于编写协议栈代码。
- Makefile: 构建系统，用于编译和链接源代码。

# 编译与运行:
确保安装了DPDK环境和必要的依赖库。
使用make命令在项目根目录下构建项目。
运行生成的可执行文件，通常命名为dpdk_tcp或根据Makefile配置命名。