# 基于 `fontmin` 压缩 `TTF` 字体文件

## 主要功能
* 根据用户传入文字 从字体文件中寻找后压缩
* 默认使用常用中文三千字进行压缩

## 使用方式

* 项目安装

```bash
  npm i melon-min-font-plugin -D
```

* `webpack` 初始化

```js
const melonMinFontPlugin = require("melon-min-font-plugin");
  plugins: [
    new melonMinFontPlugin({
      extraWord: "自定义文字",
      // true 可以将自定义文字和常用字体合并
      isMerge: false,
      // 不压缩文件
      exclude:[ 'iconfont.ttf' ]
    })
  ],
```

## 相关文档链接

* [`fontmin`](https://www.npmjs.com/package/fontmin)
* [`webpack-sources`](https://www.npmjs.com/package/webpack-sources)