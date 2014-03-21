---
layout: action
title:  "shoestrap_post_main"
category: actions
permalink: actions/shoestrap_post_main
---

The `shoestrap_post_main` action is located in `base.php` between the primary and secondary sidebars.

### Example:

```php
<?php

function my_custom_post_main() {
	echo 'This content will be visible after the main content.';
}
add_action( 'shoestrap_post_main', 'my_custom_post_main' );

?>
```

<hr>

* Location: [base.php](https://github.com/shoestrap/shoestrap/blob/master/base.php)