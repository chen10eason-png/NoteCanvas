# NoteCanvas V2

一個針對 iPad / 手機 / 桌面瀏覽器重新設計的手寫筆記 PWA 原型。

## 目前可用
- 文件庫：資料夾、筆記本、我的最愛、搜尋、排序
- 新增筆記本：選封面、空白 / 橫線 / 方格 / 點陣紙
- 頁面縮圖與新增頁面
- 書寫：原子筆 / 鋼筆 / 畫筆、壓感（瀏覽器支援 Apple Pencil pointer pressure 時）
- 螢光筆、橡皮擦、矩形圖形
- 文字方塊，套索模式下可拖曳文字
- 插入圖片
- Undo / Redo
- 閱讀模式
- 匯出目前頁面 PNG
- 本機 localStorage 自動保存
- PWA manifest + Service Worker

## 部署
將整個資料夾上傳到 GitHub repository，GitHub Pages 指向 root 即可。

## 下一階段建議
- PDF.js 匯入 / PDF 註記
- 完整套索（墨跡、圖片、文字）
- 頁面拖曳重排 / 複製 / 旋轉
- IndexedDB 取代 localStorage，支援大量筆記
- Supabase / Firebase 多裝置同步
- 音訊錄製與時間標記
- Apple Pencil 專用模式與更完整手勢
