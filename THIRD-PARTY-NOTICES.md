# 第三方组件

笔记桥自身适用专有软件使用许可；第三方组件继续适用下面各自的许可证，笔记桥的许可不限制这些第三方许可证已经授予的权利。发布版没有打包个人课件、笔记或登录凭据。

| 组件 | 版本 | 许可与保存位置 |
| --- | --- | --- |
| [PDF.js](https://github.com/mozilla/pdf.js) | 5.6.205 | Apache-2.0；`public/vendor/PDFJS-LICENSE.txt` |
| [pdf-lib](https://github.com/Hopding/pdf-lib) | 1.17.1 | MIT；`public/vendor/pdf-lib-LICENSE.md` |
| [@pdf-lib/fontkit](https://github.com/Hopding/fontkit) | 1.1.1 | MIT；`public/vendor/fontkit-LICENSE.md`；固定版本声明和来源见同目录 provenance 文件 |
| [Marked](https://github.com/markedjs/marked) | 17.0.5 | MIT；`public/vendor/MARKED-LICENSE.md` |
| [html2canvas](https://github.com/niklasvh/html2canvas) | 1.4.1 | MIT；`public/vendor/HTML2CANVAS-LICENSE.txt` |
| [KaTeX](https://github.com/KaTeX/KaTeX) | 0.19.0 | MIT；`public/vendor/katex/LICENSE.txt` |

PDF.js 的字映射、字体和图像解码器保留在原目录，具体见 `public/vendor/cmaps/LICENSE`、`standard_fonts/LICENSE_*`、`wasm/LICENSE_*`。构建时完整复制这些资源，不裁掉许可证。

Node.js 和 Codex CLI 是用户自行安装的外部依赖，不随 EXE 分发。其许可由各自发行方提供：[Node.js](https://nodejs.org/)、[Codex CLI](https://github.com/openai/codex)。表中的 `public/` 路径在 EXE 解包目录中对应 `app/public/`。

Microsoft Edge、Microsoft PowerPoint 与本机中文 TrueType 字体为外部本机组件，不随发布包复制或分发。Edge 用于 PDF 检查和渲染；PowerPoint 仅用于用户选择的 PPTX 转换。字体由用户电脑读取后用于生成 PDF；发布包不包含系统字体文件。PDF 写入库固定版本与 SHA-256 记录于 `public/vendor/pdf-lib-provenance.json`。
