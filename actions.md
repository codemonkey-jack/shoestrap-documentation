---
layout: post
title: Shoestrap Actions
---

The Shoestrap theme includes a lot of actions that you can use to insert your own custom content or trigger actions at different events during a page load.

What are Actions?
<blockquote>Actions are triggered by specific events that take place in WordPress, such as publishing a post, changing themes, or displaying an administration screen Action is a custom PHP function defined in your plugin (or theme) and hooked, i.e. set to respond, to some of these events.</blockquote>

You can read more about how to use WordPress filters by reading the [WordPress codex](http://codex.wordpress.org/Plugin_API#Actions).

<hr>

You can find a list of the available actions below:

<ul class="side-nav">

	<li><label>Actions</label></li>
	{% for post in site.categories.actions. %}
		<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}

</ul>