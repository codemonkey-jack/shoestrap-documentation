---
layout: action
title:  "shoestrap_override_index_loop"
category: actions
permalink: actions/shoestrap_override_index_loop
---

Using the `shoestrap_override_index_loop` action we can override the whole index loop of Shoestrap.

### Example:

```php
<?php

function my_custom_index_loop() {
	while ( have_posts() ) : the_post();
		ss_get_template_part( 'templates/content', get_post_format() );
	endwhile;
}
add_action( 'shoestrap_override_index_loop', 'my_custom_index_loop' );

?>
```

<hr>

* Location: [index.php](https://github.com/shoestrap/shoestrap/blob/master/index.php)