---
layout: action
title:  "shoestrap_searchform_override"
category: actions-deprecated
permalink: deprecated/shoestrap_searchform_override
---

The `shoestrap_searchform_override` action has been deprecated since Shoestrap 3.2

Instead of this action, please use the WordPress [`get_search_form`](https://codex.wordpress.org/Function_Reference/get_search_form) filter.

### Example of the get\_search\_form filter:

```php
<?php

function my_custom_get_search_form( $form ) {
	$form = '';
	ss_locate_template( '/templates/searchform.php', true, false );
	return $form;
}
add_filter( 'get_search_form', 'my_custom_get_search_form' );

?>
```

Please note that on the above example we're using the [`ss_locate_template`](/functions/ss_locate_template) shoestrap-specific function.