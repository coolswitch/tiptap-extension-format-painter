# tiptap-extension-format-painter

Format painter extension for tiptap, not support for **table and bullet** yet

## Instalation

`npm i tiptap-extension-format-painter -S`

## Usage

Add it as any extension in `useEditor()`

```ts
import FormatPainter from 'tiptap-extension-format-painter'

  extensions: {
    FormatPainter,
```

## Commands

```js
/** Enable format painter */
editor.commands.enableFormatPainter({
  once: false, // 是否单次效果
  getChain: () => props.editor.chain(),
})

/** Format painter state notify */
editor.commands.watchFormatPainterState((isEnable: boolean) => {
  console.log('FormatPainter state change:', isEnable)
}) 
```
