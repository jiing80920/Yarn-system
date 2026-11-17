# 用紗量管理

託工用紗量、各機台用紗計算、領紗提醒、預估完工時間與統整表格。
單一網頁（`index.html`），不需要安裝、不需要伺服器，資料存在使用者自己的瀏覽器。

## 檔案說明

| 檔案 | 用途 |
| --- | --- |
| `index.html` | 主程式（所有功能都在這一個檔案） |
| `manifest.json`、`icon-*.png`、`apple-touch-icon.png`、`favicon.png` | 網頁圖示與「加入主畫面」設定 |
| `.nojekyll` | 告訴 GitHub Pages 直接原樣發佈 |

## 部署到 GitHub Pages

1. 登入 GitHub，按右上角 **+** → **New repository**。
2. Repository name 取名，例如 `yarn-system`，選 **Public**，按 **Create repository**。
3. 在新的空 repository 頁面按 **uploading an existing file**，把這個資料夾**裡面的所有檔案**（包含 `.nojekyll`）拖進去，按 **Commit changes**。
   - 要上傳的是檔案本身，`index.html` 必須在 repository 的最上層，不要多包一層資料夾。
4. 進入 **Settings** → **Pages**。
5. **Source** 選 **Deploy from a branch**，**Branch** 選 `main`、資料夾選 `/ (root)`，按 **Save**。
6. 等 1～2 分鐘，頁面上方會出現網址：

   ```
   https://<你的帳號>.github.io/yarn-system/
   ```

之後要更新程式，只要在 repository 重新上傳新的 `index.html`（覆蓋同名檔案）並 Commit，約一分鐘後網址就會是新版。

## 使用提醒

- **資料只存在各自的瀏覽器裡**，換電腦、換瀏覽器、清除瀏覽器資料或使用無痕模式，記錄都不會跟著走。
- 請定期到「統整表格」分頁按 **匯出備份**，把檔案存起來；換電腦或資料遺失時用 **匯入還原** 即可還原。
- 同一個 GitHub 帳號的各個網頁（例如 `yarn-calculator`）網址相同，但本程式的資料使用獨立的名稱儲存，不會互相覆蓋。
- 更新 `index.html` 後，既有的資料不會消失（資料在瀏覽器，不在程式裡）。

## 手機／平板

用 Chrome 或 Safari 開啟網址後，選「加入主畫面」，就能像 App 一樣開啟。介面以電腦螢幕為主要設計。
