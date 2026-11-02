# 猛健樂減重日記｜可安裝式手機 APP（PWA）

## 先了解
這是一個可安裝到手機主畫面的 PWA 網頁 APP。要出現「安裝」或「加入主畫面」功能，必須先放到 **HTTPS 網址**（或在 localhost 測試）；直接點開電腦／手機裡的 HTML 檔案，不能完成 PWA 安裝。

## 部署方式（免費選項：GitHub Pages）
1. 登入或建立 GitHub 帳號，新增一個公開 Repository。
2. 將本資料夾內的所有檔案與 `icons` 資料夾上傳到 Repository 根目錄。
3. 到 Repository 的 **Settings → Pages**。
4. 在 Build and deployment 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
5. 等待 GitHub Pages 發佈完成，取得 `https://你的帳號.github.io/專案名稱/` 網址。
6. 用 Samsung 手機的 Chrome 開啟該 HTTPS 網址。
7. 點 Chrome 右上角 ⋮ → **安裝應用程式**（或「新增至主畫面」）→ 安裝。

## 資料保存
- 紀錄存在該 APP 網址的瀏覽器本機儲存空間；從同一個已安裝 APP 開啟，會使用同一個網站來源。
- 不要清除該網站的儲存資料，也不要用無痕模式。
- 仍請定期使用 APP 內的「下載備份檔」功能，並把 JSON 備份保存在手機或雲端。
- 換手機不會自動同步；可用「匯入備份」還原。

## 更新
更新網頁檔案後，Service Worker 會快取 APP 資源。若手機仍顯示舊版，可完全關閉 APP 後重新開啟，或清除該網站快取（不要清除網站資料，避免刪除紀錄）。
