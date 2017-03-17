# clipboard-copy [![travis][travis-image]][travis-url] [![npm][npm-image]][npm-url] [![downloads][downloads-image]][downloads-url]

[travis-image]: https://img.shields.io/travis/feross/clipboard-copy/master.svg
[travis-url]: https://travis-ci.org/feross/clipboard-copy
[npm-image]: https://img.shields.io/npm/v/clipboard-copy.svg
[npm-url]: https://npmjs.org/package/clipboard-copy
[downloads-image]: https://img.shields.io/npm/dm/clipboard-copy.svg
[downloads-url]: https://npmjs.org/package/clipboard-copy

### Lightweight copy to clipboard for web pages

The goal of this package is to offer simple copy-to-clipboard functionality in
modern web browsers using the fewest bytes. To do so, this package only supports
modern browsers. No fallback using Adobe Flash, no hacks. Just 25 lines of code.

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

### `copy(text)`

Copy the given text to the user's clipboard.

Note: in most browsers, copying to the clipboard is only allowed if `copy()` is
triggered in direct response to a user gesture like a `'click'` or a `'keypress'`.

## comparison to alternatives

- **`clipboard-copy` (this package): 465 bytes**
- [`clipboard-js`](https://www.npmjs.com/package/clipboard-js): 1.83 kB
- [`clipboard`](https://www.npmjs.com/package/clipboard): 3.19 kB

## license

MIT. Copyright (c) [Feross Aboukhadijeh](http://feross.org).