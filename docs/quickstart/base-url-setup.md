# Configure YesAPI Base URL

Most OpenAI-compatible tools allow you to change the API endpoint without rewriting your app. For YesAPI, use this Base URL:

```text
https://yesapi.online/v1
```

## When to use this

Use this guide when your tool asks for one of these fields:

- Base URL
- API Base
- OpenAI Base URL
- OpenAI Compatible Endpoint
- Custom API Endpoint

## Required values

```text
Base URL: https://yesapi.online/v1
API Key:  your YesAPI key
```

Get your key from the [YesAPI console](https://yesapi.online?utm_source=github&utm_medium=docs).

## Python example

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-your-yesapi-key",
    base_url="https://yesapi.online/v1",
)

response = client.chat.completions.create(
    model="gpt-5.6-sol",
    messages=[{"role": "user", "content": "Hello YesAPI"}],
)

print(response.choices[0].message.content)
```

## TypeScript example

```typescript
import OpenAI from "openai";

const openai = new OpenAI({
  apiKey: "sk-your-yesapi-key",
  baseURL: "https://yesapi.online/v1",
});

const completion = await openai.chat.completions.create({
  model: "gpt-5.6-sol",
  messages: [{ role: "user", content: "Hello YesAPI" }],
});

console.log(completion.choices[0].message.content);
```

## Common mistake

Do not use only the domain for OpenAI-compatible clients:

```text
yesapi.online
```

Use:

```text
https://yesapi.online/v1
```

## Next steps

- [Open YesAPI Console](https://yesapi.online?utm_source=github&utm_medium=docs)
- [Read full docs](https://doc.yesapi.online?utm_source=github&utm_medium=docs)
- [Get an API key](get-api-key.md)
