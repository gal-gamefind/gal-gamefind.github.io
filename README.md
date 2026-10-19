# Galgame入门百科 · 科普网站

一个纯科普向的 Galgame（美少女游戏）介绍单页网站，无成人内容，SEO 友好。

## 文件清单

| 文件 | 说明 |
| --- | --- |
| index.html | 网站主页面（单文件，无外部依赖，样式内联） |
| robots.txt | 搜索引擎爬虫规则 |
| sitemap.xml | 站点地图 |

## 域名说明

网站域名已配置为 GitHub Pages 地址：`https://gal-gamefind.github.io/`，
已在以下位置生效：

1. `index.html` → `<link rel="canonical">`
2. `index.html` → `og:url` meta 标签
3. `index.html` → JSON-LD 结构化数据中的 `"url"`
4. `robots.txt` → `Sitemap:` 行（以及 sitemap.xml 中的 `<loc>`）

## 部署到 GitHub Pages

1. 在 GitHub 创建名为 `gal-gamefind.github.io` 的仓库（仓库名必须与域名一致）。
2. 将本目录 4 个文件（index.html / robots.txt / sitemap.xml / README.md）推送到仓库 main 分支根目录。
3. 仓库 Settings → Pages → Source 选择 `main` 分支 `/ (root)`，保存。
4. 等待 1–2 分钟部署完成，访问 https://gal-gamefind.github.io/ 即可。
5. 可选：到 Google Search Console / Bing 站长平台提交 `https://gal-gamefind.github.io/sitemap.xml` 加速收录。

## 按钮链接说明

首页两处显眼的「Galgame游戏资源下载」按钮均指向 Steam 视觉小说专区：
https://store.steampowered.com/category/visual_novel

如需改为其他网址（如 HIKARI FIELD 官方商城 https://hikarifield.co.jp/ 或你自己的资源站），
在 index.html 中搜索该链接替换即可（共出现 3 处：hero 按钮、CTA 横幅按钮、页脚）。

## SEO 要点（已内置）

- 完整 TDK（title / description / keywords），核心词：galgame是什么、美少女游戏、黄油、视觉小说
- Open Graph + Twitter Card 分享卡片
- JSON-LD 结构化数据：FAQPage（5 条问答）+ WebSite
- 语义化 HTML5 标签（header/nav/main/section/article/footer）、清晰的 h1-h3 层级
- 移动端响应式、锚点导航、单文件零外部请求（加载快，利于 Core Web Vitals）

## 本地预览

直接双击 index.html 即可在浏览器打开；或部署到任意静态托管（GitHub Pages / Vercel / 云服务器）。
