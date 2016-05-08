# insert-styles [![Build Status](https://travis-ci.org/bendrucker/insert-styles.svg?branch=master)](https://travis-ci.org/bendrucker/insert-styles)

> Insert CSS styles into an HTML document


## Install

```
$ npm install --save insert-styles
```


## Usage

```js
var insertStyles = require('insert-styles')

insertStyles('h1 { font-size: 14px }')
//=> <head><style> h1 { ... }</style></head>
```

## API

#### `insertStyles(styles, [options]) -> void`

##### styles

Required. The string of styles to insert into the DOM.

##### options

###### id

Calling `insertStyles` with the same `options.id` multiple times will make the same `<style>` element be re-used.

## Related

* [insert-css](https://github.com/substack/insert-css)

## License

MIT © [Ben Drucker](http://bendrucker.me)
