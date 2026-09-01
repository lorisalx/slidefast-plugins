# Slidefast plugins

Official [Slidefast](https://slidefast.io) plugin for Codex and Claude Code. It connects to the hosted Slidefast MCP server to create, edit, review, export, and publish social carousels.

Authentication uses OAuth 2.1 with Authorization Code and PKCE. Your AI client opens Slidefast sign-in and consent on first use; no API key needs to be stored in a project.

## Codex

```bash
codex plugin marketplace add lorisalx/slidefast-plugins
codex plugin add slidefast@slidefast
```

## Claude Code

```bash
claude plugin marketplace add lorisalx/slidefast-plugins
claude plugin install slidefast@slidefast
```

Run `/reload-plugins` in an existing Claude Code session after installation or an update.

## What is included

- Codex and Claude Code plugin manifests
- Hosted MCP configuration for `https://mcp.slidefast.io/mcp`
- A shared Slidefast workflow skill
- Slidefast brand assets

The Slidefast application source is maintained separately. See the [MCP documentation](https://slidefast.io/docs/mcp), [privacy policy](https://slidefast.io/privacy), and [terms](https://slidefast.io/terms).

## License

MIT
