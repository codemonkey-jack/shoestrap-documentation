---
layout: filter
title:  "shoestrap_section_class_primary"
category: filters
permalink: filters/shoestrap_section_class_primary
---

Allows us to change or add classes to the primary sidebar

### Example:

#### Adding a class:

```php
<?php

function my_custom_class( $class ) {
	return $class . ' my-class';
}
add_filter( 'shoestrap_section_class_primary', 'my_custom_class' );

?>
```

#### Replacing the default class(es) with our own:

```php
<?php

function my_custom_class() {
	return 'my-class';
}
add_filter( 'shoestrap_section_class_primary', 'my_custom_class' );

?>
```