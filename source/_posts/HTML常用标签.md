---
title: HTML常用标签
date: 2019-05-15 16:24:56
tags:
---
# HTML常用标签简介
## 一、标签
* HTML标签由尖括号包围的关键词构成，比如`<html>`
* HTML标签有成对出现（双标签）的，也有单个出现（单标签）的。
* 例：
`<p>Neuedu，你好！</p>（段落标签）`
`<br/>（换行标签）`

***
* HTML标签对中的第一个标签是开始标签，第二个标签是结束标签。
* HTML标签尽量使用小写，所有单个标签都会以/结束，不要忘记。
## 二、属性
* HTML标签可以拥有属性。属性提供了有关HTML元素的更多信息。
* 属性总是以名称/值得形式出现，比如：name = "value"
* 属性总是在HTML元素的开始标签中规定
* 始终为属性值加引号：双引号是最常用的，不过使用单引号也没问题。
* 例：
  `<a target=xxx href="http://qq.com">qq</a>`
## 三、HTML固定基本结构
* `<html></html> — <html>` 元素。这个元素包含了整个页面的内容，被称为根元素。
* `<head></head> — <head>` 元素。这个元素放置的内容不是展现给用户的，而是包含例如面向搜索引擎的搜索关键字（keywords）、页面描述、CSS 样式表和字符编码声明等。
* `<meta charset="utf-8">` — 这个元素指定了当前文档使用 UTF-8 字符编码 ，UTF-8 包括绝大多数人类已知语言的字符。基本上 UTF-8 可以处理任何文本内容，还可以避免以后出现某些问题。
* `<title></title> — <title>` 元素。这个元素设置页面的标题，显示在浏览器标签页上，同时作为收藏网页的描述文字。
* `<body></body> — <body>` 元素。这个元素包含期望让用户在访问页面时看到的内容，可以是文本、图像、视频、游戏、可播放的音轨或其他内容。
* 例：
`<!DOCTYPE html>`
 `<html>`
  `<head>`
  `<meta charset="utf-8">`
  `<title>XXX</title>`
  `</head>`
  `<body></body>`
 `</html>`
 ## 四、常见HTML标签
 ### `<a>`——锚点
 * 全称：anchor 
  `<a>` 标签定义超链接，用于从一张页面链接到另一张页面。
  `<a>` 元素最重要的属性是 href 属性，它指示链接的目标。
* 用法举例
1. 在新页面打开链接   `<a href="http://qq.com" target="_blank">qq</a>`
2. 在当前页面打开链接   `<a href="http://qq.com" target="_self">qq</a>`
3. 在上级页面打开链接   `<a href="http://qq.com" target="_parent">qq</a>`
4. 在顶层页面打开链接   `<a href="http://qq.com" target="_top">qq</a>`
5. 刷新页面   `<a href=""></a>`
6. 下载链接   `<a href="http://qq.com" download>下载</a>`
7. 打开目录下的文件   `<a href="./xxx.html"></a>`
8. 页面内跳转，不发起请求(href="#"则跳转到页面顶部)   `<a href="#xxx"></a>`
9. 发起GET请求   `<a href="？name=xxx"></a>`
10. 使用当前页面协议（//）   `<a href="//qq.com"></a>`
11. 伪协议，执行JavaScript代码(href="javascript:;"则变为点击之后什么都不做的链接)   `<a href="javascript: alert(1);"></a>`
12. 在iframe嵌套页面内打开链接（frameborder设置边框）
    `<iframe name=xxx src="#" frameborder="0"></iframe>`
    `<a target=xxx href="http://qq.com">qq</a>`
### `<table>`——表格
* 简单的 HTML 表格由 table 元素以及一个或多个 tr、th 或 td 元素组成。
* tr 元素定义表格行，th 元素定义表头，td 元素定义表格单元。
* 例：
`table border="1">`
  `<tr>`
    `<th>Month</th>`
    `<th>Savings</th>`
  `</tr>`
  `<tr>`
    `<td>January</td>`
    `<td>$100</td>`
  `</tr>`
`</table>`

***
待续