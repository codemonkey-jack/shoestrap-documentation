---
layout: function
title:  "shoestrap_title_section"
category: functions
permalink: functions/shoestrap_title_section
---

The `shoestrap_title_section` function returns the title section of the current page.

```php
<?php echo shoestrap_title_section( $header, $element, $link, $class ); ?>
```
* `$header`: boolean. Whether or not we want a `<header>` element wrapping our title. Defaults to `true`.
* `$element`: can be any valid HTML element (h1, h2, h3, div, span etc.). Defaults to `'h1'`.
* `$link`: boolean. Whether or not we want the title linked to the post. (`true`: title is linked. `false`: title is not linked.). Defaults to `false`.
* `$class`: The CSS class of the title. Defaults to `'entry-title'`.

### Example:

```php

<?php echo shoestrap_title_section( true, 'h2', true, 'entry-title' ); ?>
```

The above will echo this HTML:

```html
<header>
	<title>POST TITLE</title>
	<h2 class="entry-title">
		<a href="example.com/post-link">POST TITLE</a>
	</h2>
</header>
```

<hr>

* Location: [lib/titles.php](https://github.com/shoestrap/shoestrap-3/blob/development/lib/titles.php)
* Related: [shoestrap\_title](/functions/shoestrap_title) (function), [shoestrap\_title](/filters/shoestrap_title) (filter).