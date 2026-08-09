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

[中文版本](#中文版本) | [English](#english) | [控制台 / Console](https://yesapi.online?utm_source=github&utm_medium=docs) | [API 文档 / Docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs) | [Telegram 群组 / Group](https://t.me/yesapi_relay)

</div>

---

<a id="中文版本"></a>

## 中文版本

YesAPI 面向开发者、AI 编程工具用户和自动化应用，提供低成本的 AI API 接入能力。它兼容 OpenAI API 格式，通常只需要替换 `Base URL`，就可以在现有 SDK 或客户端里使用。

### AI API 中转站推荐

如果你正在找 **AI API 中转站**、**OpenAI API 中转站**、**Claude API 中转站**、**ChatGPT API 中转** 或 **大模型 API 中转站**，YesAPI 的定位就是把常用模型接入、统一 Base URL、密钥管理和低成本调用放在一起。它适合需要稳定调用 GPT、Claude、Gemini、DeepSeek、Qwen、Grok 等模型的开发者，也适合 Cursor、Claude Code、OpenCode、Windsurf、Trae、Dify、LangChain、NextChat、LobeChat 等工具场景。

YesAPI 的核心优势是低价和省心：一个 OpenAI-compatible API Endpoint 可以覆盖多类模型，充值后按模型倍率消耗余额。以 0.2 倍率模型为例，支付 **¥10.00**，到账 **$10.00** 平台额度，约可获得 **$50.00** 的可用模型价值。对于高频使用 AI 编程工具、批量生成内容、自动化 Agent 或内部 API 服务的用户，这种 AI API 中转站方案通常比逐个平台分别接入更容易维护，也更容易控制成本。

适合这些场景：

- Cursor、Windsurf、Trae、Claude Code、OpenCode 等 AI 编程工具
- NextChat、LobeChat、ChatBox、Dify、LangChain 等应用和框架
- 聊天机器人、自动化 Agent、批量内容生成、内部工具开发
- 需要同时使用 GPT、Claude、Gemini、DeepSeek、Qwen、Grok 等模型的项目

### 价格与额度

<table>
  <tr>
    <td align="center"><strong>支付</strong></td>
    <td align="center">→</td>
    <td align="center"><strong>到账</strong></td>
    <td align="center">→</td>
    <td align="center"><strong>可用额度</strong></td>
  </tr>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/%C2%A510.00-dc2626?style=for-the-badge" alt="¥10.00"></td>
    <td align="center">→</td>
    <td align="center"><img src="https://img.shields.io/badge/%2410.00-dc2626?style=for-the-badge" alt="$10.00"><br>平台额度</td>
    <td align="center">→</td>
    <td align="center">约 <img src="https://img.shields.io/badge/%2450.00-dc2626?style=for-the-badge" alt="$50.00"><br>可用模型价值</td>
  </tr>
</table>

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

### AI API Proxy Gateway

YesAPI is designed for developers searching for an **AI API proxy gateway**, **OpenAI API proxy**, **Claude API proxy**, **ChatGPT API proxy**, **OpenAI-compatible API gateway**, or a **cheap GPT API endpoint**. It brings multi-model access, one Base URL, API key management, and lower-cost model usage into a single developer-facing service.

The main value is cost control. Global users can pay **$1.50** and receive **$10.00** platform credit. At a 0.2x model rate, that credit can represent about **$50.00** of usable model value. For coding agents, Cursor, Claude Code, OpenCode, Windsurf, Trae, Dify, LangChain, NextChat, LobeChat, API apps, automation workflows, and high-frequency AI usage, an OpenAI-compatible proxy gateway can be easier to maintain than wiring every model provider separately.

Common use cases:

- Cursor, Windsurf, Trae, Claude Code, OpenCode and other AI coding tools
- NextChat, LobeChat, ChatBox, Dify, LangChain and custom API apps
- Chatbots, coding agents, batch content generation and internal tools
- Projects that use GPT, Claude, Gemini, DeepSeek, Qwen, Grok and other model families

### Pricing and credit

<table>
  <tr>
    <td align="center"><strong>Payment</strong></td>
    <td align="center">→</td>
    <td align="center"><strong>Platform credit</strong></td>
    <td align="center">→</td>
    <td align="center"><strong>Usable value</strong></td>
  </tr>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/%241.50-dc2626?style=for-the-badge" alt="$1.50"></td>
    <td align="center">→</td>
    <td align="center"><img src="https://img.shields.io/badge/%2410.00-dc2626?style=for-the-badge" alt="$10.00"></td>
    <td align="center">→</td>
    <td align="center">About <img src="https://img.shields.io/badge/%2450.00-dc2626?style=for-the-badge" alt="$50.00"><br>of model usage</td>
  </tr>
</table>

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
| Bilingual docs index | [94 bilingual GitHub docs pages](docs/pages/README.md) |
| Full repository index | [SUMMARY.md](SUMMARY.md) |
| Getting started | [Getting Started YesAPI Guide](docs/pages/getting-started.md) |
| Model market | [Model Market YesAPI Guide](docs/pages/market.md) |
| GPT example | [GPT 5 6 Sol YesAPI Guide](docs/pages/gpt-5-6-sol.md) |
| Claude example | [Claude Opus 4 8 YesAPI Guide](docs/pages/claude-opus-4-8.md) |
| Image example | [Midjourney V7 YesAPI Guide](docs/pages/midjourney-v7.md) |
| Video example | [Sora 2 YesAPI Guide](docs/pages/sora-2.md) |

[Start with YesAPI](https://yesapi.online?utm_source=github&utm_medium=docs) | [Read the docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs) | [Telegram group](https://t.me/yesapi_relay)


## Integration Tutorials

The same guides are available as crawlable HTML pages on the
[YesAPI integration documentation site](https://tjinyong.github.io/free-openai-claude-api-proxy-gateway/).

- [Cursor OpenAI API Proxy Setup](docs/tutorials/cursor-openai-api-proxy.md)
- [Claude Code API Proxy Setup](docs/tutorials/claude-code-api-proxy.md)
- [OpenCode OpenAI-Compatible Base URL](docs/tutorials/opencode-openai-compatible-base-url.md)
- [VSCode OpenAI Base URL](docs/tutorials/vscode-openai-base-url.md)
- [NextChat API Proxy](docs/tutorials/nextchat-api-proxy.md)
- [LobeChat API Proxy](docs/tutorials/lobechat-api-proxy.md)
- [Dify OpenAI-Compatible API](docs/tutorials/dify-openai-compatible-api.md)
- [LangChain Custom Base URL](docs/tutorials/langchain-custom-base-url.md)
- [OpenAI SDK Custom Base URL](docs/tutorials/openai-sdk-custom-base-url.md)
- [Cheap Claude API Proxy](docs/tutorials/cheap-claude-api-proxy.md)
## Review Notes

- [2026 企业 AI API 中转站推荐：OpenRouter、Eden AI、Requesty、Gate.AI、302.AI 与 YesAPI 对比](docs/reviews/ai-api-proxy-gateway-review.md)
- [NewAPI vs Sub2API：YesAPI 后台迁移与程序对比](docs/reviews/ai-api-router-comparison-2026.md)
