=== Official Gumroad Wordpress Plugin ===
Contributors: pderksen, nickyoung87, gumroad
Tags: gumroad, gumroad product pages, gumroad overlay, gumroad embed, ecommerce, e-commerce, pdf, javascript, overlay, embed
Requires at least: 3.9
Tested up to: 4.2
Stable tag: 1.1.9
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Display your Gumroad products right on your Wordpress page.

== Description ==

This plugin lets you embed the Gumroad purchase experience right in your website. You can learn more and see examples here: https://gumroad.com/widgets.

Basic overlay example:
`[gumroad id="DviQY"]`

Basic embed example:
`[gumroad id="GAPdj" type="embed"]`

Overlay that will automatically show the payment form:
`[gumroad id="DviQY" text="Purchase Item" wanted="true"]`

See full the full documentation in Settings > Gumroad after plugin is activated.

Spanish translation by Andrew Kurtis of [webhostinghub.com](http://www.webhostinghub.com/).

[Follow this project on Github](https://github.com/gumroad/WP-Gumroad)

== Installation ==

= 1. Admin Search =
1. In your Admin, go to menu Plugins > Add.
1. Search for `Gumroad`.
1. Find the plugin that's labeled `Gumroad Overlay & Embed`.
1. Look for the author name `Gumroad` on the plugin.
1. Click to install.
1. Activate the plugin.
1. A new menu item `Gumroad` will appear under your Settings menu option.

= 2. Download & Upload =
1. Download the plugin (a zip file) on the right column of this page.
1. In your Admin, go to menu Plugins > Add.
1. Select the tab "Upload".
1. Upload the .zip file you just downloaded.
1. Activate the plugin.
1. A new menu item `Gumroad` will appear under your Settings menu option.

= 3. FTP Upload =
1. Download the plugin (.zip file) on the right column of this page.
1. Unzip the zip file contents.
1. Upload the `gumroad` folder to the `/wp-content/plugins/` directory of your site.
1. Activate the plugin through the 'Plugins' menu in WordPress.
1. A new menu item `Gumroad` will appear under your Settings menu option.

== Frequently Asked Questions ==

Your theme must implement **wp_footer()** in the footer.php file, otherwise JavaScript will not load correctly. You can test if this is the issue by switching to a WordPress stock theme such as twenty-twelve temporarily.

If the overlay doesn't get triggered on click (and your browser is redirected to a gumroad.com URL), please make sure that there is not extra code that is hijacking the click event (for example, a Google Analytics onclick event).

A popular known plugin that does this is "Google Analytics for WordPress". Try unchecking one or both of these options: 1) Track outbound clicks & downloads, 2) Check Advanced Settings, then make sure "Track outbound clicks as pageviews" is un-checked.

See the official Gumroad [overlay](https://gumroad.com/overlay) or [embed](https://gumroad.com/embed) documentation for further troubleshooting.

== Screenshots ==

1. Simple Overlay example

2. Simple Embed example

== Changelog ==

= 1.1.9 - April 25, 2015 =

* Updated calls to add_query_arg to prevent any possible XSS attacks.
* Tested up to WordPress 4.2.

= 1.1.8 =

* Remove note in help about using in template files or theme files.

= 1.1.7 =

* Tested up to WordPress 4.1.

= 1.1.6 =

* Replace all i18n functions with escaped equivalents.
* Simplified load_plugin_textdomain() call.
* Add proper escaping when building the overlay button.
* Removed activation/install notice.
* Removed some now unused functions and files.

= 1.1.5 = 

* Videos added to in-plugin help page.
* Demo videos added to Readme.txt.
* Tested up to WordPress 4.0.

= 1.1.4 =

* Added shortcode attribute to add CSS classes to the overlay link button.

= 1.1.3 = 

* Added locale shortcode attribute.

= 1.1.2 =

* Spanish translation updates.

= 1.1.1 =

* Added Spanish translation (thanks to Andrew Kurtis of [webhostinghub.com](http://www.webhostinghub.com/)).
* Tested up to WordPress 3.9.

= 1.1.0 =

* Added Gumroad embed purchase page option.
* Plugin now uses only shortcodes to display Gumroad overlay or embed.
* Main settings options removed.
* Post meta options removed.
* Tested up to WordPress 3.8.

= 1.0.1 =

* Bug fixes.
* Added settings link to plugin listing entry.
* Added plugin activation notice.
* Added sidebar content to settings page.
* Fixed PHP debug warnings.

= 1.0.0 =

* Initial release.
