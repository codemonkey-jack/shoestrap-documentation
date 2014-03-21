---
layout: action
title:  "shoestrap_page_after_content"
category: actions
permalink: actions/shoestrap_page_after_content
---

Using the `shoestrap_page_after_content` action we can inject custom content at the bottom of the content of single pages.

### Example:

```php
<?php

function my_custom_page_after_content() {
	echo 'This is my custom content';
}
add_action( 'shoestrap_page_after_content', 'my_custom_page_after_content' );

?>
```

<hr>

* Location: [templates/content-page.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content-page.php)