---
layout: function
title:  "shoestrap_section_class"
category: functions
permalink: functions/shoestrap_section_class
---

```php
<?php shoestrap_section_class( $target, $echo ); ?>
```
This function allows us to change the width of the sidebars and the main content.

Returns (or echoes depending on the value of the 2nd argument) the classes of the element that interests us. The element is defined by the `$target` parameter.

`$target`: (string) can be one of the following:
* main
* primary
* secondary
* wrapper

`$echo`: (boolean)

### Example:

If we want to echo the classes of the primary sidebar we can use the following:

```php
<?php shoestrap_section_class( 'primary', true ); ?>
```

<hr>

* Location: [lib/config.php](https://github.com/shoestrap/shoestrap-3/blob/development/lib/config.php)