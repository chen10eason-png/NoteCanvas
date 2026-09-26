# NoteCanvas v5.28.0 — Goodnotes-inspired writing page / page management

Based on the user's Goodnotes screen recording and the complete V5.27 ZIP. No original Goodnotes code or brand assets included.

## New
- A touch-first Add Page sheet with insert before/after/end, paper style and color previews, and PDF/image entry points. Existing thumbnail long-menu page copy, paste, reorder, trash and restore remain.
- Separate current-page settings: ruling type, background color, line/grid/dot spacing with live preview; apply current or all non-PDF pages without erasing notes. Existing pages without `rulingSpacing` render exactly as before.
- Page menu: page settings, outline title, clear current page ink and objects (preserving PDF or paper background), with confirmation. Undo is available for the current page through the existing in-memory history.
- Page sidebar may move left/right; preference stays on device. Reading, continuous vertical/horizontal/single page gestures remain unchanged.
- Small-screen touch layouts and mobile page-settings entry under the document menu.

## Safety
Uses unchanged IndexedDB schema and preserves old strokes. Before deploying, export each notebook JSON and download recordings separately; JSON does not contain recordings. Deploy on the existing URL and do not clear Safari website data.

## Limitations
Web Pencil input cannot replicate native Goodnotes palm rejection or latency. Physical iPad/iPhone validation is **not** claimed. Other Goodnotes screen recording menus not implemented here (e.g. OCR PDF scan, system-wide collaboration) are not implied. See TEST_REPORT.md and QA_IPAD_IPHONE.md.
