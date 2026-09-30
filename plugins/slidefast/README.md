# Slidefast

Slidefast turns a brief into an on-brand carousel for LinkedIn, Instagram, or TikTok. This plugin lets your AI assistant create and edit carousels in your Slidefast account, apply your themes and brand kit, collect client feedback through review links, export PDF or PNG files, and publish to the social accounts you connected in Slidefast.

## What you need

A Slidefast account. Sign up at [slidefast.io](https://slidefast.io). AI generation, exports, review links, and publishing follow your plan's limits.

## Install

Claude Code:

```bash
claude plugin marketplace add lorisalx/slidefast-plugins
claude plugin install slidefast@slidefast
```

Codex:

```bash
codex plugin marketplace add lorisalx/slidefast-plugins
codex plugin add slidefast@slidefast
```

On first use, your client opens a Slidefast page in the browser: sign in and approve the access. No API key to copy.

## What the plugin contains and what it connects to

- `skills/slidefast/SKILL.md`: instructions that teach the assistant the Slidefast workflow (project scope, dry-run edits before applying, confirmation before publishing).
- `.mcp.json`: one remote MCP server, `https://mcp.slidefast.io/mcp`, operated by Slidefast. The plugin runs no local code, hooks, or scripts.

Sign-in uses OAuth 2.1 with PKCE. The assistant sends the requests you ask for (briefs, slide text, image choices, export and publish commands) to that server, which acts on your Slidefast account through the Slidefast API. Your carousels, themes, and images stay in your Slidefast account. Social media credentials never pass through the plugin: you connect LinkedIn, Instagram, Facebook, or TikTok in the Slidefast web app.

## Good to know

- Edits to an existing carousel come back as suggestions first; nothing changes until you accept.
- Export links are public CDN URLs: anyone with the link can open the file.
- Publishing to LinkedIn, Meta, or TikTok direct post goes live. The assistant asks you to confirm the platform and account right before it publishes.

## Links

- Documentation: [slidefast.io/docs/mcp](https://slidefast.io/docs/mcp)
- Support: hello@slidefast.io
- Privacy policy: [slidefast.io/privacy](https://slidefast.io/privacy)
- Terms: [slidefast.io/terms](https://slidefast.io/terms)

## License

MIT
