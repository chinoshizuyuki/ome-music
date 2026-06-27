# Troubleshooting

## Windows Blocks the App

Development builds may be unsigned. Windows SmartScreen may warn before running the app. Only continue if you built the app yourself or trust the release source.

## WebView2 Missing

Install Microsoft Edge WebView2 Runtime if the app cannot open its window.

## NetEase or Bilibili Track Cannot Play

Possible reasons:

- Not logged in
- Membership required
- Copyright or region restriction
- Track removed upstream
- Source API unavailable
- Network failure

The app should show an unavailable state rather than crashing.

## Lyrics Do Not Match

Use the lyrics controls to reload, import `.lrc`, or adjust timing. The Curator must not generate fake official lyrics.

## Build Fails

Run:

```bash
npm install
npm run build
cd src-tauri
cargo check
```

If release packaging fails, confirm that Rust, Visual Studio Build Tools, WebView2, and Tauri dependencies are installed.
