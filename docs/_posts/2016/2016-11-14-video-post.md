---
layout: post

title: A Video Post
tags: [sample post]
date-string: #
---

## 天外飞仙

<embed src='http://player.youku.com/player.php/sid/XMjQ5NDkzMzIwOA==/v.swf' allowFullScreen='true' quality='high' width='960' height='600' align='middle' allowScriptAccess='always' type='application/x-shockwave-flash'><!-- </embed> -->

<script src="/assets/js/jquery.fitvids.js"></script>

<script>
  $(document).ready(function(){
    // Target your .container, .wrapper, .post, etc.
    $(".entry-content").fitVids();
  });
</script>


------


Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).


```html
<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/EqAnYPiZiNA" frameborder="0" allowfullscreen></iframe>
</center>
```

it seems youku midea iframe doesn't work, use embed only.

```html
<iframe height="498" width="510" src='http://player.youku.com/embed/XMjQ5NDkzMzIwOA==' frameborder=0 'allowfullscreen'></iframe>

 <!-- width='960' height='600' -->
```

```javascript
<script src="/assets/js/jquery.fitvids.js"></script>

<script>
  $(document).ready(function(){
    // Target your .container, .wrapper, .post, etc.
    $(".entry-content").fitVids();
  });
</script>
```
