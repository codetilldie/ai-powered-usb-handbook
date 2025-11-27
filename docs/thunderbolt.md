# Thunderbolt (雷电) 技术 (Thunderbolt Technology)

Thunderbolt 是由 Intel 和 Apple 合作开发的接口技术，以“快”和“全能”著称。

## Thunderbolt 3 (雷电 3)

-   **接口**：采用 USB Type-C 物理接口。
-   **带宽**：最高 40 Gbps。
-   **特性**：支持 PCIe x4 (用于外接显卡)、DisplayPort (用于 5K/8K 显示器) 和 USB 协议。
-   **局限**：早期雷电 3 控制器对 USB 3.x 的兼容性有时不如原生 USB 接口好。

## Thunderbolt 4 (雷电 4)

雷电 4 并没有提升最高带宽（依然是 40 Gbps），但它**提高了最低下限**，保证了更一致的用户体验。

### 雷电 4 vs 雷电 3 的关键区别

1.  **PCIe 带宽要求**：雷电 4 要求 PCIe 传输速度至少达到 **32 Gbps** (雷电 3 仅要求 16 Gbps)。这对连接外置显卡 (eGPU) 和高速 SSD 至关重要。
2.  **显示支持**：雷电 4 要求至少支持 **双路 4K 显示器** 或 **单路 8K 显示器** (雷电 3 仅要求单路 4K)。
3.  **安全性**：强制要求支持 Intel VT-d DMA 保护，防止物理 DMA 攻击。
4.  **配件扩展**：雷电 4 官方支持**雷电扩展坞 (Hub)** 带有多个下行雷电接口（例如 1 分 3），而雷电 3 只能菊花链 (Daisy Chain)。

## Thunderbolt vs USB4

-   **关系**：USB4 是基于雷电 3 协议开发的。
-   **区别**：
    -   **USB4 是一个“宽泛”的标准**：厂商可以选择性支持 20Gbps 或 40Gbps，也可以选择不支持 PCIe。
    -   **Thunderbolt 4 是一个“严格”的认证**：必须跑满 40Gbps，必须支持 PCIe，必须通过 Intel 认证。
    -   **结论**：基本上可以认为 **Thunderbolt 4 是 USB4 的“满血顶配版”**。
