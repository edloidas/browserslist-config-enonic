<h1 align="center">browserslist-config-enonic</h1>

[![Travis Build Status][travis-image]][travis-url]
[![devDependency Status][devdep-image]][devdep-url]

Shareable [Browserslist](https://github.com/ai/browserslist#shareable-configs) config for @enonic applications.

## Install

```
npm install --save-dev browserslist-config-enonic
```

## Usage

Choose the desired way to use Browserslist configuration. Additional information can be found in the official [documentation](https://github.com/ai/browserslist#shareable-configs).

###### package.json
```json
{
  "browserslist": [
    "extends browserslist-config-enonic"
  ]
}
```

###### Browserslist config (`.browserslistrc`)
```
extends browserslist-config-enonic
```

###### Babel config
In Babel configuration in `.js` format with [babel-preset-env](https://github.com/babel/babel/tree/master/experimental/babel-preset-env), requiring config will return the array of supported browsers.
```js
{
  presets: [
    [ 'env', {
      targets: {
        browsers: require('browserslist-config-enonic')
      }
    }]
  ]
}
```

## License ##

[Apache-2.0](LICENSE) © [Enonic](https://enonic.com)

<!-- Links -->
[travis-url]: https://travis-ci.org/edloidas/browserslist-config-enonic
[travis-image]: https://img.shields.io/travis/edloidas/browserslist-config-enonic.svg?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB2aWV3Qm94PSItMTQyLjUgLTE0Mi41IDI4NSAyODUiPjxjaXJjbGUgcj0iMTQxLjciIGZpbGw9IiNERDQ4MTQiLz48ZyBpZD0iYSIgZmlsbD0iI0ZGRiI%2BPGNpcmNsZSBjeD0iLTk2LjQiIHI9IjE4LjkiLz48cGF0aCBkPSJNLTQ1LjYgNjguNGMtMTYuNi0xMS0yOS0yOC0zNC00Ny44IDYtNSA5LjgtMTIuMyA5LjgtMjAuNnMtMy44LTE1LjctOS44LTIwLjZjNS0xOS44IDE3LjQtMzYuNyAzNC00Ny44bDEzLjggMjMuMkMtNDYtMzUuMi01NS4zLTE4LjctNTUuMyAwYzAgMTguNyA5LjMgMzUuMiAyMy41IDQ1LjJ6Ii8%2BPC9nPjx1c2UgeGxpbms6aHJlZj0iI2EiIHRyYW5zZm9ybT0icm90YXRlKDEyMCkiLz48dXNlIHhsaW5rOmhyZWY9IiNhIiB0cmFuc2Zvcm09InJvdGF0ZSgyNDApIi8%2BPC9zdmc%2B "Linux build"

[devdep-url]: https://david-dm.org/edloidas/browserslist-config-enonic#info=devDependencies
[devdep-image]: https://david-dm.org/edloidas/browserslist-config-enonic/dev-status.svg
