# Suno V4 5 YesAPI Guide

[中文](#中文版本) | [English](#english-version)

---

> **YesAPI pricing highlight**  
> 中文用户：**¥10.00 支付 → $10.00 平台额度 → 约 $50.00 可用模型价值**  
> Global users: **[中文](#中文版本) | [English](#english-version)

---.50 payment → $10.00 platform credit → about $50.00 usable model value**  
> [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)

<a id="中文版本"></a>

## 中文版本

通过 YesAPI 调用 Suno V4 5，适合语音、音乐、音频生成和内容生产流程。

### 基本信息

| 项目 | 配置 |
| :--- | :--- |
| 官方文档 | [Suno V4 5](https://doc.yesapi.online/suno-v4-5) |
| GitHub 分类 | 音频与音乐模型 |
| Base URL | `https://yesapi.online/v1` |
| 模型名称 | `suno-v4-5` |

### 适用场景

- 在 Cursor、Claude Code、OpenCode、NextChat、LobeChat 或自定义应用中配置 YesAPI。
- 使用一个 API Key 接入多个模型供应商。
- 需要更低成本的开发、测试或自动化调用。

### 快速配置

```text
Base URL: https://yesapi.online/v1
API Key:  你的 YesAPI 密钥
Model:    suno-v4-5
```

### 调用示例

```bash
curl https://yesapi.online/v1/audio/speech \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "suno-v4-5",
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
- [查看原始中文文档](https://doc.yesapi.online/suno-v4-5)

---

<a id="english-version"></a>

## English Version

Use Suno V4 5 through YesAPI for speech, music, audio generation, and content production workflows.

### Basic information

| Item | Value |
| :--- | :--- |
| Official docs | [Suno V4 5](https://doc.yesapi.online/en/suno-v4-5) |
| GitHub category | Audio and Music Models |
| Base URL | `https://yesapi.online/v1` |
| Model name | `suno-v4-5` |

### Use cases

- Configure YesAPI in Cursor, Claude Code, OpenCode, NextChat, LobeChat, or a custom API app.
- Access multiple model providers with one API key.
- Reduce development, testing, and automation cost while keeping an OpenAI-compatible workflow.

### Quick configuration

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
Model:    suno-v4-5
```

### Request example

```bash
curl https://yesapi.online/v1/audio/speech \
  -H "Authorization: Bearer sk-your-yesapi-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "suno-v4-5",
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
- [Open the English source docs](https://doc.yesapi.online/en/suno-v4-5)
