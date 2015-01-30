# [WP Admin Buttons](http://wordpress.org/plugins/wp-admin-buttons/) #

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/michaeluno/wp-admin-buttons/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/michaeluno/wp-admin-buttons/?branch=master)

### Welcome to our GitHub Repository

WP Admin Buttons is an open source WordPress plugin that displays buttons with the style used in the WordPress administration area.

## Screenshots ##

<p align="center">
	<a href="https://lh4.googleusercontent.com/-7WYs1W1Rhjg/VMdb3OawCjI/AAAAAAAAB7A/TGaxL_iaC6c/s0/screen-shot-3.png" title="WP Admin Buttons - Sceens shot">
		<img src="https://lh4.googleusercontent.com/-7WYs1W1Rhjg/VMdb3OawCjI/AAAAAAAAB7A/TGaxL_iaC6c/s480/screen-shot-3.png" alt="WP Admin Buttons - Sceens shot" />
	</a>
</p>

<div style="margin:20px; float:left">
	<a href="https://lh4.googleusercontent.com/-UAvhM8C_ut4/VMdUBXOjOWI/AAAAAAAAB6Y/AzdEUzPVczo/s0/screen-shot-2.png" title="WP Admin Buttons - Widget Form">
		<img src="https://lh4.googleusercontent.com/-UAvhM8C_ut4/VMdUBXOjOWI/AAAAAAAAB6Y/AzdEUzPVczo/s144/screen-shot-2.png" alt="WP Admin Buttons - Widget Form" />
	</a>
</div>    

## Installation ##

- The latest development version can be found [here](https://github.com/michaeluno/wp-admin-buttons/branches). 
- The latest stable version can be downloaded [here](http://downloads.wordpress.org/plugin/wp-admin-buttons.latest-stable.zip).

1. Upload **`wp-admin-buttons.php`** and other files compressed in the zip folder to the **`/wp-content/plugins/`** directory.,
2. Activate the plugin through the `Plugins` menu in WordPress.

## Usage ##

### Widget
1. Go to **Dashboard** -> **Appearance** -> **Widgets** and add the **WP Admin Buttons** widget to your proffered sidebar.

### Shortcode and Function Parameters
The following parameters can be used for the shortcode or the PHP function of the plugin, `printWPAdminButto()` or `getWPAdminButtons()`.

- **href** - the link url.

```php
[wp_admin_button href="http://my-download-url/file.zip"]
```

```php
<?php printWPAdminButto( array( 'href' => 'http://my-download-url/file.zip') ); ?>
```

- **label** - the text label shown in the button.

```php
[wp_admin_button label="Get" href="http://my-download-url/file.zip"]
```

```php
<?php printWPAdminButto( array( 'label' => 'Get', 'href' => 'http://my-download-url/file.zip' ) ); ?>
```

- **size** - the button size. This argument accepts either `large`, `medium`, `small`.

```php
[wp_admin_button size="large" href="http://my-download-url/file.zip"]
```

```php
<?php printWPAdminButto( array( 'size' => 'large', 'href' => 'http://my-download-url/file.zip' ) ); ?>
```

- **type** - the button type. This argument accepts either `button-primary`, or  `buton-secondary`.

```php
[wp_admin_button type="button-secondary" href="http://my-download-url/file.zip"]
```

```php
<?php printWPAdminButto( array( 'type' => 'button-secondary', 'href' => 'http://my-download-url/file.zip' ) ); ?>
```

- The follwoing color arguments can override the defult colors.

    - **label_color** - the label text color.
    - **background_color** - the button background color.
    - **border_color** - the button border color.

```php
[wp_admin_button label_color="#ccc" background_color="transparent" href="http://my-download-url/file.zip"]
```

```php
<?php 
printWPAdminButto(
    array( 
        'label_color'       => '#ccc',
        'background_color'  => 'transparent',
        'href'              => 'http://my-download-url/file.zip',
    )
); 
?>
```

- The following additional HTML tag attributes can be set.

    - **title** - the `title` attribute.
    - **class** - the `class` attribute.
    - **style** - the `inline` style attribute.
    - **target** - the `target` attribute.
    - **rel** - the `rel` attribute.

```php
[wp_admin_button title="Get the file now!" class="my-custom-class-selector" "style="text-align:center;" target="_blank" rel="nofollow" href="http://my-download-url/file.zip"]
```

```php
<?php
echo getWPAdminButtons( 
    array( 
        'type'      => 'button-secondary', 
        'title'     => 'Get the file now!',
        'class'     => 'my-custom-class-selector',
        'style'     => 'text-align:center',
        'target'    => '_blank',
        'href'      => 'http://my-download-url/file.zip',
    )
); 
?>
```

## Bugs ##
If you find an issue, let us know [here](https://github.com/michaeluno/wp-admin-buttons/issues)!

## Support ##
This is a developer's portal for WP Admin Buttons and should _not_ be used for support. Please visit the [support forums](http://wordpress.org/support/plugin/wp-admin-buttons).

## Contributions ##
Anyone is welcome to contribute to WP Admin Buttons.

There are various ways you can contribute:

1. Raise an [Issue](https://github.com/michaeluno/wp-admin-buttons/issues) on GitHub.
2. Send us a Pull Request with your bug fixes and/or new features.
3. Provide feedback and suggestions on [enhancements](https://github.com/michaeluno/wp-admin-buttons/issues?direction=desc&labels=Enhancement&page=1&sort=created&state=open).

## Supporting Future Development ##

If you like it, please rate and review it in the [WordPress Plugin Directory](http://wordpress.org/support/view/plugin-reviews/wp-admin-buttons?filter=5). Also donation would be greatly appreciated. Thank you!

[![Donate with PayPal](https://www.paypal.com/en_US/i/btn/x-click-but04.gif)](http://en.michaeluno.jp/donate) 

## Copyright and License ##

### WP Admin Buttons ###
Released under the [GPL v2](./LICENSE.txt) or later.
Copyright © 2014 Michael Uno

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.