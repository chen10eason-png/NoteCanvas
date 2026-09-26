# NoteCanvas V5.29.0 — test report

## Executed checks
- JavaScript module parsed using `node --check` (PASS).
- Manifest, HTML title/version, in-app version, service worker cache name and registration URL all updated to V5.29.0 (PASS).
- Six paper options, eight preset colors, three swipe modes, Quick Duplicate, Add Matching Page and Thumbnails controls present in DOM and have JS handlers (static PASS).
- Cornell / margin paper patterns implemented both in CSS and `composePage()` export renderer (static PASS).
- ZIP content checksum and integrity tested (PASS).

## Not tested
- Chromium smoke run timed out in this container, so browser touch interactions are NOT claimed as tested.
- No real iPad, iPhone, Apple Pencil or Safari validation performed.

## Known constraints
- Existing page canvas is 768 × 1024; true A-series paper size/landscape page changes still pending.
- PDF-backed pages preserve PDF backgrounds; paper settings do not overwrite them.
- Export notebook JSON backups and download recordings separately before upgrading.
