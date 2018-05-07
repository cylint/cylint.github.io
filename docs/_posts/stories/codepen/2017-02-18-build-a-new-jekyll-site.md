---
layout: post
title:  "build a new jekyll site"
tags: codepen
categories: codepen
---




新的网站分享我的一些旅行经历。

```
<script src="//cdn.bootcss.com/modernizr/2010.07.06dev/modernizr.js"></script>
```

### 分类如下

城市猎人：

北京市
```
后海、颐和园、圆明园、故宫、鸟巢、水立方、长城
```
上海市
```
五大景点
```
杭州市
```
西湖、太子湾公园、西溪湿地、运河广场、湘湖、灵隐寺
```
黄山市
```
黄山、翡翠谷爱情石、温泉
```
苏州市
```
留园、苏州博物馆、拙政园
```
临安市
```
清凉峰
```
广州市
```
中山公园、大和山、珠江新城
```
佛山市
```
清晖园、宝灵寺、文塔公园
```
万州区
```
移民广场、心连心广场、西山公园、奥体中心、高笋塘广场、万州二中、万州三中
```
重庆市
```
峡谷、磁器口、朝天门、渣滓洞、重庆大学
```
丽江市
```
丽江古城、玉龙雪山、苍山洱海、
```
昆明市
```
观音峡谷茶马古道
```

大理市
```
少数民族
```
武汉市
```
东湖公园、湖北省博物馆、武汉大学
```


### 遇到几个问题：

1.首页的背景视频不能播放了，当我注意到的时候，我已经做了很多修改，不知道是哪里出错。

可能原因是某个标签不全，或者是加了空格。

2.在分页中，不从总/dist/css  /dist/img 目录去查找.css和.jpg

3.page页面 mix odd 和 mix class 按奇偶顺序排列，在循环的时候不知道怎么解决。


```
https://stefanimhoff.de/2014/gulp-tutorial-1-intro-setup/
```


按照示例网站的内容，修改成Jekyll site。

### 已完成部分工作，接下来要做的事情：

- 1.修复首页视频上面的一层div

```
<div id="forside_canvas">

</div>
```


- 2.修改contact的表格




3.修改footer的联系信息

```
done
```

- 4.修改contact页面信息

```
_data 增加联系信息

for 循环调用

```


5.修复category-playground、category-arbeid左右显示问题



```
done

{% comment %}

{% for p in site.categories.playground %}

输出cycle值 {% cycle 'one', 'two', 'three' %}

{% cycle '<article class="mix odd">', '<article class="mix">' %}

{% endfor %}

{% endcomment %}
```

- 6.修复category-arbeid标签分类问题

7.修复footer样式在某些情况下不显示样式的问题

```
done
footer_bg-left.svg
不能用 adobe illustator 编辑，需要寻找一个新的编辑器。
```

- 8.修复page页面视频自动播放时，播放控件闪烁问题

- 9.修复arbeidsmetodikk页面上下平滑滚动问题

- 10.修复 favicon 有重叠样式问题

- 11.重新选用一个 site logo

- 12.重新整理 post 头文件，传递至category页面显示图片和标题


### 需要优化问题

- 1.post页面尽量减少 html class 的书写，优化成 markdown 格式

- 2.为 contact category page 重新设定 layout

- 3.script 语句放到单独文件调用

- 4.整理 .css .js 其中有一项错误需要解决

5.增加 browsersync ，不必频繁刷新和F12

```
done
https://nvbn.github.io/2015/06/19/jekyll-browsersync/
```


- 6.contact页面有地图信息，替换map为国内支持




### 其他需要注意

- 使用代码格式化工具，会将部分标签删掉，需要留意。


```
/assets/
<image ></image>
```



