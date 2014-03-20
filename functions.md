---
layout: post
title: Shoestrap Functions
---
<div class="row">
	<ul class="side-nav">

		<li><label>Functions</label></li>
		{% for post in site.categories.functions. %}
			<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
		{% endfor %}

	</ul>
</div>