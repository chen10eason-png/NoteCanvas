# NoteCanvas v5.25.0 — iPad / iPhone PWA

專為 iPad（Apple Pencil 書寫、手指移動與雙指縮放）及 iPhone（觸控優先）打造的個人筆記 PWA。這一版以使用者提供的 **v5.24.0 ZIP 原始碼**為基礎更新；不是重做專案。

## v5.25.0 更新

- **鋼筆書寫預覽效能**：開始書寫時快取既有筆跡；書寫中由 `requestAnimationFrame` 排程繪製「既有筆跡快取＋當前筆跡」，不再每次 Pencil 移動都重畫全部歷史筆跡。保留共同的筆跡渲染函式與既有筆記資料。
- **筆刷設定面板**：實際選取鋼筆、原子筆、畫筆；調整線寬、實線／虛線／點線、筆壓敏感度與筆跡穩定度。Pencil 筆壓數值由 Pointer Events 讀取；穩定度對新採樣點套用平滑演算法。對舊筆跡繼續採用原有渲染方式。
- **常用筆**：既有 3 支可編輯常用筆，增加各支的筆壓及穩定度設定；點選後真正套用於接下來的筆跡。維持 v2 常用筆偏好儲存鍵，舊設定可讀取。
- **色盤**：維持鋼筆／螢光筆各自獨立的顏色組，新增觸控式「選取色格→左移／右移」排序，不必依賴滑鼠拖曳或鍵盤。
- **觸控介面**：iPad／iPhone 書寫操作列、主工具列、次工具列的排列與水平捲動修正；iPhone 的錄音、學習卡片、跳頁、匯出與閱讀模式收進「•••」選單。iPhone 預設可手指書寫，可切「✋ 移動」；iPad 預設僅 Pencil 書寫，手指負責導覽。返回文件庫時自動離開閱讀模式。

## 安裝與更新

將 ZIP **完整解壓**後，將其中全部檔案部署至原本網站（例如 GitHub Pages 的發佈目錄）。保留檔名及相對路徑：`index.html`、`manifest.webmanifest`、`sw.js` 與圖示缺一不可。HTTPS 部署後，可在 Safari 使用「加入主畫面」。如畫面仍顯示舊版，先重新整理，必要時移除舊 PWA 主畫面捷徑後重新加入；**不要清除網站資料**，否則本機筆記和錄音可能消失。

### 資料相容與備份

- 仍採用 `NoteCanvasDB`、IndexedDB schema **2**，沿用 `books`／`audio` 兩個 object store；不執行破壞性的資料轉換或資料庫清空。
- 現有常用筆偏好 `notecanvas.penPresets.v2` 與色盤偏好 `notecanvas.toolPalettes.v1` 沿用；新筆壓／平滑偏好另外儲存在 `notecanvas.inkPrefs.v1`。
- 更新前，請在**舊版**逐本匯出 `.notecanvas.json` 備份並留在裝置以外的位置。**JSON 不包含錄音檔**：錄音獨立存在 IndexedDB `audio`；若有重要錄音，請在錄音管理中逐段下載備份。
- 不要以另一個網域或不同的 GitHub Pages 網址取代原網址並期待原有本機筆記自動出現；瀏覽器儲存按來源網址分隔。

## 測試與限制

程式已進行 JavaScript 語法、HTML／manifest／Service Worker 版本一致性、ZIP 完整性檢查，並以 Chromium 觸控模擬、**記憶體模擬 IndexedDB** 測試 iPad/iPhone 佈局、筆壓儲存、筆畫、復原／重做、常用筆與色盤。詳見 `TEST_REPORT.md` 與 `QA_IPAD_IPHONE.md`。

**尚未在實體 iPad/iPhone 及 Safari／WebKit 上完成回歸測試。** 不承諾 PWA 可達到 Goodnotes 原生 Apple Pencil 延遲、系統防掌誤觸或 Pencil Pro 硬體手勢的同等體驗。PDF 匯入／匯出部分功能依賴外部函式庫與 Safari 瀏覽器能力。
