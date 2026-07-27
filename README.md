# Free OpenAI Claude API Proxy Gateway | Cheap AI API Aggregator

<p align="center">
  <a href="#中文版本">中文版本</a>
  &nbsp;|&nbsp;
  <a href="#english-version">English Version</a>
  &nbsp;|&nbsp;
  <a href="https://yesapi.online">Start Now</a>
  &nbsp;|&nbsp;
  <a href="https://doc.yesapi.online">Docs</a>
</p>

<p align="center">
  <a href="https://yesapi.online"><img src="https://img.shields.io/badge/Top--up-%C2%A510%20%E2%86%92%20%2410%20Credit-f97316?style=for-the-badge" alt="CNY top-up deal"></a>
  <a href="https://yesapi.online"><img src="https://img.shields.io/badge/Top--up-%241.50%20%E2%86%92%20%2410%20Credit-16a34a?style=for-the-badge" alt="USD top-up deal"></a>
  <a href="https://yesapi.online"><img src="https://img.shields.io/badge/OpenAI%20Compatible-/v1%20API-2563eb?style=for-the-badge" alt="OpenAI compatible API"></a>
</p>

<div align="center">

## Cheap AI API access in one glance

### Pay less first. Spend less again by model rate.

| What you pay | What you get | Example usable value | Best for |
| :--- | :--- | :--- | :--- |
| **¥10.00** | **$10.00 platform credit** | **About $50.00 usable value at 0.2x model rate** | 中文用户、本地开发者、AI 编程工具 |
| **$1.50** | **$10.00 platform credit** | **About $50.00 usable value at 0.2x model rate** | Global users, coding agents, API apps |

**YesAPI** is an OpenAI-compatible AI API proxy gateway for GPT, Claude, Gemini, DeepSeek, Grok, Qwen and more. Use one API key, one base URL, and one balance across many models.

