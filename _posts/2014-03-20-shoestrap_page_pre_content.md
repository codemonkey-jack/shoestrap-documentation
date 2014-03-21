---
layout: action
title:  "shoestrap_page_pre_content"
category: actions
permalink: actions/shoestrap_page_pre_content
---

Using the `shoestrap_page_pre_content` action we can insert custom content at the top of the content of single pages, right below the title and the meta-data of the post.

Our content will be inserted before `the_content()`.

### Example:

```php
<?php

function my_custom_page_pre_content() {
	echo 'This is my custom content';
}
add_action( 'shoestrap_page_pre_content', 'my_custom_page_pre_content' );

?>
```

<hr>

* Location: [templates/content-page.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content-page.php)