# zax-px2rem-loader

a [webpack](http://webpack.github.io/) loader for [px2rem](https://github.com/zhiyingzzhou/zax-px2rem-loader)

[![NPM version][npm-image]][npm-url]
<!-- [![Build status][travis-image]][travis-url] -->
[![Downloads][downloads-image]][downloads-url]

[npm-image]: https://img.shields.io/npm/v/zax-px2rem-loader.svg
[npm-url]: https://npmjs.org/package/zax-px2rem-loader
<!-- [travis-image]: https://img.shields.io/travis/Jinjiang/zax-px2rem-loader.svg -->
<!-- [travis-url]: https://travis-ci.org/zhiyingzzhou/zax-px2rem-loader -->
[downloads-image]: http://img.shields.io/npm/dm/zax-px2rem-loader.svg
[downloads-url]: https://npmjs.org/package/zax-px2rem-loader

## Install

`npm install zax-px2rem-loader`

## webpack config

```
module.exports = {
  // ...
  module: {
    rules: [{
      test: /\.css$/,
      use: [{
        loader: 'style-loader'
      }, {
        loader: 'css-loader'
      }, {
        loader: 'zax-px2rem-loader',
        // options here
        options: {
          remUnit: 75,
          unit: 'vw' // 支持'vw'或者'rem'
        }
      }]
    }]
  }
}
```


详细信息查看[px2rem](https://github.com/songsiqi/px2rem)
支持将px或者rpx转化为rem或者vw单位

<!-- ## Example -->

<!-- See an example [here](./examples). -->