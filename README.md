# My VS Code Markdown CSS

## CSS 效果预览

https://szdxdxdx.github.io/my-vscode-markdown-css/markdown_editor.html

## 如何使用

### 方案一

把 `markdown.css` 文件复制到**当前工作区**，修改配置（管理 > 设置 > 打开设置 > 编辑 `Settings.json` 文件），添加如下内容，即 `markdown.css` 对于当前工作区的相对路径：

```json
"markdown.styles": [
  "markdown.css"
]
```

### 方案二

你可以上传 CSS 文件，并使用 URL 作为文件路径，比如：

```json
"markdown.styles": [
  "https://szdxdxdx.github.io/my-vscode-markdown-css/markdown.css"
],
```

### 方案三

直接替换掉 vscode 默认的 `markdown.css`。

默认的 css 样式文件可能存放在：`C:\Program Files\Microsoft VS Code\resources\app\extensions\markdown-language-features\media\markdown.css`。
