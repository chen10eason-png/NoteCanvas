# NoteCanvas v5.28.0 — validation

## Verified in this environment
- Node `--check` succeeds on both inline JavaScript blocks and Service Worker.
- HTML parsed and all `id` attributes are unique.
- Static integration checks: page insertion controls, paper settings, spacing applied both to live page CSS and exported image canvas, sidebar preference handler, page action handlers, and existing IndexedDB v2 schema remain present.
- Version synchronized across HTML / JS, manifest and service worker cache; ZIP CRC validated.

## Unverified
- Automated Chromium touch flow attempted but blocked by environment (`net::ERR_BLOCKED_BY_ADMINISTRATOR` for localhost). A green browser end-to-end test cannot be claimed.
- Actual iPad Safari, iPhone Safari and Apple Pencil writing / palm rejection / performance have not been physically tested.

## Known limitations
- Page rendering remains fixed at 768 × 1024 internal pixels, so this release does not introduce landscape canvas, page size conversion, or native Goodnotes PDF/scan services.
- Applying a new page template does not reposition existing strokes. For PDF-backed pages, the original PDF image is retained and background editing is disabled.
- When clearing the currently selected page via its menu, Undo remains available in the existing in-memory current-page history; clearing a different page is not Undo-enabled.
