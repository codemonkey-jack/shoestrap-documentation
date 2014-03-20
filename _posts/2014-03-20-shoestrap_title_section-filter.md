---
layout: filter
title:  "shoestrap_title_section"
category: filters
permalink: filters/shoestrap_title_section
---

Allows changing the title section.

### Example:

```php
<?php

function custom_shoestrap_title_section() {
	return '<header><h1>' . shoestrap_title() . '</h1></header>';
}
add_filter( 'shoestrap_title_section', 'custom_shoestrap_title_section' );
?>
```

<hr>

* Location: [lib/titles.php](https://github.com/shoestrap/shoestrap-3/blob/development/lib/titles.php)
* Related: [shoestrap\_title](/functions/shoestrap_title) (function), [shoestrap\_title](/filters/shoestrap_title) (filter).