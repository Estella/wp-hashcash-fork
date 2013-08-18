=== WP-Hashcash Reloaded ===
Contributors: ecb29, donncha, Mike_Koepke
Tags: spam, antispam, anti-spam, comments, comment, pingback, trackback, wp-hashcash, plugin, security, wordpress, javascript, js, signup, sign-up, wp-login.php, wp-signup.php, buddypress, bp, WPMU
Requires at least: 3.3
Tested up to: 3.6
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Client-side javascript blocks all spam bots. XHTML 1.1 compliant.

== Description ==

= No More Spam =

WP-Hashcash Reloaded is an antispam plugin that eradicates comment spam on WordPress blogs. It works because your visitors must use obfuscated javascript to submit a proof-of-work that indicates they opened your website in a web browser, not a robot. If the javascript check fails, WP Hashcash now gives you three options; it can either put the comment into moderation (default), put the comment in the akismet queue, or delete it.

This is a forked version of the original WP-Hashcash plugin by [Elliott Back](ttp://elliottback.com).

You can read more about the original version at the [WP Hashcash plugin](http://wordpress-plugins.feifei.us/hashcash/) page.

= Features =

1. Blocks all comment spam, but not real comments
2. Also prevents most trackback / pingback spam
3. Also protects signup pages for WordPress (WP), BuddyPress (BP), and WordPress Multi-User (WPMU)
4. Widget support to display spam statistics and edit the configuration
5. Works with IE, Firefox, Chrome, and Safari
6. 100% standards compliant XHTML 1.1, works with jQuery and Prototype
7. Tested with WordPress 3.6, Firefox, Safari, IE, and Chrome
8. Akismet compatibility

= Limitations =

WP Hashcash relies on the presence of two hooks in your theme, `wp_head` and `comment_form`. If your theme doesn't include these actions, you will need to add them immediately before the end head and end form tags respectively.

== Installation ==

= Installation Instructions =

1. To install WP-Hashcash, please download the plugin and unzip it, then copy the wp-hashcash.php file to wp-content/plugins.

= Notes =

If you are upgrading from a previous version of WP-Hashcash, please disabled the plugin, then delete its files entirely.  Then, upload the latest plugin files and activate!


== Changelog ==

= 4.7.2 =

- Renamed to WP-Hashcash Reloaded

= 4.7.1 =

- WP 3.6 compat

= 4.7 =

* WP 3.5 compat
* Changed over from wpmu implementation to WP super_admin

= 4.6 =
* Removed links from the blog linking back to Hashcash homepage to comply with WordPress.org plugin guidelines. Props Ryan Hellyer.

= 4.5.1 =
* Fix a javascript error

= 4.5 =
* Support clean interoperation with jQuery and Prototype
* Protect BuddyPress (BP) signup pages

= 4.4 =
* Admin users can now comment from Dashboard
* Tested on WP 2.9.2 in Chrome, IE, and FF
* Fix a potential JS error

= 4.1 =
* Added a new options page under Options, Wordpress Hashcash
* Fixed XHTML standards compliance
* Added validation options for pingbacks and trackbacks (stolen from here)
* Added a logging option for moderated comments

= 4.0.5 =
* Added an option for handling comments via moderation, the akismet queue, or deletion
* Removed database dependencies
* Removed error message for hash fail
* Added the noscript tag for users without javascript
* Corrected the widget formatting
* Changed zip file format from winrar to 7zip, hopefully it will be more compatible

= 4.0.4 =
* Removed version checking
* Removed an unnecessary link element in the head section

= 4.0.3 =
* Suppress errors on loading remote version by any method
* Fix typo-bugs everywhere affecting the widget reporting, date checking, etc
* Strip tags from remote version
* Try various methods to get remote version, ignore if we can't open sockets
* Fix a bug with one of the javascripts
