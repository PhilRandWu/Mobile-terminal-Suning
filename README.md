# 移动端 苏宁易购

案例： 苏宁网移动端首页

访问地址：m.suning.com

## 1.技术选型

> 方案：我们采取单独制作移动页面方案
>
> 技术： 布局采用 rem 适配布局 （less + rem + 媒体查询)
>
> 设计图： 采用 750px 设计尺寸

## 2.设置视口标签以及引入初始样式

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">
<link rel="stylesheet" type="text/css" href="CSS/normalize.css">
<link rel="stylesheet" type="text/css" href="CSS/index.css">
```

## 3.设置公共 common.less文件

> 1.新建 common.less 设置好最常见的屏幕尺寸，利用媒体查询设置不同的 html 字体大小，因为除了首页其他页面也需要
>
> 2.我们关心的尺寸有 320px 360px 375px 384px 400px 411px 414px 424px 480px 540px 720px 750px
>
> 3.划分的份数定为 15 等份
>
> 4.因为 PC 端也可以打开苏宁移动端首页，默认 HTML字体为 50px  但必须要写在最前边，防止样式被替换。

## 4.新建 index.less 文件

> 1.新建 index.less 在这里写好首页的样式
>
> 2.将刚才设置好的 common.less 引入 index.less 中 
>
> 3.生成 index.css 最后引入到 index.html 中。

## 5.body样式

```css
body {
	min-width: 320px;
    width: 15rem;
    magin: 0 auto;
    line-height: 1.5;
    font-family: Arial,Helvetica;
    background: #F2F2F2;
}
```



## 

