---
title: home
layout: home
type: parent
order: 1
carousels:
  - images: 
    - image: /img/Cameron Marsh, Back Study, Oil on Canvas, 70x100cm, 2025.jpg
    - image: /img/Cameron Marsh, Etching on copper, 15x20cm, 2025.jpg
    - image: /img/Cameron Marsh, Girl from Perugia, Oil on Canvas, 65x55cm, 2024.jpg
---

<div class="section header">
		<h1 class="title">Cameron Marsh Artwork</h1>
		<div id="navbar-wrapper">
			<div id="navbar" class="close">
				<a onclick="menuExpand()"><img id="brand" class="hide" src="{{ relative_url }}"></a>
				{% assign mypages = site.pages | where: "type", "parent" | sort: "order" %}
				{% for page in mypages %}
				<a class="button" href="{{ page.url | relative_url }}">{{ page.title }}</a>
				{% endfor %}
			</div>
		</div>
</div>

<div class="section main">
	{% include carousel.html height="50" unit="%" duration="7" number="1" %}
</div>