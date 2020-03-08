# 全局less

## 安装
`vue add style-resources-loader`
`Still proceed? Yes`
` CSS Pre-processor? (Use arrow keys)? less`

## 修改vue.config.js

```javascript
const path = require('path')
module.exports = {
  //全局less
  pluginOptions: {
    'style-resources-loader': {
      preProcessor: 'less',
      patterns: [path.resolve(__dirname, 'src/assets/css/variables.less')]
    }
  }
}
```

## assets\css\variables.less

```less
@theme_color: #692dc8;
@theme_color_h: #e9dbff;
@theme_color_btn: #884ed6;
@theme_color_btn_h: #8752dc;
@theme_color_btn_a: #4b1fa0;
```

## 引用

```less
@import './assets/css/variables.less';
.test {
  height: 100px;
  width: 100px;
  background-color: @theme_color_btn_a;
}
```
