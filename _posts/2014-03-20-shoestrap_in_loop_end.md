---
layout: action
title:  "shoestrap_in_loop_end"
category: actions
permalink: actions/shoestrap_in_loop_end
---

The `shoestrap_in_loop_end` action can be used to inject custom content at the end of the loop, after the content template.

### Example:

```php
<?php

function my_custom_in_loop_end() {
	echo 'This content will appear in the end of the loop';
}
add_action( 'shoestrap_in_loop_end', 'my_custom_in_loop_end' );

?>
```

<hr>

* Location: [index.php](https://github.com/shoestrap/shoestrap/blob/master/index.php)