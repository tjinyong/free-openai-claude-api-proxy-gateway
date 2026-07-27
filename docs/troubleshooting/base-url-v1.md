# Base URL Must Include /v1

Many OpenAI-compatible clients expect the Base URL to include the API version path.

Use:

```text
https://yesapi.online/v1
```

Do not use this for OpenAI-compatible clients:

```text
yesapi.online
```

## Symptoms

- The client sends requests to the wrong path.
- Chat completion requests fail.
- The tool reports an unexpected response format.
- The API works in one client but fails in another.

## Fix

Open your client settings and set the API Base URL to:

```text
https://yesapi.online/v1
```

Restart the client after saving the setting.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Base URL setup](../quickstart/base-url-setup.md)
