# NoteCanvas v5.26.0 — iPad / iPhone PWA

以 **v5.25.0 完整 ZIP 的實際原始碼**為基礎更新，沿用所有筆記與錄音資料結構。不重製 App。

## 這一版真正完成

- **單一情境工具列**：鋼筆、螢光筆、橡皮擦、套索、文字、圖形、雷射筆等工具，各自顯示自己的設定列；工具主列和情境列在 iPad / iPhone 觸控介面採用獨立橫向捲動，避免溢出裁切。
- **鋼筆快速設定**：情境列前段固定放 3 支現有可編輯常用筆，再放筆型、粗細與獨立色票；細緻筆壓、平滑度與實線／虛線／點線仍可從筆刷面板修改。常用筆切換會套用實際設定，不是示意按鈕。
- **真正的雷射筆模式**：新增線條／圓點兩種模式、大小調整，於獨立暫存繪圖層繪製，抬筆後淡出。雷射筆不寫入筆記筆跡、復原紀錄、匯出檔或 IndexedDB。
- **其他工具情境設定**：橡皮擦的區域／整筆及抬筆切回鋼筆、螢光筆獨立色盤及直線模式、圖形設定、文字工具保留既有事件處理；圖片加入可重開相簿的按鈕，頁面操作選單新增直接進入既有紙張範本的選項。
- **向下相容**：不更改 `NoteCanvasDB`（IndexedDB schema 2）、`books` 或 `audio` store；沿用 `notecanvas.penPresets.v2`、`notecanvas.toolPalettes.v1`、`notecanvas.inkPrefs.v1`，舊筆跡仍用既有算法顯示。新版本號已同步至首頁、網頁標題、PWA manifest、SW cache 與完整 ZIP 名稱。

## 更新前必讀

1. **先在舊版逐本匯出 JSON**，並把重要錄音從錄音管理中各別下載。JSON 備份**不包含錄音**。
2. 完整解壓 ZIP，把其中全部檔案部署至**原本網址**的 GitHub Pages 目錄；保持 `index.html`、`sw.js`、`manifest.webmanifest` 與圖示相對路徑。
3. iPad Safari、iPhone Safari / 主畫面 PWA 重新整理；**不要清除網站資料**，否則本機 IndexedDB 筆記與錄音可能遺失。若離線畫面未更新，先回線上重新載入。

## 驗證範圍

請見 `TEST_REPORT.md`、`QA_IPAD_IPHONE.md`：語法／版本／ZIP、Chromium 觸控模擬與記憶體模擬 IndexedDB 功能測試。**尚未執行真正 iPad + Apple Pencil 或 iPhone Safari / WebKit 實機測試**。瀏覽器 PWA 的筆壓、延遲與防手掌誤觸不能宣稱完全等同 Goodnotes 原生 App。
