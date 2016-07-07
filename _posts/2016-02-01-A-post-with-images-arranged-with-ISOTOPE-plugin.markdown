---
layout:     post
title:      "ISOTOPE"
subtitle:   "A post with images arranged with ISOTOPE plugin"
image:
  feature: "pc007.jpg"
date:       2016-02-01 
author:     "owner_name"
header-img: "img/postcover/pc007.jpg"
tags: [tag04]
categories: [cat04]
comments: false
images:
 - image_path: /img/journal/post01.jpg
   caption: IMAGE TITLE
   copyright: © photorama
 - image_path: /img/journal/post02.jpg
   caption: IMAGE TITLE
   copyright: © photorama
 - image_path: /img/journal/post03.jpg
   caption: IMAGE TITLE
   copyright: © photorama
---


<html class="no-js" lang="en">
<head>
	<meta content="charset=utf-8">
</head>

    <body>

<section id="content" role="main">
		<div class="wrapper">
	<br><br>
			<h2>{{page.title}}</h2>




<p> Content of your post HERE </p>

<p> Add as many paragraphs amongst your galleries as you want. </p>

<p> Add as many galleries as you want, including as many photos as you want. Simply edit the <b>FRONT MATTER</b> of the post, adding the corresponding <b>path</b>, <b>caption</b> and <b>copyright</b> info for each one of your photos. </p>
			



           <!-- Gallery __-->
			<div class="gallery masonry-gallery">
		
{% for image in page.images %}  		

				<figure class="gallery-item">
					<header class='gallery-icon'>

<a href="{{ site.url }}{{ site.baseurl }}{{ image.image_path }}" class="popup"  title="{{ image.caption }}" data-caption="{{ image.copyright }}">
<img src="{{ site.url }}{{ site.baseurl }}{{ image.image_path }}"></a>
						
					</header>	
					<figcaption class='gallery-caption'>
						<div class="entry-summary" id="{{ image.caption }}">
							<h3>{{image.caption}}</h3>
							<p>{{image.copyright}}</p>
						</div>
					</figcaption>
				</figure>
				
{% endfor %}

			</div><!-- end of GALLERY __ -->



		</div><!-- end of WRAPPER __ -->
	</section>


Photography by: <a href="https://unsplash.com/photos/j0g8taxHZa0">UNSPLASH</a>