---
layout: post
title: Shoestrap Classes
---
<div class="row">
	<ul class="side-nav">

		<li><label>Classes</label></li>
		{% for post in site.categories.classes. %}
			<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
		{% endfor %}

	</ul>
</div>