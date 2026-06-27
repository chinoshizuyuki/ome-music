# Ome Music

A small, immersive desktop music player with NetEase Cloud Music, Bilibili atmosphere video, emotional danmaku, synced lyrics, and a private music curator experience.

Ome Music is built for local-first listening: the player opens quickly, keeps personal data on your device by default, and hides technical configuration behind a calm music-focused interface.

## Highlights

- Immersive Apple Music-inspired player UI
- Local music import and playback
- NetEase Cloud Music source integration
- Bilibili music/video source integration
- Bilibili video atmosphere layer
- Global ambient danmaku layer
- Synced lyrics with offset adjustment
- Lightweight settings system
- Private DJ / Curator panel
- SQLite local library and listening history
- Tauri-based Windows desktop packaging

## Screenshots

Safe public screenshots are not included yet. Add sanitized images later under:

- `docs/assets/screenshot-main.png`
- `docs/assets/screenshot-settings.png`
- `docs/assets/screenshot-bilibili-atmosphere.png`

Do not commit screenshots that reveal accounts, cookies, private playlists, local paths, or personal listening history.

## Download

For normal use, download the Windows release package from GitHub Releases when available.

Local release builds produce:

- Portable app: `release/Ome Music.exe`
- Installer: `release/Ome Music Setup.exe`

Release binaries are ignored by Git and should be uploaded through GitHub Releases, not committed to the repository.

## Development

### Requirements

- Windows 10/11
- Node.js
- Rust stable toolchain
- Tauri CLI through `@tauri-apps/cli`
- Microsoft Edge WebView2 Runtime

### Install

```bash
npm install
```

### Run Web Frontend

```bash
npm run dev
```

### Run Desktop App

```bash
npm run desktop
```

### Build Frontend

```bash
npm run build
```

### Build Windows Release

```bash
npm run release:windows
```

Tauri will build the frontend from `dist` and package the app without requiring a development server.

## Configuration

Ome Music does not include built-in API keys, cookies, passwords, or tokens.

Configure sources inside the app:

- NetEase Cloud Music: API base URL, login session, optional cookie import
- Bilibili: public search, optional login session/cookie for account-only content
- Curator/API: OpenAI-compatible provider name, base URL, API key, model
- Voice: optional speech-to-text and text-to-speech providers

See [docs/CONFIGURATION.md](docs/CONFIGURATION.md).

## Privacy

- Local music files are referenced by path and are not uploaded.
- Local audio files are not copied into the application directory.
- API keys and source credentials should be stored only on the user's local machine.
- SQLite is used for local metadata, playback history, preferences, lyrics cache, and small text records.
- Do not commit databases, cookies, tokens, logs, caches, screenshots, or release binaries.

See [docs/PRIVACY.md](docs/PRIVACY.md).

## Disclaimer

This project is for personal learning and local music experience only.

Ome Music does not provide, host, store, or distribute copyrighted music. NetEase Cloud Music, Bilibili, and any third-party content remain the property of their respective platforms and rights holders. Users are responsible for complying with applicable laws and each platform's terms of service.

## Security

If you discover a security issue, do not open a public issue with secrets or exploit details. See [SECURITY.md](SECURITY.md).

## License

Ome Music is released under the MIT License. See [LICENSE](LICENSE).
