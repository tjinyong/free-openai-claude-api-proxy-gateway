# ⚡ Free API Proxy & Aggregator for Claude 5 (Opus 5 & Sonnet 5), OpenAI (GPT-5.6 Sol, GPT-5o) & DeepSeek

<p naming="languages">
  <b>Language / 语言:</b>
  <a href="#english">English</a> | 
  <a href="#chinese">中文文档</a>
</p>

[![Status](https://img.shields.io/badge/API_Status-99.9%25_Uptime-brightgreen)](https://yesapi.online)
[![Supports](https://img.shields.io/badge/Supports-Cursor_%7C_Windsurf_%7C_Trae-blue)](https://yesapi.online)
[![Pricing](https://img.shields.io/badge/Pricing-As_Low_As_3%25-red)](https://yesapi.online)

---

<a name="english"></a>
## 🌐 English

> **Looking for a high-speed, stable, and ultra-affordable API Proxy & LLM Aggregator?**
> [YesAPI](https://yesapi.online) provides low-latency, enterprise-grade API access for developers and global teams. Save up to **97% off official pricing** with zero hidden fees! Fully compatible with official OpenAI/Anthropic SDKs and major AI coding tools.

🔗 **Official Website & Free Trial**: [https://yesapi.online](https://yesapi.online)

### 💰 Unbeatable Pricing & Discount Mechanics
We offer **costs as low as 3% of official API prices**!
- **Example (0.2x Ratio Model)**: Recharge **$10.00** $\rightarrow$ Get **$50.00 Credit** balance!
- Balance can be used across **all supported models** (Claude 5, GPT-5.6, DeepSeek, etc.).

### 📌 Why Choose YesAPI Proxy?
- 💸 **As Low As 3% Cost**: Enjoy enterprise LLM performance at a fraction of official rates.
- 🚀 **Ultra-Low Latency**: Multi-region route optimization for instant code completion in Cursor, Windsurf, and Trae.
- 🛡️ **High Uptime**: Built with dedicated PostgreSQL, Redis cache, and Cloudflare DDoS protection.
- 💳 **Global & Local Payments**: Supports USD (Credit Cards/Crypto) and CNY.

### 📊 Supported Models
| Provider | Model ID | Core Capability | Context Window |
| :--- | :--- | :--- | :--- |
| **Anthropic** | `claude-opus-5` / `claude-sonnet-5` | Frontier Agentic Coding & Adaptive Thinking | 1M |
| **OpenAI** | `gpt-5.6-sol` / `gpt-5.6-terra` | Flagship Reasoning & Advanced Agent Workflows | 1.05M |
| **OpenAI** | `gpt-5o` / `gpt-5o-mini` | Low-Latency Multimodal & Everyday Knowledge Work | 256k |
| **DeepSeek** | `deepseek-chat` / `deepseek-coder` | High-Efficiency Budget Coding & Fast Inference | 128k |

---

<a name="chinese"></a>
## 🇨🇳 中文文档

> **寻找高速、稳定且极具性价比的 AI API 中转站与聚合网关？**
> [YesAPI 稳定中转站](https://yesapi.online) 为开发者及企业团队提供低延迟、企业级的 API 中转服务。相比官方直连**最高可节省 97% 成本**，无任何隐藏费用！全面兼容 OpenAI/Anthropic 官方 SDK 及各大 AI 编程工具（Cursor / Windsurf / Trae）。

🔗 **官网入口与免费测试**: [https://yesapi.online](https://yesapi.online)

### 💰 极致性价比与充值折算说明
成本最低可至官方价格的 **3%**，大幅降低 AI 开发与使用成本！
- **充值示例（以 0.2 倍率模型为例）**：充值 **$10.00（或等值人民币）** $\rightarrow$ 可得 **$50.00 额度**！
- 账户余额通用，可无缝用于全站**所有支持的模型**（Claude 5、GPT-5.6、DeepSeek 等）。

### 📌 为什么选择 YesAPI 中转站？
- 💸 **低至 3% 成本**：以几分钱的价格享受顶尖旗舰大模型性能。
- 🚀 **极速低延迟**：多机房线路优化 + 独立缓存，保障 Cursor、Windsurf 等 IDE 代码补全丝滑不卡顿。
- 🛡️ **高可用架构**：独立 PostgreSQL + 独立 Redis 缓存 + Cloudflare 高防，拒绝断连与抽风。
- 💳 **灵活支付**：支持美元（信用卡/加密货币）及人民币快速充值。

---

## 🛠️ Quick Integration / 快速接入指南

### 1. Cursor IDE 接入设置
1. 打开 Cursor 设置 -> **Models** -> **OpenAI API Key**。
2. 将 **Base URL** 修改为: `https://yesapi.online/v1`
3. 填入你在 YesAPI 获得的 API Key 即可开始使用。

### 2. NextChat / LobeChat / One-API 接入
- **API 接口地址 (Host)**: `https://yesapi.online`
- **密钥 (Secret Key)**: 你的 YesAPI Key (`sk-...`)

### 3. Python SDK 代码示例
```python
import openai

client = openai.OpenAI(
    base_url="[https://yesapi.online/v1](https://yesapi.online/v1)",
    api_key="your-yesapi-key"
)

response = client.chat.completions.create(
    model="claude-sonnet-5",
    messages=[{"role": "user", "content": "Hello YesAPI"}]
)
print(response.choices[0].message.content)

```
❓ FAQ / 常见问题
Q: 倍率折算机制是怎么计算的？ / How does the pricing multiplier work?
我们采用倍率模型（如 0.2 倍率）。当您充值 $10 时，账户实际到账 $50 额度，从而将 API 使用成本大幅压低至官方原价的 3%~20%。

Q: 中转站安全且隐私吗？ / Is this API proxy safe and private?
是的。我们严格遵守无日志政策（No-Logs Policy），绝不存储用户的 Request/Response 请求体内容，全程 SSL 加密传输。

Q: 如何领取免费测试额度？ / How to get a free test API Key?
只需前往 https://yesapi.online 注册新账号，即可自动获得免费测试额度。

🌐 Resources / 相关资源
官网 / Website: https://yesapi.online

文档 / Documentation: https://yesapi.online/docs

---
