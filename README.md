# ozpwebsite

个人作品集静态站点（纯 `index.html` + 图片资源）。

## 本地预览

直接双击 `index.html` 即可打开，或用任意静态服务器：

```powershell
cd D:\ozpwebsite
python -m http.server 8080
```

访问 `http://localhost:8080`

## 部署到公网（推荐 Vercel）

本项目无需构建步骤，直接静态托管。

### 方式 A：Vercel CLI（最快）

```powershell
cd D:\ozpwebsite
vercel login
vercel --prod
```

首次部署时：
- 选择是否链接现有项目：`N`
- Project Name: `ozpwebsite`（可改）
- 其他保持默认

部署成功后会返回公网 URL。

### 方式 B：Vercel 网页导入 GitHub

1. 把本地仓库推送到 GitHub
2. 到 Vercel 导入仓库
3. Framework 选 `Other`，Build 留空，Output 留空
4. 点击 Deploy

## 内容更新

更新 `index.html` 或图片后：

```powershell
git add .
git commit -m "update portfolio content"
git push
```

Vercel 会自动重新部署。
