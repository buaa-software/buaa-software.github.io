# 开发指南

> 官方文档：https://docsify.js.org/#/zh-cn/

## 开发环境配置

本项目采用 `docsify` 作为静态文档框架，并使用 `docsify-cli` 作为命令行工具，因此需要先安装 `Node.js` 和 `docsify-cli` 。

### 安装 `Node.js`

> 若本机已有 `Node.js` 环境可跳过此步骤。

访问 `Node.js` [官网下载页](https://nodejs.org/zh-cn/download) ，根据界面提示选择适合本机的命令集或安装包进行安装即可。

### 安装 `docsify-cli`

这是 `docsify` 官方的命令行工具，提供了初始化、本地运行、文件生成等功能。

推荐全局安装 `docsify-cli` 工具，可以方便地常见及在本地预览生成的文档。

```bash
npm i docsify-cli -g
```

## 本地运行

确认安装好 `docsify-cli` 工具后，在项目根目录下运行以下命令即可启动本地服务：

```bash
docsify serve .
```

默认端口为 `3000` ，可以通过 `--port, -p` 选项修改。


## 项目结构

以下为项目的基本目录结构：

```bash
.
├── _404.md
├── _asset
├── _media
├── _navbar.md
├── _sidebar.md
├── course
│   └── README.md
├── dev.md
├── index.html
├── life
│   └── README.md
├── README.md
├── school
│   ├── README.md
├── technical
│   └── README.md
└── tool
    └── README.md
```

- `index.html` 为入口文件，定义了项目的样式、行为和功能
- `README.md` 定义首页的内容
- `_sidebar.md` 定义侧边栏的内容
- `_navbar.md` 定义顶部导航栏的内容
- `_404.md` 定义异常页面的内容
- `dev.md` 为项目开发指南，即本页面中的内容
- `_asset` 为静态资源文件夹，其中包含项目所需的图片、文档等资源
- `_media` 为媒体资源文件夹，目前存储了软件学院logo作为网页图标
- `course` 为课程文件夹、`school` 为学校文件夹、 `technical` 为专业文件夹、 `life` 为生活文件夹、 `tool` 为工具文件夹，其中分别包含了各个模块的文档内容
