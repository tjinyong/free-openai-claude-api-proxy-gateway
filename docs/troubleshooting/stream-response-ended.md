# Stream Response Ended Unexpectedly

Some AI clients show errors such as "response ended unexpectedly" or "stream interrupted" when a streaming request is cut off before completion.

## First checks

1. Confirm the Base URL includes `/v1`:

```text
https://yesapi.online/v1
```

2. Confirm the API key is valid.
3. Test a short prompt.
4. Test a non-streaming request if your client supports it.

## Cloudflare cache rule

API requests should bypass cache. If you use Cloudflare, make sure API paths are not cached.

Recommended bypass paths:

```text
/v1/*
/responses/*
/api/*
```

## Client-side checks

- Restart the client after changing provider settings.
- Confirm the selected model exists in your YesAPI console.
- Reduce the test prompt size.
- Check whether the client supports SSE streaming with custom endpoints.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [OpenCode setup](../integrations/opencode-setup.md)
