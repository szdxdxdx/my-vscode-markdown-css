# My VS Code Markdown CSS

## Intro

Using custom markdown styles in VS code.

## Markdown Styles Preview

*The preview page needs to introduce various JS libraries online. Please be patient and wait for the page to load.*

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
