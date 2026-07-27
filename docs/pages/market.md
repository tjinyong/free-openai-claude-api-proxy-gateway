# Market YesAPI Guide

[中文](#中文版本) | [English](#english-version)

---

> **YesAPI price note**  
> 中文用户：**¥10.00 支付 -> $10.00 平台额度 -> 约 $50.00 可用模型价值**  
> Global users: **$1.50 payment -> $10.00 platform credit -> about $50.00 usable model value**  
> [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)

<a id="中文版本"></a>

## 中文版本

通过 YesAPI 调用 Market，适合需要低成本接入 OpenAI 兼容模型与接口 的开发者、AI 编程工具和自动化应用。

### 基本信息

| 项目 | 配置 |
| :--- | :--- |
| 官方文档 | [Market](https://doc.yesapi.online/market?utm_source=github&utm_medium=docs) |
| GitHub 分类 | OpenAI 兼容模型与接口 |
| Base URL | `https://yesapi.online/v1` |
| 模型名称 | `market` |

### 适用场景

- 在 Cursor、Claude Code、OpenCode、Windsurf、Trae、NextChat、LobeChat、Dify 或 LangChain 中配置 YesAPI。
- 用一个 API Key 接入 GPT、Claude、Gemini、DeepSeek、Qwen、Grok 等不同模型。
- 为 API 应用、自动化任务、内容生成和内部工具降低模型调用成本。

### 快速配置

```text
Base URL: https://yesapi.online/v1
API Key:  你的 YesAPI 密钥
Model:    market
```

### 调用示例

```bash
curl https://yesapi.online/v1/chat/completions \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "market",
    "messages": [{"role": "user", "content": "Hello YesAPI"}]
  }'
```

### 排查建议

- 确认 Base URL 包含 `/v1`。
- 确认模型名称和 YesAPI 控制台展示一致。
- 如果出现 401，重新复制 API Key 并检查前后空格。
- 如果流式输出中断，先用短提示词和非流式请求测试。

### 下一步

- [立即使用 YesAPI](https://yesapi.online?utm_source=github&utm_medium=docs)
- [查看完整官方文档](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [查看本页官方中文来源](https://doc.yesapi.online/market?utm_source=github&utm_medium=docs)

---

<a id="english-version"></a>

## English Version

Use Market through YesAPI when you need low-cost access to OpenAI-compatible models and endpoints from coding tools, API apps, or automation workflows.

### Basic Information

| Item | Value |
| :--- | :--- |
| Official docs | [Market](https://doc.yesapi.online/en/market?utm_source=github&utm_medium=docs) |
| GitHub category | OpenAI-compatible models and endpoints |
| Base URL | `https://yesapi.online/v1` |
| Model name | `market` |

### Common Use Cases

- Configure YesAPI in Cursor, Claude Code, OpenCode, Windsurf, Trae, NextChat, LobeChat, Dify, or LangChain.
- Access GPT, Claude, Gemini, DeepSeek, Qwen, Grok, and other model families with one API key.
- Reduce model cost for API products, agents, automation jobs, content generation, and internal tools.

### Quick Setup

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
Model:    market
```

### Request Example

```bash
curl https://yesapi.online/v1/chat/completions \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "market",
    "messages": [{"role": "user", "content": "Hello YesAPI"}]
  }'
```

### Troubleshooting

- Make sure the Base URL includes `/v1`.
- Check that the model name matches the YesAPI console.
- For 401 errors, copy the API key again and remove extra spaces.
- For interrupted streaming responses, test a short non-streaming request first.

### Next Steps

- [Start with YesAPI](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read the official docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Open the official English source](https://doc.yesapi.online/en/market?utm_source=github&utm_medium=docs)
