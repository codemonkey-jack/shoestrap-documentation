---
layout: action
title:  "shoestrap_entry_meta"
category: actions
permalink: actions/shoestrap_entry_meta
---

The `shoestrap_entry_meta` action is in the `content`, `content-single` and `content-page` templates, right after the title.

It is used to add the meta-data and the featured images, but can also be used to inject your own custom content.

### Example:

```php
<?php

function my_custom_entry_meta() {
	echo 'This content will appear wherever meta-data are displayed';
}
add_action( 'shoestrap_entry_meta', 'my_custom_entry_meta' );

?>
```

<hr>

* Location: [content.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content.php), [content-single.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content-single.php), [content-page.php](https://github.com/shoestrap/shoestrap/blob/master/templates/content-page.php)