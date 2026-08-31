# 草本堂出勤管理

獨立的後台、店內動態 QR 顯示頁及員工打卡頁。綠白配色；不包含其他店的員工或紀錄。

- `app/`：後台及打卡功能、雲端 API。
- `web/`：GitHub Pages 前端入口；`docs/`：編譯後網站。
- `.openai/hosting.json`：草本堂獨立服務及資料庫綁定。
- 正式密碼與存取憑證只儲存在服務端環境設定，不能提交至 GitHub。
- 首次登入從空白人員、排班、範本、出勤與審核資料開始。

使用 Node.js 22+ 和 pnpm。前端編譯：`pnpm exec vite build web --config web/vite.config.ts --base /caobentang/ --outDir ../docs`。
雲端服務：`pnpm build`。
