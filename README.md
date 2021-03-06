# entry-extract-webpack-plugin

微信小程序构建入口生成插件，依赖于源代码目录中的 app.json 文件进行入口生成，属于 webpack-build-miniprogram 工具包核心依赖。

## Installation

```shell
$ npm install entry-extract-webpack-plugin --save
```

## Usage

```javascript
const EntryExtractPlugin = require('entry-extract-webpack-plugin');

module.exports = {
  // ...
  plugins: [
    new EntryExtractPlugin(options),
  ],
  // ...
};
```

## Options

### context

* Type: `String`
* Default: `compiler.context`

源代码目录绝对路径，建议您在`webpack`配置文件中设置`context`属性。

### templateExt

* Type:  `String`
* Default: `.wxml`

模板文件后缀名，可支持`.wxml` 和 `.swan` 两种文件。

## License

[MIT](https://github.com/Oc-master/entry-extract-webpack-plugin/blob/master/LICENSE)
