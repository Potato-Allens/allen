[README.md](https://github.com/user-attachments/files/30400364/README.md)
# 极序超级龙虾

一个静态版 OpenClaw 技能大全页面，用于展示 OpenClaw 相关技能、分类筛选、搜索结果和客服联系方式。

## 项目简介

本项目是纯前端静态页面，不需要后端服务或构建流程。仓库中主要包含完整的 HTML 页面和页面所需的图片资源，适合直接部署到 GitHub Pages、Nginx、宝塔、Cloudflare Pages、Vercel 静态站点等环境。

## 功能特性

- 技能大全展示：以卡片形式展示 OpenClaw 相关技能内容。
- 分类筛选：通过侧边栏分类快速筛选技能。
- 关键词搜索：支持在页面中搜索技能内容。
- 分页浏览：适合展示较多技能条目。
- 明暗主题：页面内置浅色和深色视觉样式。
- 客服弹窗：内置关于介绍图、QQ 售后信息和微信二维码。
- 静态部署：无需数据库、无需 Node.js、无需登录即可访问。

## 目录结构

```text
.
├── index.html                  # 主页面
├── OpenClaw技能大全.html        # 与主页面内容一致的中文命名页面
├── favicon.svg                 # 网站图标
└── public/
    ├── about.png               # 关于/介绍图片
    ├── claw.svg                # OpenClaw 标识
    └── contact/
        ├── qq-afternoon-evening.png
        └── wechat-morning.png
```

## 本地预览

方式一：直接打开

双击 `index.html` 即可在浏览器中预览。

方式二：启动本地静态服务

```bash
python -m http.server 8080
```

然后访问：

```text
http://localhost:8080/
```

## 部署方式

将仓库内的文件上传到任意静态网站托管环境即可，入口文件使用 `index.html`。

常见部署位置：

- GitHub Pages
- Cloudflare Pages
- Vercel
- Netlify
- Nginx 静态目录
- 宝塔网站根目录

## 内容维护

当前页面内容主要集中在 `index.html` 中。如果需要修改技能文案、分类、联系方式或页面样式，可以直接编辑该文件。

图片资源位于 `public/` 目录：

- 替换介绍图：更新 `public/about.png`
- 替换 Logo：更新 `public/claw.svg`
- 替换二维码：更新 `public/contact/` 下的图片

## 注意事项

- 页面是构建后的静态 HTML，文件体积较大，编辑前建议先备份。
- 如果修改了图片文件名，需要同步修改 HTML 中引用图片的路径。
- 部署到子目录时，请确认 `./public/...` 资源路径仍然可以正确访问。

## 项目地址

GitHub: <https://github.com/Potato-Allens/allen>
