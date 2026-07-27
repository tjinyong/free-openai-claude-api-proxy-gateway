# Get a YesAPI API Key

You need a YesAPI API key before using the OpenAI-compatible endpoint.

## Steps

1. Open the [YesAPI console](https://yesapi.online?utm_source=github&utm_medium=docs).
2. Sign in or create an account.
3. Open the API key page.
4. Create or copy your API key.
5. Use it with this Base URL:

```text
https://yesapi.online/v1
```

## Keep your key private

Do not commit real API keys to GitHub, public chat logs, screenshots, or shared config files.

Use environment variables when possible:

```bash
export OPENAI_API_KEY="sk-your-yesapi-key"
export OPENAI_BASE_URL="https://yesapi.online/v1"
```

For Windows PowerShell:

```powershell
$env:OPENAI_API_KEY="sk-your-yesapi-key"
$env:OPENAI_BASE_URL="https://yesapi.online/v1"
```

## Test with curl

```bash
curl https://yesapi.online/v1/models \
  -H "Authorization: Bearer sk-your-yesapi-key"
```

If the key is valid, the response should not be a 401 authentication error.

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Base URL setup](base-url-setup.md)
