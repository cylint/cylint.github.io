---
layout: default
title: Bridges crossing Huanghe
subtitle: „Huanghe is the longest in China next to the Yangtse River“
permalink: /bridges-crossing-huanghe/
image: langzhou-zhongli.jpg
description: 描述.
author: zhang
scripts: [ekko-lightbox.js, video.js]
---		
<section class="story-header-image">
		
	<!-- image -->  
	<img src="{{site.img}}/header/{{page.image}}" class="img-responsive" alt="{{ page.title }}"/>  
	<!-- description div -->  
	<div class="story-header-image-description">  
		<span class="subdescr">
			{{ page.title }}
		</span> 
		<div class="clearfix">&nbsp;</div>
		<span class="descr">
			{{ page.subtitle }}
		</span>  
		
	</div>
</section>			

<section id="kapitel1">
	
	<article class="teaser no-comment" style="padding-top: 35px;">

			<p>
				<em>{{ page.description }}</em>
			</p>
			<p class="credits no-comment">
			{% assign author = site.authors[page.author] %}
				<strong><em>Text</em></strong> <span style="text-transform: uppercase;">{{ author.display_name }}</span> | <strong><em>Bilder und Videos</em></strong> <span style="text-transform: uppercase;">{{ author.display_name }}</span> and <span style="text-transform: uppercase;">Carolyn Wißing</span>, 2016/08/26<br />
			</p>
		
	</article>



	





	<article style="padding-top: 35px;">
		
		
	<p>又是一段文字。
		</p>
	</article>
	


	
<!-- 评论留言的功能打不开？ -->
	<article class="comments">
		<p>评论留言的功能打不开？</p>
		{% include comments.html inline="true" %}
	</article>
		
</section>

<section id="anmerkungen">

	<article class="full" style="padding-right: 25px;">					

		<h4>备注</h4>
		<p>
			桥的
		<br />
		联系作用
		</p>
		
	</article>
		
</section>