[**Start with YesAPI**](https://yesapi.online) · [**Read API Docs**](https://doc.yesapi.online) · [**中文说明**](#中文版本) · [**English Guide**](#english-version)

</div>

> Pricing and promotional credit may change. Always follow the actual price and balance shown on [yesapi.online](https://yesapi.online).

---

## Why this gateway is cheap

| Layer | Explanation | Example |
| :--- | :--- | :--- |
| **1. Top-up bonus** | Pay a small amount and receive more platform credit. | **¥10.00 / $1.50 -> $10.00 credit** |
| **2. Model rate discount** | Usage is consumed by each model's rate. Lower rate means longer usage. | **0.2x rate: $10 credit ≈ $50 model usage** |
| **3. Universal balance** | One balance works across supported models and providers. | GPT, Claude, Gemini, DeepSeek, Qwen, Grok |

## Quick API configuration

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
Docs:     https://doc.yesapi.online
Website:  https://yesapi.online
```

### OpenAI-compatible Python example

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://yesapi.online/v1",
    api_key="your-yesapi-key",
)

response = client.chat.completions.create(
    model="gpt-5.6-sol",
    messages=[{"role": "user", "content": "Hello YesAPI"}],
)

print(response.choices[0].message.content)
```

---

<a id="中文版本"></a>

# 中文版本

## ¥10 低门槛充值，到账 $10 额度

<p align="center">
  <img src="./yesapi-value-cn.svg" alt="支付 ¥10，到账 $10 额度，低倍率模型约 $50 可用价值" width="860">
</p>

YesAPI 是面向中文开发者、AI 编程工具用户和创业团队的 **低价 AI API 中转站 / 大模型聚合网关**。它兼容 OpenAI API 格式，可用于 Cursor、Windsurf、Trae、Claude Code、OpenCode、NextChat、LobeChat 等工具。

## 中文用户一眼看懂

| 重点 | 说明 |
| :--- | :--- |
| **充值便宜** | 示例：支付 **¥10.00**，到账 **$10.00 平台额度**。 |
| **使用更便宜** | 调用模型时按模型倍率消耗余额，低倍率模型更省。 |
| **余额更耐用** | 示例：0.2 倍率模型下，$10 额度约等于 $50 可用模型价值。 |
| **一个 Key 通用** | 一个 API Key 接入 GPT、Claude、Gemini、DeepSeek、Qwen、Grok 等模型。 |
| **适合 AI 编程** | 适合 Cursor、Windsurf、Trae、Claude Code、OpenCode 等高频调用场景。 |

## 支持模型示例

| 类型 | 模型示例 | 适合场景 |
| :--- | :--- | :--- |
| OpenAI / GPT | `gpt-5.6-sol`, `gpt-5.6-terra`, `gpt-5.5` | 代码、推理、Agent 工作流 |
| Claude | `claude-opus-4-8`, `claude-sonnet-4-6` | 长文本、代码理解、复杂任务 |
| Gemini | `gemini-3-pro`, `gemini-2.5-pro` | 多模态、长上下文、综合任务 |
| DeepSeek | `deepseek-v3-2`, `deepseek-r1` | 高性价比中文和代码任务 |
| 图像 / 视频 | `midjourney-v7`, `sora-2`, `veo-3-1` | 图片生成、视频生成、多媒体应用 |

## 中文快速接入

```text
API 地址: https://yesapi.online/v1
文档地址: https://doc.yesapi.online
官网入口: https://yesapi.online
```

### Cursor / Windsurf / Trae

1. 打开工具的模型或 API 设置。
2. 找到 OpenAI-compatible / OpenAI API Key 设置。
3. Base URL 填写：`https://yesapi.online/v1`
4. API Key 填写你的 YesAPI 密钥。

### 常见问题

**为什么看起来比官方便宜？**

因为有两层机制：充值到账优惠 + 模型倍率消耗。实际价格以网站展示为准。

**余额只能用于一个模型吗？**

不是。YesAPI 余额可用于平台支持的多个模型。

**适合什么用户？**

适合需要低成本使用 AI 编程工具、自动化 Agent、聊天机器人、批量内容生成、API 应用的用户。

[开始使用 YesAPI](https://yesapi.online) · [查看中文文档](https://doc.yesapi.online)

---

<a id="english-version"></a>

# English Version

## Pay $1.50, get $10 credit, use it across models

<p align="center">
  <img src="./yesapi-value-en.svg" alt="Pay $1.50, get $10 credit, about $50 usable value at low model rate" width="860">
</p>

YesAPI is a **low-cost OpenAI-compatible API proxy gateway** for developers, AI coding tools, startups, and automation workflows. It lets you call multiple model providers through one API key and one `/v1` endpoint.

## English users: what matters

| Highlight | Details |
| :--- | :--- |
| **Cheap entry** | Example: pay **$1.50** and get **$10.00 platform credit**. |
| **Lower usage cost** | Balance is consumed by model rate. Lower rate means longer usage. |
| **More usable value** | Example: at 0.2x model rate, $10 credit can represent about $50 model usage. |
| **One API key** | Use GPT, Claude, Gemini, DeepSeek, Qwen, Grok and more with one key. |
| **Built for coding tools** | Works with Cursor, Windsurf, Trae, Claude Code, OpenCode and API apps. |

## Example model coverage

| Category | Model examples | Use cases |
| :--- | :--- | :--- |
| OpenAI / GPT | `gpt-5.6-sol`, `gpt-5.6-terra`, `gpt-5.5` | Coding, reasoning, agent workflows |
| Claude | `claude-opus-4-8`, `claude-sonnet-4-6` | Long context, code review, complex tasks |
| Gemini | `gemini-3-pro`, `gemini-2.5-pro` | Multimodal work, long context, general tasks |
| DeepSeek | `deepseek-v3-2`, `deepseek-r1` | Cost-efficient coding and reasoning |
| Image / Video | `midjourney-v7`, `sora-2`, `veo-3-1` | Image generation, video generation, media apps |

## English quick start

```text
Base URL: https://yesapi.online/v1
Docs:     https://doc.yesapi.online
Website:  https://yesapi.online
```

### Cursor / Windsurf / Trae

1. Open the model or API settings.
2. Choose OpenAI-compatible API configuration.
3. Set Base URL to `https://yesapi.online/v1`.
4. Use your YesAPI API key.

### FAQ

**Why can it be cheaper than direct official APIs?**

Because usage can combine top-up credit promotion with model-rate consumption. Actual pricing is shown on the website.

**Can one balance be used across models?**

Yes. A single YesAPI balance can be used across supported providers and models.

**Who is this for?**

Developers, AI coding tool users, agent builders, API apps, startups, and high-frequency automation workflows.

[Start with YesAPI](https://yesapi.online) · [Read Docs](https://doc.yesapi.online)

---

## SEO keywords

OpenAI API proxy, Claude API proxy, cheap GPT API, cheap Claude API, OpenAI compatible API gateway, AI API aggregator, GPT-5.6 Sol API, Claude Opus API, Gemini API gateway, DeepSeek API, Cursor API key, Windsurf API, Trae AI API, YesAPI.
