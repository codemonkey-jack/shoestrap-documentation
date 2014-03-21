---
layout: action
title:  "shoestrap_in_article_top"
category: actions
permalink: actions/shoestrap_in_article_top
---

Using the `shoestrap_in_article_top` action we can inject custom content at the top of the content for single posts and custom post types, right before the title.

### Example:

```php
<?php

function my_custom_top_content() {
	echo 'This content will appear at the very top of all posts';
}
add_action( 'shoestrap_in_article_top', 'my_custom_top_content' );

?>
```

<hr>

* Location: [templates/content.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content.php)