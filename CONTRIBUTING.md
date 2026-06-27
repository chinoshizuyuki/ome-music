# Contributing

Thanks for helping improve Ome Music.

## Development

```bash
npm install
npm run build
npm run desktop
```

For release packaging:

```bash
npm run release:windows
```

## Before Opening a Pull Request

- Keep changes focused.
- Do not commit build output, release binaries, logs, caches, databases, or personal config.
- Do not include real API keys, cookies, tokens, passwords, local paths, or private account data.
- Run `npm run build`.
- Run `cargo check` in `src-tauri` when Rust code changes.

## Design Direction

Ome Music should stay small, immersive, calm, and music-first. Avoid turning the interface into a dashboard or technical control panel.
