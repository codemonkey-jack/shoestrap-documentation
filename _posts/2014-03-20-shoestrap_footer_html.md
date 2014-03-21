---
layout: action
title:  "shoestrap_footer_html"
category: actions
permalink: actions/shoestrap_footer_html
---

The `shoestrap_footer_html` action can be used to inject custom content (like copyright info and social links) inside the footer area.

### Example:


```php
<?php

function my_custom_footer_html() {
	echo 'This content will be visible inside the footer.';
}
add_action( 'shoestrap_footer_html', 'my_custom_footer_html' );

?>
```

<hr>

* Location: [lib/footer.php](https://github.com/shoestrap/shoestrap/blob/master/lib/footer.php)