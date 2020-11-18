# 微信 Markdown 编辑器

## 项目运行
* yarn install 如果没有响应或者很慢的话，可以使用 npm install
* npm run serve 

## 配置说明
### header 操作栏
header 操作栏的配置文件在 src/assets/scripts/config.js 中，包括：
* 有无称线
* 字号大小
* 默认颜色
* 代码主题风格

### 默认文本
默认文本内容在 src/assets/scripts/default-content.js 中

### 文献引用
可以参考如下使用方法
```html
## Markdown 增加文献引用
<span style="color:blue">这篇文章是介绍如何在 Markdown 中增加文献引用。</span>[<sup style="color:red">[1]</sup>](#refer-anchor-1)

<div id="refer-anchor-1"></div>

- [1] [百度学术](http://xueshu.baidu.com/)

<div id="refer-anchor-2"></div>

- [2] [Wikipedia](https://en.wikipedia.org/wiki/Main_Page)
```
