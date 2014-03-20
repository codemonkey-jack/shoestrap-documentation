---
layout: post
title: Shoestrap Actions
---
<div class="row">
	<ul class="side-nav">

		<li><label>Actions</label></li>
		{% for post in site.categories.actions. %}
			<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
		{% endfor %}

	</ul>
</div>