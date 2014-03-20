---
layout: filter
title:  "shoestrap_title"
category: filters
permalink: filters/shoestrap_title
---

The `shoestrap_title` fuilter can be used to change the output of the [`shoestrap_title`](/functions/shoestrap_title) function.

### Example:

```php
<?php

function custom_shoestrap_title( $title ) {
	return '<span>' . $title . '</span>';
}
add_filter( 'shoestrap_title', 'custom_shoestrap_title' );

?>
```

Output can be filtered using the [shoestrap\_title](/filters/shoestrap_title) filter.

* Location: [lib/titles.php](https://github.com/shoestrap/shoestrap-3/blob/development/lib/titles.php)
* Related: [shoestrap\_title](/filters/shoestrap_title)