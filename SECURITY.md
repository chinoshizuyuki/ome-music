# Security Policy

## Supported Versions

Ome Music is currently pre-release. Security fixes are handled on the main development line.

## Reporting a Vulnerability

Please do not publish API keys, cookies, tokens, passwords, private account data, or exploit details in a public issue.

Report privately to the maintainer first. Include:

- A short description of the issue
- Affected version or commit
- Steps to reproduce without exposing secrets
- Suggested mitigation, if known

## Secret Handling Rules

- Do not commit `.env` files.
- Do not commit SQLite databases.
- Do not commit cookies, tokens, or API keys.
- Do not commit logs or diagnostics that include request headers.
- Do not commit screenshots showing account state or personal playlists.
