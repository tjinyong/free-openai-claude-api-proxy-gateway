# Phase 2 Documentation Roadmap

Phase 1 creates a small set of original developer guides. Phase 2 can expand the repository after the first pages are published and reviewed.

## Additional integration guides

- `docs/integrations/nextchat-setup.md`
- `docs/integrations/lobe-chat.md`
- `docs/integrations/langchain-python.md`
- `docs/integrations/dify.md`

## Model guides

- `docs/models/openai-compatible.md`
- `docs/models/claude.md`
- `docs/models/deepseek.md`
- `docs/models/gemini.md`
- `docs/models/qwen.md`

These pages should focus on practical examples, model selection, and client configuration. They should not copy API parameter tables from `doc.yesapi.online`.

## GitHub Pages

After the Markdown guides are stable:

1. Choose MkDocs Material or Docsify.
2. Publish from the repository with GitHub Pages.
3. Generate a sitemap.
4. Submit the sitemap in Google Search Console.

## GitHub Issues for common problems

Create solved issues for real troubleshooting topics:

- 401 Unauthorized
- Missing `/v1` in Base URL
- Stream response ended unexpectedly
- Too many requests
- Model name not found

Each issue should include the symptom, likely cause, and fix. Do not create duplicate or low-quality issues.

## Optional migration script

Only add a migration script if there is a clear source export from `doc.yesapi.online`.

The script should:

- Strip `<script>` and `<style>` blocks.
- Convert HTML to Markdown.
- Preserve code blocks.
- Add a consistent `## Next steps` section.
- Avoid duplicating API reference pages word-for-word.
