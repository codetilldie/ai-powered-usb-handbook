# 第 3 章：USB 传输协议 (USB Transfer Protocols)

USB 协议决定了数据传输的**速度**。由于 USB-IF (USB 开发者论坛) 多次更改命名规则，导致市场上存在大量混淆的名称。

## 早期标准

-   **USB 1.0 / 1.1**:
    -   **Low Speed**: 1.5 Mbps (用于键盘鼠标)
    -   **Full Speed**: 12 Mbps
-   **USB 2.0**:
    -   **High Speed**: 480 Mbps。这是目前大多数“仅充电线”或入门手机的数据传输上限。

## USB 3.x 命名大乱斗

这是最让人头疼的部分。请参考下表进行对照：

| 原始名称 | 第一次改名 (2013) | 第二次改名 (2019) | 市场通俗名称 | 理论带宽 | 编码方式 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **USB 3.0** | USB 3.1 Gen 1 | **USB 3.2 Gen 1** | USB 3.0 / 5Gbps | 5 Gbps | 8b/10b |
| N/A | **USB 3.1 Gen 2** | **USB 3.2 Gen 2** | USB 3.1 / 10Gbps | 10 Gbps | 128b/132b |
| N/A | N/A | **USB 3.2 Gen 2x2** | USB 3.2 / 20Gbps | 20 Gbps | 128b/132b |

> **注意**：USB 3.2 Gen 2x2 需要使用 Type-C 接口，因为它利用了 Type-C 的两组高速通道同时传输（双通道）。

## USB4

USB4 基于 Intel 捐赠的 Thunderbolt 3 协议构建，旨在统一高速接口标准。

-   **USB4 Gen 2x2**: 20 Gbps
-   **USB4 Gen 3x2**: 40 Gbps (强制要求)
-   **主要特性**：
    -   **隧道技术 (Tunneling)**：可以动态分配带宽给数据 (USB 3.2)、显示 (DisplayPort) 和 PCIe。
    -   **兼容性**：向后兼容 USB 3.2、USB 2.0 和 Thunderbolt 3。
