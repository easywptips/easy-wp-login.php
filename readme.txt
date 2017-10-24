=== Easy wp-login.php ===

Contributors:      @easywptips
Tags:              Easy, login, wp-login, wp-login.php, custom login url, admin Dashboard, wp-login change
Requires at least: 4.4
Tested up to:      4.4.1
Stable tag:        2.5.5
License:           GPL-2.0+

Change wp-login.php to anything you want.

== Description ==

**I don't offer support through the support forum. Use [GitHub](https://github.com/easywptips/easy-wp-login.php) instead.**

*Easy wp-login.php* is a very light plugin that lets you easily and safely change wp-login.php to anything you want. It doesn’t literally Easy or change files in core, nor does it add rewrite rules. It simply intercepts page requests and works on any WordPress website. The wp-admin directory and wp-login.php page become inaccessible, so you should bookmark or remember the url. Deactivating this plugin brings your site back exactly to the state it was before.

= Compatibility =

All login related things such as the registration form, lost password form, login widget and expired sessions just keep working.

It’s also compatible with any plugin that hooks in the login form, including

* BuddyPress,
* TML,
* UserPro,
* bbPress,
* Limit Login Attempts,
* and User Switching.

Obviously it doesn’t work with plugins that *hardcoded* wp-login.php.

Works with multisite, but not tested with subdomains. Activating it for a network allows you to set a networkwide default. Individual sites can still Easy their login page to something else.

If you’re using a **page caching plugin** you should add the slug of the new login url to the list of pages not to cache.

If you wish, you can block wp-login.php with `.htaccess` from now on.

== Installation ==

1. Go to Plugins › Add New.
2. Search for *Easy wp-login.php*.
3. Look for this plugin, download and activate it.
4. The page will redirect you to the settings. Easy wp-login.php there.
5. You can change this option any time you want, just go back to Settings › Permalinks › Easy wp-login.php.

== Frequently Asked Questions ==

= I forgot my login url!  =

Either go to your MySQL database and look for the value of `rwl_page` in the options table, or remove the `Easy-wp-login` folder from your `plugins` folder, log in through wp-login.php and reinstall the plugin.

On a multisite install the `rwl_page` option will be in the sitemeta table, if there is no such option in the options table.

== Changelog ==

= 1.0 =

* Adding New feature
* Initial version.
