# 幻象金融 Mirage Finance — 隱私政策與服務條款

對外託管頁：<https://yang87924.github.io/mirror-privacy-policy/>

供 Google Play「應用程式內容」與 App Store 的隱私政策 URL 欄位使用。

## ⚠️ 不要直接編輯 `index.html`

本檔是**產生物**。內容的唯一正本在私有 monorepo：

```text
mirror_finance_mono/mirror_finance_app/lib/features/settings/presentation/pages/legal_content.dart
```

那份同時是 App 內「設定 → 關於 → 隱私政策」顯示的內容——
商店要求政策須可於 App 內取得，所以以使用者實際看到的那份為準。

## 更新方式

改完正本後，在 monorepo 執行：

```powershell
node scripts/generate-legal-pages.mjs --publish-to D:\code\side-projcet\mirror-privacy-policy
```

再於本 repo `git add index.html && git commit && git push`。

## 為什麼這裡是獨立的 public repo

monorepo 為私有，GitHub Pages 對私有 repo 需付費方案，故對外託管拆出來。

這份必然是副本——但**副本只要是「一個指令重產」就不會分家，用手複製才會**。
請務必用上面的指令，不要複製貼上。
