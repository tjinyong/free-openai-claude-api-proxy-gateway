# GPT 5 4 Mini YesAPI Guide

[中文](#中文版本) | [English](#english-version)

---

<a id="中文版本"></a>

## 中文版本

在兼容 OpenAI 的客户端中调用 GPT 5 4 Mini，适合聊天、推理、代码和 Agent 工作流。

### 基本信息

| 项目 | 配置 |
| :--- | :--- |
| 官方文档 | [GPT 5 4 Mini](https://doc.yesapi.online/gpt-5-4-mini) |
| GitHub 分类 | 对话与推理模型 |
| Base URL | `https://yesapi.online/v1` |
| 模型名称 | `gpt-5-4-mini` |

### 适用场景

- 在 Cursor、Claude Code、OpenCode、NextChat、LobeChat 或自定义应用中配置 YesAPI。
- 使用一个 API Key 接入多个模型供应商。
- 需要更低成本的开发、测试或自动化调用。

### 快速配置

```text
Base URL: https://yesapi.online/v1
API Key:  你的 YesAPI 密钥
Model:    gpt-5-4-mini
```

### 调用示例

```bash
curl https://yesapi.online/v1/v1/chat/completions \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-5-4-mini",
    "messages": [{"role": "user", "content": "Hello YesAPI"}]
  }'
```

### 排查建议

- 确认 Base URL 包含 `/v1`。
- 确认模型名称与 YesAPI 控制台展示一致。
- 如果出现 401，重新复制 API Key 并检查前后空格。
- 如果流式输出中断，先用短提示词和非流式请求测试。

### Next steps

- [打开 YesAPI 控制台](https://yesapi.online?utm_source=github&utm_medium=docs)
- [查看完整官方文档](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [查看原始中文文档](https://doc.yesapi.online/gpt-5-4-mini)

---

<a id="english-version"></a>

## English Version

Use GPT 5 4 Mini through YesAPI for chat, reasoning, coding, and agent workflows with an OpenAI-compatible client.

### Basic information

| Item | Value |
| :--- | :--- |
| Official docs | [GPT 5 4 Mini](https://doc.yesapi.online/en/gpt-5-4-mini) |
| GitHub category | Chat and Reasoning Models |
| Base URL | `https://yesapi.online/v1` |
| Model name | `gpt-5-4-mini` |

### Use cases

- Configure YesAPI in Cursor, Claude Code, OpenCode, NextChat, LobeChat, or a custom API app.
- Access multiple model providers with one API key.
- Reduce development, testing, and automation cost while keeping an OpenAI-compatible workflow.

### Quick configuration

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
Model:    gpt-5-4-mini
```

### Request example

```bash
curl https://yesapi.online/v1/v1/chat/completions \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-5-4-mini",
    "messages": [{"role": "user", "content": "Hello YesAPI"}]
  }'
```

### Troubleshooting

- Make sure the Base URL includes `/v1`.
- Make sure the model name matches the YesAPI console.
- If you see a 401 error, copy the API key again and remove extra spaces.
- If streaming ends unexpectedly, test a short prompt and then a non-streaming request.

### Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full official docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Open the English source docs](https://doc.yesapi.online/en/gpt-5-4-mini)
