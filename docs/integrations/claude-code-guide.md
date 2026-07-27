# Claude Code Guide for YesAPI

Claude Code can be configured with an Anthropic-compatible base URL in environments that support custom provider settings.

## Environment variables

```bash
export ANTHROPIC_BASE_URL="https://yesapi.online/v1"
export ANTHROPIC_AUTH_TOKEN="sk-your-yesapi-key"
export CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1
```

Use the API key from your [YesAPI console](https://yesapi.online?utm_source=github&utm_medium=docs).

## Notes

- Keep the token private.
- Restart Claude Code after changing environment variables.
- If your client expects OpenAI-compatible requests, use `https://yesapi.online/v1` instead.

## Test

Ask Claude Code to run a small read-only task, such as listing files or explaining a short file. If the request completes, the endpoint and token are working.

## Troubleshooting

If authentication fails, generate a new key in the YesAPI console and update `ANTHROPIC_AUTH_TOKEN`.

If the client cannot connect, check whether the tool expects an Anthropic-style base URL or an OpenAI-compatible `/v1` Base URL.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Base URL setup](../quickstart/base-url-setup.md)
