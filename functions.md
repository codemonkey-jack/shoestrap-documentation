---
layout: full-width
title: Shoestrap Functions
---

<hr>

You can find a list of the available functions below:

<ul class="inline-list">

	<li><label class="button small primary disabled">Functions:</label></li>
	{% for post in site.categories.functions. %}
		<li><a class="button small secondary" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}

</ul>
