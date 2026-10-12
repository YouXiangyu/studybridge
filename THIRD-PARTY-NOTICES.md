# 第三方组件

笔记桥自身适用专有软件使用许可；第三方组件继续适用下面各自的许可证，笔记桥的许可不限制这些第三方许可证已经授予的权利。发布版没有打包个人课件、笔记或登录凭据。

| 组件 | 版本 | 许可与保存位置 |
| --- | --- | --- |
| [PDF.js](https://github.com/mozilla/pdf.js) | 5.6.205 | Apache-2.0；`public/vendor/PDFJS-LICENSE.txt` |
| [Marked](https://github.com/markedjs/marked) | 17.0.5 | MIT；`public/vendor/MARKED-LICENSE.md` |
| [html2canvas](https://github.com/niklasvh/html2canvas) | 1.4.1 | MIT；`public/vendor/HTML2CANVAS-LICENSE.txt` |
| [KaTeX](https://github.com/KaTeX/KaTeX) | 0.19.0 | MIT；`public/vendor/katex/LICENSE.txt` |

PDF.js 的字映射、字体和图像解码器保留在原目录，具体见 `public/vendor/cmaps/LICENSE`、`standard_fonts/LICENSE_*`、`wasm/LICENSE_*`。构建时完整复制这些资源，不裁掉许可证。

Node.js 和 Codex CLI 是用户自行安装的外部依赖，不随 EXE 分发。其许可由各自发行方提供：[Node.js](https://nodejs.org/)、[Codex CLI](https://github.com/openai/codex)。表中的 `public/` 路径在 EXE 解包目录中对应 `app/public/`。
