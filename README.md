# 代码卡片

MyPaste extension `com.mypaste.code-card` (version `6.3.0`).

把代码或纯文本条目渲染成可分享的卡片图片：整页工作台沿用 carbon.now.sh 的编辑器布局——主题与语言两条下拉、编辑、复制与导出、页面关闭按钮，背景色板与「窗口 / 编辑器」两栏都在设置浮层里。卡片默认跟随宿主主题，另有七套配色、三种窗口框、行号、自动换行、字号、行高、留白与投影，背景可透明或任意十六进制色，导出 1× 或 2×；单行内容先按语言重排再绘制，宽度按真正画出的文字量取，长行默认在页面宽度处折行，不出横向滚动条；点卡片本身就能在卡片里改字，光标落在点到的位置，边打边重绘。卡片完全在本机绘制，不联网、不读取其它条目。

This repository is an independent copy extracted from the former `mypaste-code-extensions` monorepo at commit `2af6675ab1473c9e38146ea0b6da68256a293440`. It contains only this extension's tracked source files. The published `.mypaste-plugin` archives and marketplace index live in [`mypaste-extensions-catalog`](https://github.com/mypaste/mypaste-extensions-catalog).

The manifest speaks MyPaste plugin protocol v3. Installation, capability mediation, and content-digest verification are performed by the MyPaste desktop host.

## Files

- `mypaste.plugin.json`: package identity and capability declaration.
- `run.sh`, `src/`, `panel.html`, or `run`: package implementation.

## Build

```bash
bun install
bun run build
```

The generated `preview.html` is intentionally ignored; edit `src/preview.html` and `src/main.ts` instead.

## License

MIT. See [LICENSE](LICENSE).
