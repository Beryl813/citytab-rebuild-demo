# 找语伴 Demo

这是 `https://city-wv9q.vercel.app/` 的可部署静态构建包。文件已全部平铺在根目录，适合直接上传到自己的 GitHub 仓库，或部署到 Vercel、GitHub Pages、Netlify 等静态托管平台。

## 本地预览

需要 Node.js。进入项目目录后运行：

```bash
npx serve .
```

然后打开终端输出的本地地址。

也可以使用任意静态文件服务器，不建议直接双击 `index.html`，因为部分浏览器会限制本地文件的模块加载。

## 部署到 GitHub

```bash
git init
git add .
git commit -m "Add language partner demo"
git branch -M main
git remote add origin https://github.com/<your-name>/<your-repo>.git
git push -u origin main
```

在 Vercel 中导入该仓库时：

- Framework Preset 选择 `Other`
- Build Command 留空
- Output Directory 填 `.`

如果使用 GitHub 网页上传文件，请把压缩包里的所有文件直接上传到仓库根目录。

## 资源说明

- 页面逻辑和样式来自线上公开部署的生产构建文件，原始 React/Vite 源码和 source map 未随部署公开。
- 头像使用 Unsplash 远程图片。
- 地图使用 Pigeon Maps 和 OpenStreetMap 瓦片，页面内保留了对应署名链接。
- 因此这个包可以复现当前 demo 的页面与交互，但不包含原项目的开发源码、构建配置或后端服务。
