# idunno — 書評網站

部署到 `io-yy.github.io` 的完整靜態網站。

## 檔案結構

```
根目錄/
├── index.html
├── about.html
├── banner.jpg
├── taiyang-cover.jpg
├── README.md
└── reviews/
    ├── taiyang.html
    └── template.html
```

## 部署步驟

1. 在 GitHub 建立 repo，名稱為 `io-yy.github.io`
2. 把這整個資料夾的檔案上傳進去
3. 進入 repo Settings → Pages → Source 選 `main` branch
4. 幾分鐘後網站就上線了：https://io-yy.github.io

## 新增一篇書評

1. 複製 `reviews/template.html`，改名（例如 `reviews/kafukatui.html`）
2. 修改 `template.html` 裡標有 `★ 修改這裡` 的地方：
   - 分類 & 日期
   - 書名、作者
   - 星星評分
   - 出版資訊
   - 書評內文
3. 在 `index.html` 的書評列表裡新增一個 `.book-card` 區塊，
   複製現有的格式，改連結、書名、摘要即可。

## 書背顏色

每本書的書背可以用這幾個 class：
- `s1` 深棕
- `s2` 森林綠
- `s3` 靛藍
- `s4` 玫瑰紅
- `s5` 深紫

輪流使用，或自訂 `style="background: #你的顏色"` 也可以。
