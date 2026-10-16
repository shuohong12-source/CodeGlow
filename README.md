# CodeGlow

**把代码高亮后复制到 Word，同时保留颜色、缩进、行号和可编辑文字。**

CodeGlow 是一个面向 Word 文档排版的代码高亮工具。粘贴代码后，页面会自动完成语法高亮；点击“复制格式”，即可将代码以富文本表格形式粘贴到 Word 中。粘贴后的代码不是图片，仍然可以继续修改。

## 在线使用

访问：<https://shuohong12-source.github.io/CodeGlow/>

如果页面暂时无法打开，请确认仓库已经在 **Settings → Pages** 中启用 GitHub Pages，并等待几分钟后刷新。

## 主要功能

- 输入代码后实时高亮，无需额外点击“高亮”按钮
- 支持自动识别语言，也可以手动选择语言
- 一键复制为适合 Word 的富文本表格
- Word 中使用 **Consolas** 字体，代码内容保持可编辑
- 可显示或隐藏行号
- 长代码会在同一行号下自动换行
- 保留原始空格、制表符和代码缩进
- 代码区域使用 **0.5 磅黑色外边框**，不显示内部网格线
- 代码块跨页时尽量保留四周外框，并避免单行代码被拆开
- 提供 Obsidian 浅色、纸张墨色和午夜深色三种主题
- 单文件运行，无需安装、登录或上传代码到服务器

## 支持的语言

| 语言 | 语言 | 语言 |
| --- | --- | --- |
| C | C++ | Python |
| JavaScript | TypeScript | Java |
| Go | Rust | Bash |
| CMD / Windows 批处理 | SQL | JSON |
| HTML / XML | CSS | 自动识别 |

## 使用方法

1. 在左侧输入框中粘贴代码。
2. 根据需要选择语言、主题，以及是否显示行号。
3. 确认右侧预览效果。
4. 点击 **复制格式**。
5. 打开 Word，在需要的位置正常粘贴。
6. 如果 Word 显示粘贴选项，请选择 **保留源格式**。

粘贴完成后，代码中的文字、颜色和缩进仍可在 Word 中继续编辑。

## 本地使用

本项目不需要安装任何依赖：

1. 下载仓库中的 `index.html`。
2. 双击 `index.html`，使用浏览器打开。
3. 建议使用最新版 Microsoft Edge、Google Chrome 或其他 Chromium 内核浏览器。

所有代码高亮和格式生成都在浏览器本地完成。

## 部署到 GitHub Pages

1. 将 `index.html` 和 `README.md` 上传到仓库根目录。
2. 打开仓库的 **Settings → Pages**。
3. 在 **Build and deployment** 中选择 **Deploy from a branch**。
4. 分支选择 `main`，目录选择 `/(root)`，然后点击 **Save**。
5. 等待 GitHub 完成部署后，访问：

   `https://shuohong12-source.github.io/CodeGlow/`

## 常见问题

### 粘贴后没有颜色

请先使用 CodeGlow 的“复制格式”按钮，不要直接选中网页文字复制。粘贴到 Word 时选择“保留源格式”。

### Word 中出现红色波浪线

这是 Word 的拼写检查提示，不是代码格式错误。可以在 Word 的校对设置中关闭对代码区域的拼写检查。

### 字体为什么不是 Consolas

CodeGlow 会在复制内容中指定 Consolas。如果电脑没有该字体，Word 可能会使用其他等宽字体代替。

### 浏览器提示无法访问剪贴板

请允许当前页面使用剪贴板，或改用最新版 Edge/Chrome。通过 GitHub Pages 的 HTTPS 地址访问时兼容性通常更好。

## 项目结构

```text
CodeGlow/
├─ index.html   # 完整应用，包含页面、样式、高亮规则和复制功能
└─ README.md    # 项目说明
```

## 技术说明

CodeGlow 使用原生 HTML、CSS 和 JavaScript 构建，并将语法高亮能力直接打包在 `index.html` 中，因此可以作为单文件离线运行，也可以直接部署到 GitHub Pages。

---

如果这个工具对你的论文、实验报告或技术文档排版有帮助，欢迎为仓库点一个 Star。
