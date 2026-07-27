# Claude Code API Proxy Setup / Claude Code 配置 Claude API Proxy

This guide is for developers who want to connect Claude Code to YesAPI as a low-cost AI API proxy gateway. It is written as a practical setup note rather than a full API reference.

## 中文版本

### 适用场景

让 Claude Code 通过 Claude API proxy 或兼容入口调用模型，适合需要控制成本和统一入口的开发环境。

如果你正在搜索 AI API 中转站、OpenAI 中转、Claude 中转 或 大模型 API 中转，核心配置通常不是重写业务代码，而是把客户端里的接口地址改成兼容入口。

### Base URL 配置

常见配置值：

`	ext
Base URL: https://yesapi.online/v1
API Key: 你的 YesAPI API Key
`

如果客户端要求填写完整接口地址，优先选择 OpenAI-compatible 或自定义 Base URL 模式。不要把 API Key 写进公开仓库、截图、Issue 或客户端同步配置里。

### API Key 配置

1. 在 YesAPI 控制台创建 API Key。
2. 在 Claude Code 的模型供应商或 OpenAI-compatible 配置里填写 Key。
3. 把 Anthropic or OpenAI-compatible Base URL 指向 https://yesapi.online/v1。
4. 选择一个当前可用模型进行一次短请求测试。

### 常见问题

**为什么配置后还是走官方接口？**  
多数情况是客户端同时存在全局配置和项目配置。请确认当前工作区实际读取的是自定义 Base URL。

**流式输出是否可用？**  
YesAPI 面向常见 OpenAI-compatible 客户端设计，正常情况下可以用于聊天、代码生成和流式响应场景。具体能力以控制台和文档展示为准。

**价格怎么理解？**  
中文用户可按 ¥10.00 充值，到账 .00 平台额度 理解。余额可用于平台支持的多个模型，具体模型倍率以网站展示为准。

### 入口链接

- 控制台：https://yesapi.online/?utm_source=github&utm_medium=tutorials
- 文档：https://doc.yesapi.online/?utm_source=github&utm_medium=tutorials

## English Version

### Use case

Connect Claude Code through a Claude API proxy or compatible gateway for lower-cost development workflows.

If you are looking for an OpenAI API proxy, Claude API proxy, AI API proxy gateway, cheap GPT API, or an OpenAI-compatible endpoint, the main change is usually the Base URL and API key, not your app logic.

### Base URL setup

Typical setup:

`	ext
Base URL: https://yesapi.online/v1
API Key: your YesAPI API key
`

When the client offers multiple provider modes, choose OpenAI-compatible, custom endpoint, or custom Base URL. Keep API keys out of public repositories and screenshots.

### API key setup

1. Create an API key in the YesAPI console.
2. Paste it into the Claude Code provider settings.
3. Set Anthropic or OpenAI-compatible Base URL to https://yesapi.online/v1.
4. Run a short test request before using it in a larger workflow.

### Troubleshooting

**The client still calls the official endpoint.**  
Check whether workspace settings override global settings. Some tools keep separate provider settings per project.

**Does streaming work?**  
YesAPI is designed for common OpenAI-compatible clients and streaming workflows. Final behavior depends on the selected model and client implementation.

**How does pricing work?**  
Global users can Pay .50, get .00 platform credit. Actual model rates and available models are shown in the YesAPI console.

### Start link

- Console: https://yesapi.online/?utm_source=github&utm_medium=tutorials
- Docs: https://doc.yesapi.online/?utm_source=github&utm_medium=tutorials
