---
layout: action
title:  "shoestrap_include_files"
category: actions
permalink: actions/shoestrap_include_files
---

The `shoestrap_include_files` action will allow you to include files in the theme's functions.php file. This way if you're building a plugin or theme and want to take advantage of shoestrap's framework you can be sure that the theme core files have been loaded prior to your own custom code.

### Example:

This function is from our [Shoestrap EDD Child Theme](http://shoestrap.org/downloads/shoestrap-3-edd-child/):

```php
<?php

/**
 * Include our custom files after the theme core files and framework
 */
function shoestrap_edd_include_files() {

	// Only include our files if Easy Digital Downloads exists
	if ( class_exists( 'Easy_Digital_Downloads' ) ) {

		require_once dirname( __FILE__ ) . '/lib/class-Shoestrap_EDD.php';
		require_once dirname( __FILE__ ) . '/lib/checkout-template.php';
		require_once dirname( __FILE__ ) . '/lib/login-register.php';
		require_once dirname( __FILE__ ) . '/lib/edd-shortcodes.php';
		require_once dirname( __FILE__ ) . '/lib/edd-widgets.php';
		require_once dirname( __FILE__ ) . '/lib/addons/edd-simple-shipping.php';
		require_once dirname( __FILE__ ) . '/lib/addons/edd-variable-pricing-switcher.php';

	}

}
add_action( 'shoestrap_include_files', 'shoestrap_edd_include_files' );

?>
```

<hr>

* Location: [functions.php](https://github.com/shoestrap/shoestrap-3/blob/master/functions.php).