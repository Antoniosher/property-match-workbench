物件配對工作台 V2｜網站部署包

內容
- index.html：網站入口，包含物件配對、客戶追蹤 CRM、AI 業務導師示範模組。

目前版本能力
- 可在手機與桌面瀏覽器操作。
- 物件與客戶資料存在使用者目前瀏覽器的 localStorage。
- 可匯出物件 CSV。
- AI 導師目前是內建情境範本，不會呼叫外部 AI 模型。
- 591 連結目前是人工補充資料流程，並非官方 API 串接。

部署方式（靜態網站）
1. 將本資料夾上傳到 GitHub repository。
2. 在 repository 的 Settings > Pages 開啟 GitHub Pages。
3. Source 選 Deploy from a branch，Branch 選 main，Folder 選 /(root)，儲存。
4. GitHub Pages 完成後會提供固定網址，可用 Safari 開啟並加入主畫面。

重要限制
這只是可部署的前端原型。部署成公開網址後，不會自動變成安全的多人 CRM。不要在此版本存放身分證、銀行帳戶、合約等敏感資料。正式商用前應加入登入驗證、伺服器端資料庫、角色權限、備份、稽核紀錄與 AI API 的伺服器端代理；不可把 AI API Key 寫在前端 HTML。
