# NoteCanvas v5.26.0 — 驗證紀錄

檢查日期：2026-09-26。以使用者 v5.24.0 原始 ZIP 經驗證的 v5.25.0 完整版為基礎，未更換 IndexedDB schema；完整 ZIP 保留原有 PWA 圖示。

## 實際執行並通過

- **靜態檢查**：HTML 標籤與重複 ID 檢查、主 module／一般 script／Service Worker `node --check`；首頁版本、程式版本、manifest、SW 註冊與 cache、README、ZIP 檔名一致。
- **兩組 Chromium 觸控模擬**：iPad 834 × 1112、iPhone 390 × 844；模擬 localStorage 及 IndexedDB 記憶體操作。測試原有鋼筆 20 個採樣點、筆壓與平滑、常用筆偏好、色盤排序、舊版筆跡渲染、復原重做、閱讀模式回到文件庫、iPad Pencil Only 及 iPhone 手指移動／書寫；兩種版面皆 0 個 JavaScript page error。
- **v5.26 新功能實測**：在兩種觸控版面依序切換 10 種工具，檢查一次只顯示對應情境設定列、選單位於可見範圍；常用筆即時切換、色票、橡皮擦模式、螢光筆設定、圖片情境列和頁面範本選單正常；雷射筆線條與圓點顯示、抬筆後淡出及清除、不儲存成筆跡、不占用復原歷史紀錄。
- **版面**：Chromium 擷圖檢查 iPad、iPhone 介面；iPad 834px 將次要文件功能收至更多選單，避免標題與按鈕字體擠壓；全頁無超出裝置寬度的整頁水平捲動，主工具列及情境設定列可各自左右捲動。
- **資料格式不更動**：`NoteCanvasDB` schema 2／`books`／`audio` 與三組既有本機設定鍵不變；模擬 v5.24 格式筆跡依舊可顯示。
- **封裝**：ZIP 成員全部可讀、manifest 可解析、版本字串同步，兩張 PWA 圖示與 v5.25 逐 byte 相同。

## 尚未執行（不宣稱已通過）

- 真正的 iPad + Apple Pencil（含筆壓、手掌防誤觸、長時間手寫）與 iPhone Safari／WebKit／主畫面 PWA 實機操作。
- 真實 IndexedDB 跨版本 5.25 → 5.26 升級持久性端到端測試：本次執行環境阻擋 Playwright 導覽測試用的虛擬 HTTPS 位址；已以記憶體模擬驗證資料格式與 UI，但**不得把模擬說成真實持久化測試**。
- PWA SW 真實線上／離線更新、麥克風實際錄音、外部 PDF CDN、真實 Safari 上長筆記效能等仍待在使用者裝置上回歸。

更新前請備份每一本 `.notecanvas.json` 及另外下載重要錄音；JSON 不含音檔。不要刪除原網站的 Safari 網站資料。
