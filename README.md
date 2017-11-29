## Magento 2 theme based on Bootstrap

This is a Magento 2 theme based on Bootstrap.


![Theme Preview](https://github.com/webgriffe/theme-bootstrap/raw/master/media/preview.png)

The theme has been designed to be overridden by project's specific theme.

For example you can override only the `bootstrap-theme.less` and `_variables.less` files to completely customize the look and feel of your theme.

Installation
------------

Add this repository to Composer's repositories and then require the theme:

```
composer config repo.bootstrap-menu vcs https://github.com/webgriffe/module-bootstrap-menu
composer config repo.bootstrap-theme vcs https://github.com/webgriffe/theme-bootstrap.git
composer require webgriffe/theme-frontend-bootstrap "dev-master"
```

Then you should run Magento's setup upgrade:

```
php bin/magento setup:upgrade
```

Now you activate the Bootstrap Theme under `Content -> Design -> Configuration.`.

Lastly clear Magento generated suff and caches:

```
rm -rf pub/static/frontend/
rm -rf var/view_preprocessed/css/frontend/
php bin/magento cache:clean
```

ToDo
----

This theme is still work in progress. Here is a list of done / todo sections:

* ~~Home Page~~
* ~~Category Page~~
* ~~Product Page~~
* Cart
* Checkout
* ~~Login~~
* ~~Signup~~
* Forgot Password
	* ~~Request~~
	* Set Password
* My Account
	* ~~Account Dashboard~~
	* ~~Account Information~~
	* ~~Address Book~~
	* My Downloadable Products
	* ~~My Orders~~
	* My Credit Cards
	* Newsletter Subscriptions
	* Billing Agreements
	* My Product Reviews
	* My Wish List


License
-------

This library is under the MIT license. See the complete license in the LICENSE file.

Credits
-------

Developed by [Webgriffe®](http://www.webgriffe.com/). Please, report to us any bug or suggestion by GitHub issues.
