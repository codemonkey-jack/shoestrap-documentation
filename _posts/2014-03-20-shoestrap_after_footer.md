---
layout: action
title:  "shoestrap_after_footer"
category: actions
permalink: actions/shoestrap_after_footer
---

The `shoestrap_after_footer` action is located in the `base.php` file after the footer div, right before the call to `wp_footer()`.

### Example:

```php
<?php

function my_custom_after_footer() {
	echo 'This content will be visible after the footer.';
}
add_action( 'shoestrap_after_footer', 'my_custom_after_footer' );

?>
```

<hr>

* Location: [base.php](https://github.com/shoestrap/shoestrap/blob/master/base.php)