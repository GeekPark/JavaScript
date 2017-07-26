# JavaScript
GeekPark JavaScript 编码规范

参考文档 https://github.com/standard/standard/blob/master/docs/README-zhcn.md

1. 前端 `vue` 项目中 `webpack` -> `module` -> `rules` 如下配置, [`.eslintrc.js`](https://github.com/GeekPark/JavaScript/blob/master/.eslintrc.js) 文件
``` JavaScript
{
  test: /\.(js|vue)$/,
  loader: 'eslint-loader',
  enforce: 'pre',
  nclude: [resolve('src'), resolve('test')],
  options: {
    formatter: require('eslint-friendly-formatter')
  }
}
```
并安装依赖项 `yarn add xxx --dev`
``` json
"eslint": "^3.19.0",
"eslint-config-standard": "^6.2.1",
"eslint-friendly-formatter": "^3.0.0",
"eslint-loader": "^1.7.1",
"eslint-plugin-html": "^3.0.0",
"eslint-plugin-promise": "^3.4.0",
"eslint-plugin-standard": "^2.0.1",
```
