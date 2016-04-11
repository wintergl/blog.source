title: 参考代码-前端-标签切换
date: 2015-11-4 20:00:29
tags: [code, css, html]
categories: 参考
toc: true
layout: no_side_bar
---
标签切换页面代码
<!-- more -->
### CSS代码
```css
.co-tab{
    height: 40px;
    border-bottom: 2px solid #FF6D00;
    position: relative;
    overflow: hidden;
}
.co-tab ul{
    list-style: none;
}
.co-tab ul li{
    float: left;
    width: 140px;
    height: 43px;
    line-height :43px;
    margin-right: 10px;
    background-color: #EFEFEF;
    border : 1px solid #DCDDDD;
    border-radius: 5px;
    border-bottom: none;
    text-align: center;
}
.co-tab ul li.focus{
    background-color: #FF6D00;
    color: #FFFFFF;
}
```
### HTML代码
```html
<div class="co-tab">
     <ul>
          <li class="focus">TAB1</li>
          <li>TAB2</li>
     </ul>
</div>

```
