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
```
### Example Output ###
------------
```html
<div class="nav-menu">
	<ul>
		<li><a href="http://devsite.dev/blog/">Blog</a></li>
		<li><a href="http://devsite.dev/cart/">Cart</a></li>
		<li><a href="http://devsite.dev/front-page/">Front Page</a></li>
		<li><a href="http://devsite.dev/image-store/">Image Store</a></li>
		<li class="active"><a href="http://devsite.dev/sample-page/">Sample Page</a></li>
		<li><a href="http://devsite.dev/secure-images/">Secure Images</a></li>
		<li><a href="http://devsite.dev/about/">About The Tests</a>
			<ul>
				<li><a href="http://devsite.dev/about/page-image-alignment/">Page Image Alignment</a></li>
				<li>
					<a href="http://devsite.dev/about/page-markup-and-formatting/">Page Markup And Formatting</a>
				</li>
				<li><a href="http://devsite.dev/about/clearing-floats/">Clearing Floats</a></li>
				<li><a href="http://devsite.dev/about/page-with-comments/">Page with comments</a></li>
				<li>
					<a href="http://devsite.dev/about/page-with-comments-disabled/">Page with comments disabled</a>
				</li>
			</ul>
		</li>
		<li><a href="http://devsite.dev/level-1/">Level 1</a>
			<ul>
				<li><a href="http://devsite.dev/level-1/level-2/">Level 2</a>
					<ul>
						<li><a href="http://devsite.dev/level-1/level-2/level-3/">Level 3</a></li>
						<li><a href="http://devsite.dev/level-1/level-2/level-3a/">Level 3a</a></li>
						<li><a href="http://devsite.dev/level-1/level-2/level-3b/">Level 3b</a></li>
					</ul>
				</li>
				<li><a href="http://devsite.dev/level-1/level-2a/">Level 2a</a></li>
				<li><a href="http://devsite.dev/level-1/level-2b/">Level 2b</a></li>
			</ul>
		</li>
		<li><a href="http://devsite.dev/lorem-ipsum/">Lorem Ipsum</a></li>
		<li><a href="http://devsite.dev/page-a/">Page A</a></li>
		<li><a href="http://devsite.dev/page-b/">Page B</a></li>
	</ul>
</div>