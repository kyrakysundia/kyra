# 月汐 Kyra Kysundia 官方網站

這是一個純靜態網站（不需要伺服器、不需要安裝任何東西），可以直接用 GitHub Pages 免費上線。

## 一、上傳到 GitHub（第一次）

1. 登入 GitHub，右上角 **＋ → New repository**。
   - **Repository name**：
     - 想要網址是 `https://你的帳號.github.io/`，就取名 **`你的帳號.github.io`**（帳號要完全一樣）。
     - 不想的話，隨便取名，例如 `kyra-site`，網址會是 `https://你的帳號.github.io/kyra-site/`。
   - 選 **Public**（免費的 GitHub Pages 需要公開）。
   - 按 **Create repository**。
2. 在新專案頁面點 **uploading an existing file**（或 **Add file → Upload files**）。
3. 把這個資料夾**裡面的所有東西**（`index.html`、`images` 資料夾、四個圖示和預覽圖檔案）一起拖進去。
   - 重點：`index.html` 必須在最外層，不能多包一層資料夾。
4. 等上傳完成，按最下面的 **Commit changes**。

## 二、開啟 GitHub Pages

1. 專案上方 **Settings → Pages**。
2. **Build and deployment → Source** 選 **Deploy from a branch**。
3. **Branch** 選 **main**，資料夾選 **/ (root)**，按 **Save**。
4. 等 1～3 分鐘，重新整理這個頁面，上方會出現你的網站網址。

## 三、一定要改的地方：分享預覽卡片

貼網址到 X、Discord 時，會顯示預覽圖。這需要「完整網址」，所以請改一次：

1. 在 GitHub 專案裡點開 `index.html`，按右上角的鉛筆圖示（Edit）。
2. 找到標著「分享預覽卡片」的那一段（在檔案最上面，大約第 8 到 17 行）。
3. 把 **`USERNAME`** 換成你的 GitHub 帳號，**`REPO`** 換成你的專案名稱，共 **3 處**。
   - 例如帳號 `kyra`、專案 `kyra-site`：
     `https://kyra.github.io/kyra-site/og-image.png`
   - 如果你的專案取名 `你的帳號.github.io`，網址沒有 `REPO` 這一段，
     請改成 `https://你的帳號.github.io/og-image.png`。
4. 按 **Commit changes**。

> 小提醒：X 和 Discord 會把預覽圖暫存一段時間。如果改完還是看到舊的，
> 在網址後面加 `?v=2` 再貼一次就會重新抓取。

## 四、之後怎麼更新

**改連結、信箱**
打開 `index.html`，拉到最底下找到「網站設定」那一塊（`const SITE={ ... }`），
直接改引號裡的網址就好：棉花糖、X、YouTube、Twitch、Instagram、Discord、歐付寶、信箱，都在這裡。

**換圖片**
到 `images` 資料夾，用**同一個檔名**上傳新圖就會取代舊圖：
- `images/logo.png`：導覽列 LOGO
- `images/three-view.jpg`：三視圖設定圖
- `images/hero.webp`、`images/about-portrait.webp`、`images/design-detail.webp`、`images/banner.jpg`：首頁與關於頁的圖
- `images/works/work-01.webp ~ 04`：委託作品集
- `images/emotes/`：表情符號，`emote-06-anim.webp` 這種有 `-anim` 的是動圖，滑過去才會播放
- 根目錄的 `og-image.png`（分享預覽）、`favicon.ico` 等：網站小圖示

換完圖後，網站更新大約要等 1～3 分鐘；瀏覽器如果還看到舊圖，重新整理或換個瀏覽器確認。

**改文字、價格、新增表情等**
這些在 `index.html` 裡，直接搜尋文字就找得到。比較複雜的改動（新增表情、改版面）建議再請 Claude 幫忙。

## 五、上線前檢查清單

- [ ] 分享預覽卡片的 `USERNAME`、`REPO` 已經換成真的
- [ ] 用手機打開網址，每個分頁都點一遍
- [ ] 貼到 Discord 或 X，確認預覽圖有出現
- [ ] Discord 邀請連結沒有過期
- [ ] 棉花糖連結可以正常開啟
- [ ] 房間背景老師的名字（如果之後要補）

## 備註

- 網站字體（思源宋體、Cormorant Garamond、Playfair Display）是從 Google Fonts 載入的，
  訪客需要連網才會顯示完整字體。
- 檔案很小（全部約 1.5 MB），GitHub Pages 的免費額度完全夠用。
