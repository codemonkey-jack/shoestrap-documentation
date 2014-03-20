---
layout: post
title:  "shoestrap_do_the_excerpt"
category: actions
permalink: actions/shoestrap_do_the_excerpt
---

The `shoestrap_do_the_excerpt` action allows you to bypass the_excerpt call that exists in the templates/content.php template file.

Example:

```php
<?php

function custom_replace_excerpt_with_content() {
	the_content();
}
add_action( 'shoestrap_do_the_excerpt', 'custom_replace_excerpt_with_content' );
?>
```

<div data-alert class="alert-box info">
Location: <a href="https://github.com/shoestrap/shoestrap/blob/master/templates/content.php">templates/content.php</a>
</div>