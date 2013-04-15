hidaayat-browser
================

Islamic branch of the sermon browser wordpress plugin

Original Plugin Name: Sermon Browser
Original Plugin URI: http://www.sermonbrowser.com/
Original Description: Upload sermons to your website, where they can be searched, listened to, and downloaded. Easy to use with comprehensive help and tutorials.
Author: Mark Barnes
Version: 0.45.4
Author URI: http://www.4-14.org.uk/

Copyright (c) 2008-2011 Mark Barnes

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

The structure of this plugin is as follows:
===========================================
MAIN FILES
----------
sermon.php     - This file. Contains common functions and initialisation routines.
admin.php      - Functions required in the admin pages.
frontend.php   - Functions required in the frontend (non-admin) pages.

OTHER FILES
-----------
ajax.php       - Handles AJAX returns.
dictionary.php - Translates the template tags into php code. Used only when saving a template.
filetypes.php  - User-editable file, which returns the correct mime-type for common file-extensions.
php4compat.php - Small number of functions required for PHP4 compatibility
podcast.php    - Handles the podcast feed
sb-install.php - Used only when installing the plugin for the first time
style.php      - Outputs the custom stylesheet
uninstall.php  - Removes the plugin and its databases tables and rows
upgrade.php    - Runs only when upgrading from earlier versions of SermonBrowser

If you want to follow the logic of the code, start with sb_sermon_init, and trace the Wordpress actions and filters.
The frontend output is inserted by sb_shortcode