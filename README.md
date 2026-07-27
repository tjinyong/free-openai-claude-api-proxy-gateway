<div align="center">

# YesAPI - AI API 中转站

**低成本、OpenAI 兼容的 AI API 接入服务**

**OpenAI-compatible API endpoint for GPT, Claude, Gemini, DeepSeek, Qwen, Grok and more**

<p>
  <a href="https://yesapi.online?utm_source=github&utm_medium=docs"><img src="https://img.shields.io/badge/Status-Online-16a34a?style=for-the-badge" alt="Status Online"></a>
  <a href="https://yesapi.online?utm_source=github&utm_medium=docs"><img src="https://img.shields.io/badge/OpenAI%20Compatible-/v1%20Endpoint-2563eb?style=for-the-badge" alt="OpenAI compatible endpoint"></a>
  <a href="https://yesapi.online?utm_source=github&utm_medium=docs"><img src="https://img.shields.io/badge/%C2%A510-%2410%20Credit-f97316?style=for-the-badge" alt="CNY top up credit"></a>
  <a href="https://yesapi.online?utm_source=github&utm_medium=docs"><img src="https://img.shields.io/badge/%241.50-%2410%20Credit-0f766e?style=for-the-badge" alt="USD top up credit"></a>
</p>

[中文版本](#中文版本) | [English](#english) | [控制台 / Console](https://yesapi.online?utm_source=github&utm_medium=docs) | [API 文档 / Docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)

</div>

---

<a id="中文版本"></a>

## 中文版本

YesAPI 面向开发者、AI 编程工具用户和自动化应用，提供低成本的 AI API 接入能力。它兼容 OpenAI API 格式，通常只需要替换 `Base URL`，就可以在现有 SDK 或客户端里使用。

适合这些场景：

- Cursor、Windsurf、Trae、Claude Code、OpenCode 等 AI 编程工具
- NextChat、LobeChat、ChatBox、Dify、LangChain 等应用和框架
- 聊天机器人、自动化 Agent、批量内容生成、内部工具开发
- 需要同时使用 GPT、Claude、Gemini、DeepSeek、Qwen、Grok 等模型的项目

### 价格与额度

| 项目 | 数值 |
| :--- | :--- |
| 支付 | <span style="color:#dc2626"><strong>¥10.00</strong></span> |
| 到账 | <span style="color:#dc2626"><strong>$10.00</strong></span> 平台额度 |
| 可用额度 | 约 <span style="color:#dc2626"><strong>$50.00</strong></span> 可用模型价值 |

以 0.2 倍率模型为例，`$10.00` 平台额度约等于 `$50.00` 可用模型价值。美元支付用户可按 **$1.50** 获得 **$10.00** 平台额度。

> 实际价格、模型倍率和到账额度以 YesAPI 控制台展示为准。

<p align="center">
  <img src="./yesapi-value-cn.svg" alt="支付 ¥10，到账 $10 额度，低倍率模型约 $50 可用价值" width="860">
</p>

### 快速接入

```text
Base URL: https://yesapi.online/v1
API Key:  你的 YesAPI 密钥
Docs:     https://doc.yesapi.online?utm_source=github&utm_medium=docs
```

### Python 示例

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-your-yesapi-key",
    base_url="https://yesapi.online/v1",
)

response = client.chat.completions.create(
    model="gpt-5.6-sol",
    messages=[{"role": "user", "content": "Hello YesAPI"}],
)

print(response.choices[0].message.content)
```

### 常见问题

**需要改代码吗？**

如果你的项目本来就使用 OpenAI SDK 或 OpenAI-compatible 客户端，通常只需要把 `Base URL` 改成 `https://yesapi.online/v1`，再填入 YesAPI 密钥。

**余额只能用于一个模型吗？**

不是。YesAPI 余额可以用于平台支持的多个模型，具体可用模型和倍率以控制台展示为准。

**为什么余额更耐用？**

充值到账额度和模型倍率会共同影响实际可用量。低倍率模型消耗更少，同样余额可以使用更久。

[立即使用 YesAPI](https://yesapi.online?utm_source=github&utm_medium=docs) | [查看 API 文档](https://doc.yesapi.online?utm_source=github&utm_medium=docs)

---

<a id="english"></a>

## English

YesAPI provides a low-cost, OpenAI-compatible API endpoint for developers, coding agents, automation workflows, and AI apps. In most integrations, you only need to replace the `Base URL` and keep using your existing SDK or client.

Common use cases:

- Cursor, Windsurf, Trae, Claude Code, OpenCode and other AI coding tools
- NextChat, LobeChat, ChatBox, Dify, LangChain and custom API apps
- Chatbots, coding agents, batch content generation and internal tools
- Projects that use GPT, Claude, Gemini, DeepSeek, Qwen, Grok and other model families

### Pricing and credit

| Item | Value |
| :--- | :--- |
| Payment | <span style="color:#dc2626"><strong>$1.50</strong></span> |
| Platform credit | <span style="color:#dc2626"><strong>$10.00</strong></span> |
| Usable value | About <span style="color:#dc2626"><strong>$50.00</strong></span> of model usage |

At a 0.2x model rate, `$10.00` platform credit can represent about `$50.00` of usable model value. Chinese users can pay **¥10.00** to receive **$10.00** platform credit.

> Final pricing, model rates and credited balance are based on the YesAPI console.

<p align="center">
  <img src="./yesapi-value-en.svg" alt="Pay $1.50, get $10 credit, about $50 usable value at low model rate" width="860">
</p>

### Quick start

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
Docs:     https://doc.yesapi.online?utm_source=github&utm_medium=docs
```

### TypeScript example

```typescript
import OpenAI from "openai";

const openai = new OpenAI({
  apiKey: "sk-your-yesapi-key",
  baseURL: "https://yesapi.online/v1",
});

async function main() {
  const completion = await openai.chat.completions.create({
    model: "gpt-5.6-sol",
    messages: [{ role: "user", content: "Hello YesAPI" }],
  });

  console.log(completion.choices[0].message.content);
}

main();
```

### Supported clients and models

YesAPI works with OpenAI-compatible SDKs and tools such as Cursor, Claude Code, OpenCode, NextChat, LobeChat, Dify and LangChain. Supported model families include GPT, Claude, Gemini, DeepSeek, Qwen, Grok, image generation and video generation models.

## Developer Guides

| Topic | Guide |
| :--- | :--- |
| Base URL setup | [Configure YesAPI Base URL](docs/quickstart/base-url-setup.md) |
| API key | [Get a YesAPI API Key](docs/quickstart/get-api-key.md) |
| Cursor | [Cursor Integration with YesAPI](docs/integrations/cursor-integration.md) |
| Claude Code | [Claude Code Guide for YesAPI](docs/integrations/claude-code-guide.md) |
| OpenCode | [OpenCode Setup with YesAPI](docs/integrations/opencode-setup.md) |
| Missing /v1 | [Base URL Must Include /v1](docs/troubleshooting/base-url-v1.md) |
| Streaming issue | [Stream Response Ended Unexpectedly](docs/troubleshooting/stream-response-ended.md) |
| Roadmap | [Phase 2 Documentation Roadmap](docs/phase-2-roadmap.md) |

[Start with YesAPI](https://yesapi.online?utm_source=github&utm_medium=docs) | [Read the docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
