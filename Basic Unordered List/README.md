Basic Unordered List
=====================

Usage
------------
Update your `wp_nav_menu()` function to use this walker class by adding a "walker" item to the wp_nav_menu array.

```php
 <?php
	wp_nav_menu(
		array(
			'menu'              => 'menu_id',
			'theme_location'    => 'menu_location_id',
			'container'         => 'div',
			'container_class'   => 'my-menu',
			'container_id'      => 'my-menu-id',
			'menu_class'        => 'nav-class',
			'walker'            => new Basic_Unordered_List()
		)
	);
?>