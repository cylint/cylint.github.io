---
layout: post
categories: gallery
title: "Friends at STEC"
tags: [gallery]
---



<center>
        <div class="photoset-grid-lightbox" data-layout="212">
        <img src="{{site.url}}/images/stec/sm-cgz.jpg">
        <img src="{{site.url}}/images/stec/sm-mawei.jpg">
        <p>人在塔在 德玛西亚</p>
        <img src="{{site.url}}/images/stec/sm-renyong.jpg">
        <p>潇洒帅气</p>
        <img src="{{site.url}}/images/stec/sm-yts.jpg">   
        <img src="{{site.url}}/images/stec/sm-wq-zjl.jpg">        
		<p>我的好兄弟  ——  一曲肝肠断</p>
    </div>
</center>




<script src="/assets/js/jquery.photoset-grid.js"></script>

<script src="/assets/js/jquery.colorbox.js"></script>

<script type="text/javascript">
$('.photoset-grid-lightbox').photosetGrid({
  highresLinks: true,
  rel: 'withhearts-gallery',
  gutter: '5px',

  onComplete: function(){
    $('.photoset-grid-lightbox').attr('style', '');
    $('.photoset-grid-lightbox a').colorbox({
      photo: true,
      scalePhotos: true,
      maxHeight:'90%',
      maxWidth:'90%'
    });
  }
});
</script>