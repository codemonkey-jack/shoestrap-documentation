---
layout: post
title: Shoestrap Filters
---
<div class="row">
	<ul class="side-nav">

		<li><label>Filters</label></li>
		{% for post in site.categories.filters. %}
			<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
		{% endfor %}

	</ul>
</div>