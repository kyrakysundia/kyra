# 月汐 Kyra Kysundia 官方網站

網站網址：https://kyrakysundia.github.io/kyra/

所有檔案都放在專案最外層（沒有子資料夾）。

## 怎麼更新

**改連結、信箱**
打開 `index.html`，拉到「網站設定」那一塊（`const SITE={ ... }`），直接改引號裡的網址：
棉花糖、X、YouTube、Twitch、Instagram、Discord、歐付寶、信箱都在這裡。

**換圖片**
用**同一個檔名**上傳新圖就會取代舊圖（Add file → Upload files）：
- `logo.png`：導覽列 LOGO
- `three-view.jpg`：三視圖設定圖
- `hero.webp`、`about-portrait.webp`、`design-detail.webp`、`banner.jpg`：首頁與關於頁的圖
- `work-01.webp ~ work-04.webp`：委託作品集
- `emote-01.webp ~ emote-09.webp`：表情符號；有 `-anim` 的是動圖，滑過去才會播放
- `og-image.png`：貼到 X、Discord 時的分享預覽圖
- `favicon.ico`、`favicon-32.png`、`apple-touch-icon.png`：網站小圖示

更新後網站大約 1～3 分鐘會變，看不到新圖時，用 Ctrl + Shift + R 重新整理。

**改文字、價格、新增表情等**
在 `index.html` 裡，直接搜尋文字就找得到。比較複雜的改動，建議再請 Claude 幫忙。
