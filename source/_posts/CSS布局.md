---
title: CSS布局
date: 2019-05-26 16:43:21
tags:
---
# CSS常用布局简介
## 一、左右布局
* 目前我使用较多的左右布局方法有两种：<br/>
* float实现左右布局<br/>
* position:absolute左右布局<br/>
***
1. 通过float实现左右布局
* 给需要左右布局的元素加上"float: left"、"float: right"
* 给左右布局的元素的父级元素加上"class='.clearfix'"，避免下一部分的内容自己跳到横向排列后面来<br/>
".clearfix::after{
    content: '';
    display: block;
    clear: both;"
***
2. 通过position:absolute左右布局
* 给需要左右布局的元素加上"position: absolute;"
* 给左右布局的元素的父级元素加上"position: relative;"
* 通过分别调整两个元素的"left""top"属性来实现左右布局
* 例如：<br/>
左——"style='left: 0px;top: 0px'"<br/>
右——"style='left: 645px;top: 0px'"
## 二、左中右布局
* 与左右布局的第二种方法类似，通过"top""left""right"三个属性调整左中右三个元素的位置来达到左中右的布局方式
* 给中间的元素加上"position: relative;",并设置对应的左右"margin"
* 给左右两边的元素加上"position: absolute;"
* 例如：<br/>
左——"style='left: 0;top: 0'"<br/>
中——"style='margin: 0px 190px 0 190px'"<br/>
右——"style='right: 0;top: 0'"<br/>
***
* 通过左元素: float: left; 右元素: float: right; 中间元素:自动填充的方法
* 设置中间元素的左右两边margin宽度
## 三、水平居中
1. 要水平居中对齐一个元素(如 <div>), 可以使用"margin: auto;"
* 设置元素的宽度将防止它溢出到容器的边缘,元素通过指定宽度，并将两边的空外边距平均分配
* 例如：<br/>
".center{
    margin: auto;
    width: 50%;
    }"
2. 文本在元素内居中对齐，可以使用"text-align: center;"
## 四、竖直居中
1. 通过设置上下"padding"来实现竖直居中
* 例如：<br/>
".center {
    padding: 70px 0;
    border: 3px solid green;
}"
2. 使用"line-height"
* 设置子元素的line-height值等于父元素的height，这种方法适用于子元素为单行文本的情况。
## 五、CSS的小技巧
* 在<span>中添加"word-break: break-all"使内联元素中的英文单词可以被打断自动换行
* 在<div>中添加"display: inline-block"使块级元素可以填充上一行的空隙（类似"float"的效果）
* 块级元素的子元素宽度默认为父级元素的100%
* 以一个冒号开头的是伪类，以两个冒号开头的是伪元素