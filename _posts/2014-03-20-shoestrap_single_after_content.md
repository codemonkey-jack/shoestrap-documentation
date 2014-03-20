---
layout: action
title:  "shoestrap_single_after_content"
category: actions
permalink: actions/shoestrap_single_after_content
---

This action can be used to add content on single posts, right after `the_content()`.

### Example:

```php
<?php

// Insert content using the 'shoestrap_single_after_content' action.
function custom_content_shoestrap_single_pre_content() {

	echo '<p>This content will be added on all posts.</p>';
	echo '<p>The content will be located AFTER the main post content.</p>';

}
add_action( 'shoestrap_single_after_content', 'custom_content_shoestrap_single_top' );

?>
```

<hr>

* Location: [templates/content-single.php](https://github.com/shoestrap/shoestrap-3/blob/development/templates/content-single.php)