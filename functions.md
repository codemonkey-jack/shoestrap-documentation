---
layout: post
title: Shoestrap Functions
---

Below is a list of functions that the Shoestrap theme contains:

<ul class="side-nav">

	<li><label>Functions</label></li>
	{% for post in site.categories.functions. %}
		<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}

</ul>