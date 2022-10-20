# tiptap-extension-format-painter

tiptap 的格式刷扩展，暂未对**表格、项目符号**做支持

## Instalation

`npm i tiptap-extension-format-painter -S`

## Usage

添加在 `useEditor()` 的扩展中：

```ts
import FormatPainter from 'tiptap-extension-format-painter'

  extensions: {
    FormatPainter,
```

## Commands

```js
/** 启用格式刷 */
editor.commands.enableFormatPainter({
  once: false, // 是否单次效果
  getChain: () => props.editor.chain(),
})

/** 格式刷启用状态通知 */
editor.commands.watchFormatPainterState((isEnable: boolean) => {
  console.log('FormatPainter state change:', isEnable)
})
```
