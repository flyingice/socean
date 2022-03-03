# 故障排除

## **"Transaction simulation failed: Error processing Instruction 1: custom program error: 0x1"**

当您没有足够的额外SOL用来支付创建新scnSOL代币账户所需的交易成本和租金时，就会出现此问题。尝试预留～0.1 SOL在您的钱包中，而不要用尽它们。

## 当我点击“Approve”时，交易无法通过。

您正在使用Ledger硬件钱包（Ledger Nano X/Nano S)吗？如果是的话，请**启用盲签名**(blind signing).

{% embed url="https://support.ledger.com/hc/en-us/articles/360016265659-Solana-SOL-?docs=true" %}
Ledger Live说明文档
{% endembed %}

> 在Solana区块链上发送代币前，确保您在Solana应用程序设置中启用了**盲签名**（blind signing）。
>
> 启动盲签名（blind signing）：
>
> 1. 连接并解锁您的Ledger设备。
> 2. 打开**Solana**应用程序。
> 3. 按下右侧按钮导航到**设置**（Settings）。然后同时按下两边按钮确认。
> 4. 在**盲签名**（Blind signing）设置中，同时按下两边按钮选择**是**（Yes）。
