# Railway 部署说明

## 目录

`/Users/liu/.openclaw/workspace/paperdrop-site`

## 方式一：Railway 网页端从 GitHub 部署（推荐）

1. 把这个目录提交到 GitHub 仓库
2. 打开 Railway，新建 Project
3. 选择 `Deploy from GitHub repo`
4. 选择包含 `paperdrop-site` 的仓库
5. 如果 Railway 让你选 Root Directory，填写：
   `paperdrop-site`
6. Railway 会自动执行：
   - 安装依赖（这个项目几乎没有依赖）
   - 运行 `npm start`
7. 成功后在 Railway 里生成公网域名

## 方式二：Railway CLI

在这个目录运行：

```bash
cd /Users/liu/.openclaw/workspace/paperdrop-site
railway up
```

如果还没登录：

```bash
railway login
```

## 当前运行方式

- 使用 `server.js` 提供静态页面
- 默认入口：`index.html`
- 端口：`PORT` 环境变量（Railway 自动提供）
