---
layout: post
title: Shoestrap Classes
---

Classes are a way to better organize the code in the Shoestrap theme. We are slowly moving towards a more OOP model, so some of the [functions](/functions) currently available in the theme will be slowly migrating in classes.

You can learn more about PHP Classes in the [PHP Manuals](http://www.php.net/manual/en/language.oop5.php).

<hr>

<ul class="side-nav">

	<li><label>Classes in the Shoestrap Theme:</label></li>
	{% for post in site.categories.classes. %}
		<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}

</ul>