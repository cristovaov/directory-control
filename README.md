# Directory Control #

**Contributors:** johnbillion  
**Tags:** developer  
**Requires at least:** 3.5  
**Tested up to:** 3.7  
**Stable tag:** 1.1.1  
**License:** GPL v2 or later 

A WordPress plugin to specify the location of the uploads and themes directories.

## Usage ##

Define the `WP_UPLOAD_DIR`, `WP_UPLOAD_URL`, and `WP_THEME_DIR` constants in your `wp-config.php` file to override the upload directory, upload URL and theme directory respectively.

## Background ##

WordPress does not have a `WP_UPLOAD_DIR` constant. The `UPLOADS` constant does not perform as expected and is always prepended with `ABSPATH`, meaning it is impossible to use a root directory for uploads if WordPress is installed in its own directory. This plugin fixes that by introducing `WP_UPLOAD_DIR` and `WP_UPLOAD_URL` constants. Define these constants in your `wp-config.php` file and their value will override the default upload directory.

WordPress does not have a `WP_THEME_DIR` constant. Themes can only be present in `WP_CONTENT_DIR/themes`. This plugin fixes that by introducing `WP_THEME_DIR` and `WP_THEME_URL` constants. Define these constants in your `wp-config.php` file and their value will override the default theme directory.

---

This plugin was originally commissioned by Daft Media for TheJournal.ie
