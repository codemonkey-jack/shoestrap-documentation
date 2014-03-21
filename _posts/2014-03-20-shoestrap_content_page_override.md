---
layout: action
title:  "shoestrap_content_page_override"
category: actions
permalink: actions/shoestrap_content_page_override
---

This will skip loading the [templates/content-page.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content-page.php) file, allowing us to replace it with our own custom template.

### Example:

```php
<?php

function my_custom_page_content() {

	while ( have_posts() ) : the_post();
		
		the_content();

		echo '<div class="clearfix"></div>';

	endwhile;

}
add_action( 'shoestrap_content_page_override', 'my_custom_page_content' );

?>
```

<hr>

* Location: [page.php](https://github.com/shoestrap/shoestrap/blob/master/page.php)