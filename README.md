# clipboard-copy

_This repo is a fork of `clipboard-copy` that supports ES Modules._

### Lightweight copy to clipboard for the web

The goal of this package is to offer simple copy-to-clipboard functionality in
modern web browsers using the fewest bytes. To do so, this package only supports
modern browsers. No fallback using Adobe Flash, no hacks. Just 30 lines of code.

Unlike other implementations, text copied with `clipboard-copy` is clean and
unstyled. Copied text will not inherit HTML/CSS styling like the page's background
color.

**Supported browsers:** Chrome, Firefox, Edge, Safari.

Works in the browser with [browserify](http://browserify.org/)!

## install

```
npm install clipboard-copy
```

## usage

```js
const copy = require('clipboard-copy')

button.addEventListener('click', function () {
  copy('This is some cool text')
})
```

## API

### `successPromise = copy(text)`

Copy the given text to the user's clipboard. Returns `successPromise`, a promise that resolves if the copy was successful and rejects if the copy failed.

Note: in most browsers, copying to the clipboard is only allowed if `copy()` is
triggered in direct response to a user gesture like a `'click'` or a `'keypress'`.

## comparison to alternatives

- **`clipboard-copy` (this package): [508 B gzipped](https://bundlephobia.com/result?p=clipboard-copy)**
- [`clipboard-js`](https://www.npmjs.com/package/clipboard-js): [1.7 kB gzipped](https://bundlephobia.com/result?p=clipboard-js)
- [`clipboard`](https://www.npmjs.com/package/clipboard): [3.2 kB gzipped](https://bundlephobia.com/result?p=clipboard)

## testing

Testing this module is currently a manual process. Open `test.html` in your web browser and follow the short instructions. The web page will always load the latest version of the module, no bundling is necessary.

## license

MIT. Copyright (c) [Feross Aboukhadijeh](http://feross.org).
