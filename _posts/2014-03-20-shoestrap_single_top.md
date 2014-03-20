---
layout: action
title:  "shoestrap_single_top"
category: actions
permalink: actions/shoestrap_single_top
---

This action can be used to add content on single posts, right after the `<article>` element opens.

### Example:

```php
<?php

// Insert content using the 'shoestrap_single_top' action.
function custom_content_shoestrap_single_top() {

	echo '<p>This content will be added on all posts.</p>';
	echo '<p>The content will be located BEFORE the title</p>';

}
add_action( 'shoestrap_single_top', 'custom_content_shoestrap_single_top' );

?>
```

<hr>

* Location: [templates/content-single.php](https://github.com/shoestrap/shoestrap-3/blob/development/templates/content-single.php)