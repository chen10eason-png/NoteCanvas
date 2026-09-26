# Goodnotes research log — verified starting set

This is a source inventory, not a claim that all content has been watched, tested, or implemented. Source availability and app version may change. Target: 100+ distinct sources; **not yet reached**.

## Official Goodnotes feature documentation
1. [Manage writing-tool color presets](https://support.goodnotes.com/hc/en-us/articles/7353743265039-Add-and-manage-writing-tool-color-presets) — 12 colors/tool, edit/reorder/reset.
2. [Pen tool](https://support.goodnotes.com/hc/en-us/articles/7353756785679-Write-and-customize-ink-with-the-Pen-tool) — stroke presets, pen styles.
3. [Customize toolbar](https://support.goodnotes.com/hc/en-us/articles/8900755183631-Customize-the-toolbar) — toolbar configuration.
4. [Eyedropper](https://support.goodnotes.com/hc/en-us/articles/8061582993423-Find-the-perfect-color-with-the-Eyedropper-Color-Picker) — document color picking.
5. [Separate color palettes](https://support.goodnotes.com/hc/en-us/articles/17476182494479-Why-don-t-color-palettes-sync-across-writing-tools) — tool-specific palettes.
6. [Pencil tool](https://support.goodnotes.com/hc/en-us/articles/10730874907023-Create-lively-drawings-with-the-Pencil-tool) — pencil customization.
7. [Lasso](https://support.goodnotes.com/hc/en-us/articles/7353695644175-Select-Move-and-Edit-Content-With-the-Lasso-Tool) — selection and movement.
8. [Eraser](https://support.goodnotes.com/hc/en-us/articles/7353718249231-Erase-handwriting-and-page-content-with-the-Eraser-tool) — precision/standard/stroke erasers.
9. [Folders and documents](https://support.goodnotes.com/hc/en-us/articles/15303674514191-Organize-folders-and-documents-in-Goodnotes) — library.
10. [Sidebar](https://support.goodnotes.com/hc/en-us/articles/9497798035983-Use-the-Sidebar-to-navigate-your-document) — page thumbnails and bookmarks.
11. [Outlines](https://support.goodnotes.com/hc/en-us/articles/7353757101071-Create-and-manage-document-outlines) — hierarchy and navigation.
12. [Highlighter](https://support.goodnotes.com/hc/en-us/articles/7353718215823-Using-the-Highlighter-tool) — stroke settings.
13. [Export](https://support.goodnotes.com/hc/en-us/articles/7353742824975-Export-documents-or-pages) — formats.
14. [Import](https://support.goodnotes.com/hc/en-us/articles/7353717816463-Import-files-into-Goodnotes) — supported formats.
15. [Library deletion](https://support.goodnotes.com/hc/en-us/articles/7353743683599-Delete-documents-notebooks-and-folders-from-your-library) — trash.
16. [Move documents](https://support.goodnotes.com/hc/en-us/articles/7353712019599-Move-documents-and-folders-in-your-Goodnotes-library) — drag/drop and move.
17. [Backups](https://support.goodnotes.com/hc/en-us/articles/7352786555279-How-to-Set-Up-Auto-Backup-in-Goodnotes) — automatic backups.
18. [Backup zip](https://support.goodnotes.com/hc/en-us/articles/7353742233359-I-cannot-view-the-Goodnotes-backup-zip-file-on-my-computer) — restore.

## Independent video walkthroughs
19. [Paperless Lab, Ultimate GoodNotes 2026 Tutorial](https://www.youtube.com/watch?v=-2sb0a5g_no) — comprehensive chapter list for UI, library, tools, page management, whiteboard.
20. [Acchan, Goodnotes 2026 complete guide](https://www.youtube.com/watch?v=A4tq8OOezXg) — timestamped walkthrough for pen, highlighter, lasso, pages, export and PDF.

## v5.25.0 增補：9 份不同的 Goodnotes 官方來源（總目錄 29 份）

以下 21–29 是新增的**不同頁面**；既有的 1–20 保留作為延續參考。檢查日期 2026-09-26；「讀過全文」及「搜尋結果摘要已核對」分開記錄，不將頁面清單等同於完整分析。

21. [Improved User Interface](https://support.goodnotes.com/hc/en-us/articles/13682253498767-Improved-User-Interface) — **已閱讀全文**；新版文件頁分頁、導覽列、情境工具選單，iPhone 的次級操作應收進易觸控的選單。v5.25.0 落實小螢幕次級操作入口；通用物件選單尚待規劃。
22. [Write with the Zoom Window](https://support.goodnotes.com/hc/en-us/articles/7353756826383-Write-with-the-Zoom-Window) — **已核對官方摘要**；局部放大手寫、Auto-Advance、換行距離。NoteCanvas 目前只有整頁雙指縮放，尚無獨立 Zoom Window。
23. [Apple Pencil Pro: Squeeze and Barrel Roll](https://support.goodnotes.com/hc/en-us/articles/9757771783823-Utilize-the-new-features-of-Apple-Pencil-Pro) — **已核對官方摘要**；Pencil Pro 擠壓叫出工具及旋轉控制筆觸。Web/PWA 無法假定可以取得同等硬體事件；尚未實作。
24. [Configure palm rejection](https://support.goodnotes.com/hc/en-us/articles/7353727026959-Configure-palm-rejection-for-comfortable-writing) — **已核對官方摘要**；可按書寫姿勢和靈敏度調整防掌誤觸。NoteCanvas iPad 預設限制 Pencil 落筆，並不等於原生 Goodnotes 防掌誤觸演算法。
25. [Zoom, pan, and scroll](https://support.goodnotes.com/hc/en-us/articles/6554036735631-Zoom-pan-and-scroll-through-pages-in-Goodnotes) — **已核對官方摘要**；單指平移、雙指縮放、上下／左右捲動。NoteCanvas 已有連續捲動與縮放；需繼續實機比較邊界情況。
26. [Apple Pencil compatibility](https://support.goodnotes.com/hc/en-us/articles/7353710962575-Check-Apple-Pencil-compatibility-with-your-iPad-and-Goodnotes) — **已核對官方摘要**；各代 Pencil 需要匹配 iPad 硬體；不可把支援 Pointer Events 誤稱為所有 Pencil 機型均通過測試。
27. [Convert handwriting to text](https://support.goodnotes.com/hc/en-us/articles/7353695997199-Convert-handwriting-to-text) — **已核對官方摘要**；以套索選取字跡轉文字。NoteCanvas 套索有，但 OCR 尚未實作。
28. [Unexpected Pencil lines](https://support.goodnotes.com/hc/en-us/articles/360001872735-Why-do-random-lines-appear-while-writing-with-Apple-Pencil) — **已核對官方摘要**；需排除筆尖、配對、保護貼及誤觸因素。供實機 QA 排錯。
29. [Troubleshoot Pencil issues](https://support.goodnotes.com/hc/en-us/articles/360001472956-Troubleshoot-Apple-Pencil-issues-in-Goodnotes) — **已核對官方摘要**；筆尖鬆動、電量、重新配對等排錯路徑。供實機 QA 使用，非程式能解決的硬體情況。

## v5.25.0 實作對照（另重新閱讀既有來源 1、2）

| 官方操作 | 本版實際狀態 | 尚存差異 |
| --- | --- | --- |
| 再點鋼筆開啟設定、鋼筆／原子筆／畫筆 | 已有可操作筆刷面板，線寬、筆壓、穩定度與線型會影響新筆跡 | 尖端銳利度、筆尖扁平度、Draw-and-Hold 智能幾何辨識尚未做 |
| 寫字工具各有獨立色盤 | 維持鋼筆與螢光筆獨立色盤；增設選色格左右移動 | 目前未涵蓋官方所有工具的色盤和拖曳排序手勢 |
| Apple Pencil 單獨落筆；手指移動／捏合 | iPad 預設 Pencil only；iPhone 預設觸控書寫，設有手動切換移動鍵 | 依賴 Web Pointer/Touch Events，尚未在實體 iOS Safari 實測 |
| 進行中筆畫快速顯示 | 完成筆跡快取＋每幀預覽，避免每次 Pointer Move 重畫歷史筆跡 | 仍會重畫進行中的完整筆畫；未經長篇手寫效能基準測試 |

**研究里程碑：29 / 100 個不同來源已列入追蹤，其中本次新增 9 篇有紀錄的官方文章。未宣稱已完整研讀 29 篇，更未達成 100 篇完整分析。**

## Implementation tracking
- Implemented in v5.15: clearly labeled Manage Favorite Pens, per-pen Use/Edit buttons, explicit save-vs-temporary action, independent pen/highlighter color palettes inherited from v5.14.
- At v5.15, not yet verified or implemented: all latest Goodnotes features, 100-source research milestone, Apple Pencil hardware regression, true iCloud sync, audio recording (subsequently added in **v5.21**), native handwriting OCR, proprietary AI features.

- Implemented in v5.18: page-template chooser, per-page and non-PDF bulk apply, page number jump, typed-text/outline/page-number navigation. Handwriting OCR remains unavailable.

## v5.24 iOS 優先方向
移除桌面快捷鍵；iPad/iPhone 提供易點擊的復原、重做、鋼筆、橡皮擦。後續需以實機核對 Goodnotes 手勢與書寫反應，不聲稱已完全相同。

## v5.26.0 的使用者實拍影片參考（與官方研究數目分開）

- 2026-09-26 使用者錄製約 70 秒 Goodnotes 工具操作：實際看到隨工具變更的次設定列、鋼筆／螢光筆／橡皮擦設定、雷射筆線條／圓點。對照文件：`VIDEO_COMPARISON.md`。此為 1 份使用者影片，**不**冒充新分析的官方文件。
