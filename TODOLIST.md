# TODO（需要你亲自完成的步骤）

以下步骤涉及账号登录/授权，我无法替你完成。

## 1. 登录 Vercel（必须）

在 `D:\ozpwebsite` 执行：

```powershell
vercel login
```

按提示用浏览器完成登录授权。

## 2. 首次发布到公网（必须）

```powershell
vercel --prod
```

按提示选择：
- Link to existing project? -> `N`
- Project name -> `ozpwebsite`
- In which directory is your code located? -> `./`

完成后会得到公网链接（例如 `https://xxx.vercel.app`）。

## 3. （可选）绑定自定义域名

登录 Vercel Dashboard：
- 打开项目 `ozpwebsite`
- Settings -> Domains
- 添加你的域名并按提示配置 DNS

## 4. （可选）把代码推到 GitHub 以便持续部署

```powershell
git remote add origin https://github.com/<你的用户名>/<你的仓库名>.git
git push -u origin main
```

之后每次 `git push` 会触发自动更新。
