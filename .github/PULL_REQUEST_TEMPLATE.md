## Summary

<!-- What does this PR do? Keep it focused and small. -->
<!-- 这个 PR 做了什么？保持聚焦，一次改一件事。 -->

## Changes

- 

## Checklist

### Frontend (always)
- [ ] `npm run lint` passes
- [ ] `npm run format:check` passes
- [ ] `npx tsc --noEmit` passes
- [ ] `npm run build` passes

### Rust / Tauri backend (if changed)
- [ ] `cargo check` in `src-tauri` passes
- [ ] `cargo fmt --all -- --check` passes
- [ ] `cargo clippy --workspace -- -D warnings` passes

### UI (if changed)
- [ ] Light glass aesthetic preserved (spacing, radii, no jitter)
- [ ] Window size stable, no overflow or scroll issues
- [ ] Playwright screenshots attached
<!-- Drag screenshots here or paste links -->

## Product principles check

- [ ] No large new dependencies added (ask before adding any)
- [ ] No duplicate settings or over-engineered architecture
- [ ] Listening experience improved, not cluttered with controls

## Safety

- [ ] No build output, binaries, logs, caches, or databases committed
- [ ] No API keys, tokens, cookies, passwords, or personal config committed
- [ ] No destructive operations (delete, migrate, bulk cleanup)

## Related Issues

Closes #
