---
layout: post
title:  "Fixing bugs !"
tags: codepen
categories: codepen
---

* TOC
{:toc}


1.首页的背景视频

```
注释掉了两行代码
<!-- <div id="forside_canvas"> -->
<!-- </div> -->
```


2./dist/css  /dist/img 

```
site.baseurl 有问题
site.baseurl 最后不带/，需要自行添加/assets/img/...
路径已基本上修改完毕
```


3.page页面 mix odd 和 mix class

```
使用cycle liquid语法
```

4.测试移动端会消失

```
原因同5，done
<span id="menuToggle">
menuToggle_Meny.svg
</span>
```


5.首页内容右侧会超出边界

```
meny元素
done 注释标签之前不闭合
```


6.body class 标签放置位置

```
问题已解决，class放在最底层的layout中，contact、playground、post、default等多个布局样式
<!-- <body> -->
<body class="arbeid footer-pull ">

</body>
```

