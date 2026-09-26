# NoteCanvas v5.27.0 驗證報告

## 已執行

- 主程式兩段內嵌 JavaScript、Service Worker：Node.js `--check` 語法檢查通過。
- 靜態檢查新版主工具列與浮動工具列 CSS、實作中的新增筆記流程、紙張選擇、三角形與菱形繪圖分支。
- 版本號已同步 HTML title、APP_VERSION、manifest 及 SW/cache；ZIP 會包含全部必要資產。
- 仍使用 IndexedDB NoteCanvasDB v2；沒有 DB 升級或清除資料指令。

## 未通過／未執行的範圍

- 嘗試使用容器 Chromium + Playwright 的 iPad／iPhone 觸控流程測試，但執行環境封鎖 `http://127.0.0.1` 和 `file://` 導航（`net::ERR_BLOCKED_BY_ADMINISTRATOR`），因此未能進行該回歸測試，不能宣稱 Chromium 功能測試通過。
- iPad Safari、iPhone Safari、Apple Pencil 手寫筆壓與手掌防誤觸，尚未實機測試。
- Goodnotes 原生筆刷核心與手掌排除機制無法僅從畫面錄影複製到 PWA；本版是同類操作／高度相近介面的獨立實作，不宣稱一模一樣。
