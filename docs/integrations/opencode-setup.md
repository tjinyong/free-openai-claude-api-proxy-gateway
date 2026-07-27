# OpenCode Setup with YesAPI

OpenCode can use an OpenAI-compatible provider configuration. Set the base URL to the YesAPI `/v1` endpoint.

## Example configuration

```json
{
  "provider": {
    "openai": {
      "options": {
        "baseURL": "https://yesapi.online/v1",
        "apiKey": "sk-your-yesapi-key"
      },
      "models": {
        "gpt-5.6-sol": {
          "name": "GPT-5.6 Sol"
        }
      }
    }
  }
}
```

## Checklist

- `baseURL` includes `/v1`.
- `apiKey` uses your YesAPI key.
- The model name exists in your YesAPI console.
- The client is restarted after config changes.

## Troubleshooting

If OpenCode says the response ended unexpectedly, test a non-streaming request first and confirm API paths bypass cache.

If OpenCode cannot find models, verify the configured model names match the names exposed by YesAPI.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Stream response troubleshooting](../troubleshooting/stream-response-ended.md)
