# Configuration

Ome Music is local-first. It does not ship with provider keys, cookies, or account credentials.

## Music Sources

### Local Music

Use the app to choose a local music folder. Ome Music stores file paths and metadata in SQLite. It does not copy your songs into the app directory.

### NetEase Cloud Music

Supported configuration:

- Enable/disable source
- API base URL
- QR/login session
- Optional cookie import
- Playback quality preference

Some tracks may still be unavailable because of copyright, region, membership, account permission, or upstream API limitations.

### Bilibili

Supported configuration:

- Enable/disable source
- API base URL
- Search scope
- QR/login session
- Optional cookie import

Bilibili video atmosphere and danmaku are loaded only when Bilibili content is played.

## Curator/API

The Curator uses an OpenAI-compatible provider configuration:

- Provider name
- Base URL
- API key
- Model

The API key must be entered by the user and stored locally. Do not commit it.

## Voice

Speech-to-text and text-to-speech are optional. If no voice provider is configured, the Curator falls back to text.
