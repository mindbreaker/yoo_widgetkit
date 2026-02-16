# Widgetkit (PHP 8 Fork) #

- Original version: 1.4.5 (June 2013)
- Original author: YOOtheme GmbH (http://www.yootheme.com)
- PHP 8 port: [mindbreaker](https://github.com/mindbreaker)

## About this fork

This is a **PHP 8 compatible fork** of YOOtheme Widgetkit 1.4.5.

The original plugin has not been maintained since 2013 and is no longer functional under PHP 8. Widgetkit 1.x is no longer supported by YOOtheme, and migrating to Widgetkit 2.x or 3.x would require recreating all widgets from scratch. I ported 1.4.5 to PHP 8 instead, because I needed it for the **[yoo_tasty](https://github.com/mindbreaker/yoo_tasty)** WordPress theme, which was also ported to PHP 8.

### Changes from original

- Fixed `DOMElement` method signatures to match PHP 8.1 interface requirements (return types)
- Updated `WP_Widget` constructors to use modern `__construct()` syntax
- Replaced deprecated `create_function()` calls with anonymous functions (closures)
- Made implicitly nullable parameters explicitly nullable (`?Type`)
- Fixed static vs. non-static method calls
- Resolved various PHP 8 deprecation warnings
