=== maksuturva-for-woocommerce ===
Contributors: maksuturva
Tags: maksuturva, payment gateway
Requires at least: 4.0
Tested up to: 4.4.2
Stable tag: 2.0.0
WC requires at least: 2.2.10
WC tested up to: 2.5
License: LGPL v. 2.1 or later
License URI: https://www.gnu.org/licenses/lgpl-2.1.html

Maksuturva payment module for WooCommerce.

== Description ==

Copyright (C) 2016 Maksuturva Group Oy

This library is free software; you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either version 2.1 of the License, or (at your option) any later
version. [GNU LGPL v. 2.1 @gnu.org] (https://www.gnu.org/licenses/lgpl-2.1.html)

This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for
more details.

> Contact information:
Maksuturva Group Oy
Keilaranta 5
02150 Espoo
Finland
e-mail: info@maksuturva.fi

Maksuturva Group Oy, hereby disclaims all copyright interest in the library 'maksuturva-for-woocommerce'
written for Maksuturva Group Oy

[http://www.maksuturva.fi](http://www.maksuturva.fi/)

== Changelog ==

= 1.0.0 =
* Initial release

= 2.0.0 =
* Complete re-factoring of the plugin surce code to follow WordPress and WooCommerce standards and best practices.
* Issue #1: on_uninstall, do_background_checks is too generic global functions.
The plugin now uses classes and the function names have been renamed.
* Removed the eMaksut option from plugin administration, and always send "Y" as value for the "escrow" field.
Maksuturva handles this mode internally, and the setting in the plugin has no effect.
* The plugin now creates a separate row for additional fees (e.g. invoicing fee) added to orders in Maksuturva service.
The fee is shown as an extra row in the order both on the receipt and the administration interface.