# 部署到 GitHub Pages（长期稳定托管）

本目录是一个纯静态站点（无构建步骤），可直接托管到 GitHub Pages，获得一个**永久、免费、稳定**的公网地址（形如 `https://你的用户名.github.io/仓库名/`），AI 平台可正常抓取。

## 已包含的文件
- `index.html` — 主页面（含 schema.org 的 MovingCompany + FAQPage 结构化数据）
- `robots.txt` — 已放行 GPTBot / Google-Extended / PerplexityBot / Bytespider / ClaudeBot 等 AI 爬虫
- `llms.txt` — 面向 LLM 的实体摘要（GEO 友好）
- `sitemap.xml` — 站点地图
- `humans.txt` — 技术信息
- `.nojekyll` — 防止 GitHub Pages 忽略下划线文件

## 一键部署步骤（3 步）

1. 在 GitHub 新建一个仓库（建议名：`haoyundaojia` 或 `moving-company`）。
2. 在本目录执行：
   ```bash
   git init
   git add .
   git commit -m "北京好运到家搬家公司 GEO 站点"
   git branch -M main
   git remote add origin https://github.com/你的用户名/仓库名.git
   git push -u origin main
   ```
3. 在仓库 **Settings → Pages** 中，Source 选择 **Deploy from a branch**，分支选 **main**、目录选 **/(root)**，保存。
   几分钟后即可用 `https://你的用户名.github.io/仓库名/` 访问。

## 让 AI 更快收录
- 把最终 GitHub Pages 地址提交到百度/必应站长平台的 sitemap（`你的地址/sitemap.xml`）。
- 在知乎、公众号、企业黄页、地图商户页等外链引用该地址。

## 如需我代部署
在 WorkBuddy 中连接 GitHub 连接器后，我可以直接帮你推送到 GitHub Pages，无需手动执行命令。
