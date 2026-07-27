# Cursor Integration with YesAPI

Cursor can use OpenAI-compatible API settings. If your Cursor setup supports a custom OpenAI Base URL, you can point it to YesAPI.

## Required values

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
```

## Setup

1. Open Cursor settings.
2. Go to the model or API provider settings.
3. Find the OpenAI API key or OpenAI-compatible provider section.
4. Set the Base URL to `https://yesapi.online/v1`.
5. Paste your YesAPI API key.
6. Select a supported model from your YesAPI console.
7. Send a short test prompt.

## Test prompt

```text
Reply with one short sentence confirming the API connection works.
```

## Troubleshooting

If Cursor reports an authentication error, confirm the API key is copied correctly.

If Cursor reports a network or endpoint error, confirm the Base URL includes `/v1`.

If a model is unavailable, check whether the model name exists in your YesAPI console.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Base URL setup](../quickstart/base-url-setup.md)
