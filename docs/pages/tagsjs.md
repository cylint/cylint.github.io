---
title: tags js
layout: tags
title: Tag Js
excerpt: "An list of posts sorted by tag."
hidelogo: true
search_omit: true
permalink: /tagsjs/
---

<div id='tag_cloud'>
{% for tag in site.tags %}
<a href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="{{ tag[1].size }}">{{ tag[0] }}</a>
{% endfor %}
</div>

<ul class="listing">
{% for tag in site.tags %}
  <li class="listing-seperator" id="{{ tag[0] }}">{{ tag[0] }}</li>
{% for post in tag[1] %}
  <li class="listing-item">
  <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
  <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}" class="listing-item-a">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>

<script src="/assets/js/vendor/jquery-1.9.1.min.js" type="text/javascript" charset="utf-8"></script> 
<script src="/assets/js/tag/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script> 
<script language="javascript">
  $.fn.tagcloud.defaults = {
      size: {start: 1, end: 1, unit: 'em'},
      color: {start: '#c0edf7', end: '#018aaa'}
  };
</script>
