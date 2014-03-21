---
layout: action
title:  "shoestrap_content_override"
category: actions
permalink: actions/shoestrap_content_override
---

Using the `shoestrap_content_override` action we can override the content of individual posts inside the loop in post archives.

### Example:

```php
<?php

function my_shoestrap_content_override() {
	echo 'This is my custom content';
}
add_action( 'shoestrap_content_override', 'my_shoestrap_content_override' );

?>
```

<hr>

* Location: [index.php](https://github.com/shoestrap/shoestrap/blob/master/index.php)