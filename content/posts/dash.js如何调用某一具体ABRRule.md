---
title: "dash.js如何调用某一具体ABRRule（未完）"
subtitle: ""
date: 2021-11-27T09:34:32+08:00
draft: false

summary: "当点击Load之后..."

tags: [前端, AngularJS, 框架理解]
categories: [dash.js]

hiddenFromHomePage: false
hiddenFromSearch: false

featuredImage: ""
featuredImagePreview: ""

license: '<a rel="license external nofollow noopener noreffer" href="https://creativecommons.org/licenses/by-nc/4.0/" target="_blank">CC BY-NC 4.0</a>'
---





## 一、定位：load按钮之后的逻辑

### doLoad(): `./samples/dash-if-reference-player/app/main.js`

选择元素，定位到Load按钮上，它对应的html元素中，`ng-click="doLoad()"`中的ng-click是AngularJS的一种指令，后面跟的是普通的expression表达式，语法规则为：

```html
<element ng-click="expression"></element>
```

<img src="https://gitee.com/tanneho/pic/raw/master/img/202111262228745.png" style="zoom: 80%;" />

即点击就会执行doLoad函数。这个函数定义在main.js中，那么它干了什么呢。这条路我昨天找没找通，是不是应该反过来找啊！