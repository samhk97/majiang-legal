# Deploy to GitHub Pages（5 分鐘）

## 步驟

1. 在 GitHub 開新 repo：`majiang-legal`（public）
2. 把整個 `e:/majiang/docs/legal/` 資料夾的內容（不含這個 README）push 到 repo root：

   ```bash
   cd e:/majiang/docs/legal
   git init
   git add privacy-policy.zh-Hant.md privacy-policy.en.md terms-of-service.zh-Hant.md terms-of-service.en.md index.md _config.yml
   git commit -m "Initial legal docs"
   git branch -M main
   git remote add origin https://github.com/<你的 user>/majiang-legal.git
   git push -u origin main
   ```

3. GitHub repo → **Settings → Pages**：
   - Source: Deploy from a branch
   - Branch: `main` / root
   - Save

4. 等 1-2 分鐘，GitHub Pages 完成 build。URL 會是：

   ```
   https://<你的 user>.github.io/majiang-legal/
   ```

5. 各文件 URL（拿這些填到 App Store / Play Store）：

   - 首頁：`https://<user>.github.io/majiang-legal/`
   - 隱私權（中）：`https://<user>.github.io/majiang-legal/privacy-policy.zh-Hant`
   - 隱私權（英）：`https://<user>.github.io/majiang-legal/privacy-policy.en`
   - 使用條款（中）：`https://<user>.github.io/majiang-legal/terms-of-service.zh-Hant`
   - 使用條款（英）：`https://<user>.github.io/majiang-legal/terms-of-service.en`

## 之後要改內容

直接編輯 .md → push → 1-2 分鐘自動更新。
