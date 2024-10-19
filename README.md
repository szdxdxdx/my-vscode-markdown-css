
# My VS Code Markdown CSS

## CSS 效果预览

https://szdxdxdx.github.io/my-vscode-markdown-css/markdown_editor.html

## 如何使用

### 清除默认的 CSS

`my_markdown.css` 并没有完全覆写 vscode 的默认样式，所以需要手动把 vscode 的默认样式文件 `markdown.css` 和 `highlight.css` 中的内容清空。

默认样式文件可能存放在 `C:\Program Files\Microsoft VS Code\resources\app\extensions\markdown-language-features\media\` 目录中。

### 使用自定义的 CSS

#### 方案一

把 `my_markdown.css` 文件复制到当前工作区，修改配置（管理 > 设置 > 打开设置 > 编辑 `Settings.json` 文件），添加如下内容：

```json
"markdown.styles": [
  "my_markdown.css"
]
```

注意，添加的是`my_markdown.css` 在当前工作区的相对路径。似乎不支持 Windows 的绝对路径（`C:\...`）。

#### 方案二

或者，你可以上传 CSS 文件，并使用 URL 作为文件路径，比如：

```json
"markdown.styles": [
  "https://szdxdxdx.github.io/my-vscode-markdown-css/my_markdown.css"
]
```

#### 方案三

把 vscode 默认样式文件 `markdown.css` 中的内容替换成 `my_markdown.css` 的内容。

<hr style="margin: 5em 0;">

# My VS Code Markdown CSS

## CSS Preview

https://szdxdxdx.github.io/my-vscode-markdown-css/markdown_editor.html

## How to Use

### Clear Default CSS

`my_markdown.css` does not fully overwrite the default VS Code styles, so you need to manually clear the contents of the default style files `markdown.css` and `highlight.css`.

These files are likely located in the directory: `C:\Program Files\Microsoft VS Code\resources\app\extensions\markdown-language-features\media\`.

### Use Custom CSS

#### Option 1

Copy the `my_markdown.css` file to your current workspace, then modify the `Settings.json` (File > Preferences > Settings), and add the following:

```json
"markdown.styles": [
  "my_markdown.css"
]
```

You should add the relative path to `my_markdown.css` within your current workspace. Absolute paths (e.g., `C:\...`) from Windows might not be supported.

#### Option 2

Alternatively, you can upload the CSS file and use the URL as the file path, for example:

```json
"markdown.styles": [
  "https://szdxdxdx.github.io/my-vscode-markdown-css/my_markdown.css"
]
```

#### Option 3

You can replace the contents of VS Code's default `markdown.css` file with the contents of `my_markdown.css`.
