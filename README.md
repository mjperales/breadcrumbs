# breadcrumbs

Breadcrumb function for Wordpress

This is allows visitors to quickly navigate back to a previous section or root page.

I have also incorporated custom post types and taxonomies.

This was adopted from <a href="https://github.com/cyberchimps">CyberChimps</a> and the <a href="https://github.com/cyberchimps/responsive">Responsive WordPress Theme</a>
Adopted from <a href="http://dimox.net/wordpress-breadcrumbs-without-a-plugin/">Dimox Plugin</a>

Install:

Paste this function into your `functions.php` file. Make sure you change the `options` section within the function to match your theme.

### Display
Now just paste the code below on each page template that you want breadcrumbs to appear

``` php
	<?php if (function_exists('mjp_breadcrumbs_list')) { mjp_breadcrumbs_list(); } ?>
```

### Style
``` html
	<div class="breadcrumb-list" xmlns:v="http://rdf.data-vocabulary.org/#">

	    <span class="breadcrumb" typeof="v:Breadcrumb">
	        <a href="#" property="v:title" rel="v:url">Home</a>
	    </span>
	    <span class="chevron"></span>
	    <span class="breadcrumb" typeof="v:Breadcrumb">
	        <a href="#">Other Page</a>
	    </span>
	    <span class="chevron"></span>
	    <span class="breadcrumb-current">Other Page</span>

	</div>
```

