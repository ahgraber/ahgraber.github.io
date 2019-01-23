---
layout: default
title: Project Portfolio
---
	<h1>{{ page.title }}</h1>
	<ul>
    {% assign projects = site.pages | where: "project", true %}
	  {% for proj in projects %}
	    <li>
			<h3><a href="{{ proj.url }}" title="{{ proj.title }}">{{ proj.title }} </a></h3>
			{{ proj.excerpt | markdownify }}</li>
	  {% endfor %}
	</ul>
