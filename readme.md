Convert Word Documents to HTML
==============================

Cleans up the otherwise-ugly output generated by Microsoft Word when you use the File -> Save As HTML option and optionally includes Twitter Bootstrap. Relies heavily on WordPress's texturize engine and internal encoding functions to do the heavy lifting. It also converts footnotes into a format compatible with Bootstrap's tooltips.

* Normalizes encoding and line endings
* Removes uneccessary tags and attributes, such as inline CSS and extraneous IDs
* Cleans up encoding problems and HTML entities
* Balances tags to ensure valid HTML
* Typesets everything via the Texturize engine
* Converts Word's footnotes into a format compatible with Bootstrap's tooltips
* Strips HTML comments
* Removes consecutive spaces
* Removes empty paragraph tags
* Removes the otherwise-hard word wrap
* Converts `<b>`'s to `<strong>`'s and `<i>`'s to `<em>`'s
* Optionally includes a stand-alone version of Twitter Bootstrap

Screenshot
----------
![Screenshot](https://github.com/benbalter/Convert-Word-Documents-to-HTML/raw/master/screenshot.png)

Requirements
------------

* LAMP Server
* WordPress (uses texturize and kses engines)

Usage
-----

1. Place plugin within server's web root, and adjust the path to `wp-load.php` in the project's `index.php`
1. Open the target file in Microsoft Word
1. Go to "`File`" -> "`Save As Web Page`"
1. Save the file someplace convenient
1. Open `index.php` in your favorite web browser and select the file
1. This script will return the clean up file as a download

Licenese
--------

Licensed under the GNU General Public License Version 3 or later.