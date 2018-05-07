---
layout: post
categories: posts
title: Panorame-Viewer
tags: [sample post]
---

<script>
// Use $(window).load() on live site instead of document ready. This is for the purpose of running locally only
  $(document).ready(function(){
  $(".panorama").panorama_viewer({
    repeat: true
  });
	});
	
</script>


<div class="panorama">
<img src="{{site.url}}/images/panorama/demo_photo.jpg">
	<div class="credit">
	 Photo by DAVID ILIFF. License: CC-BY-SA 3.0
	</div>
</div>

<div style="clear:both"></div>


### Basic Usage

```
http://www.thepetedesign.com/demos/panorama_viewer_demo.html

https://github.com/peachananr/panorama_viewer
```

You can now display your panorama photos on your site with this plugin. To do this, first you have to include the latest jQuery library together with jquery.panorama_viewer.js and panorama_viewer.css into your document's <head>. Now all you have to do this add your image to your HTML like this:

```
<div class="panorama">
 <img src="your-panorama.jpg">
 ...
</div>
```
Make sure to change the source of the image to your image and call the function as shown below:


```
$(".panorama").panorama_viewer({
repeat: false,              // The image will repeat when the user scroll reach the bounding box. The default value is false.
direction: "horizontal",    // Let you define the direction of the scroll. Acceptable values are "horizontal" and "vertical". The default value is horizontal
animationTime: 700,         // This allows you to set the easing time when the image is being dragged. Set this to 0 to make it instant. The default value is 700.
easing: "ease-out",         // You can define the easing options here. This option accepts CSS easing options. Available options are "ease", "linear", "ease-in", "ease-out", "ease-in-out", and "cubic-bezier(...))". The default value is "ease-out".
overlay: true               // Toggle this to false to hide the initial instruction overlay
});
```
