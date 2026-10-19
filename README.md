# mark.tw

https://mark.tw 的原始檔：純 HTML，沒有建置步驟，中文在 `/`，英文 `/en/`，日文 `/ja/`（三份手動同步）。

- **正式站**：Cloudflare Pages，push 到 `main` 就上線；每個分支有自己的預覽網址。
- **鏡像**：https://markhhm.github.io （GitHub Pages）和 https://www.mark.tw 會把訪客轉到 mark.tw 的同一頁。
- **改 `style.css` 時**：Cloudflare 讓瀏覽器把 CSS 快取 4 小時，所以 6 個頁面引用的 `style.css?v=…` 要一起換成新的版號（例如 `md5 -q style.css | cut -c1-8`），不然訪客會看到舊樣式。
