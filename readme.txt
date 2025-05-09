=== Reusable Admin Panel ===
Contributors: polyplugins
Tags: admin, developer, developer tool, extendable admin, beautiful admin
Requires at least: 4.0
Tested up to: 6.8
Stable tag: 1.0.7
Requires PHP: 5.4
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl-3.0.html

A settings class to help developers easily add beautiful admin pages and handle getting, sanitizing, and saving options.

== Description ==

<img src="https://www.polyplugins.com/plugins/reusable-admin-panel/preview.gif" alt="Reusable Admin Panel Preview" />

Our goal was to create a reuseable admin panel that can be used by various plugins without having to build or include classes of the same code in multiple plugins, while at the same time being quick to setup.

View our [Documentation](https://www.polyplugins.com/docs/reusable-admin-panel/) to see a list of fields and their parameters.

You can also download our [example plugin](https://www.polyplugins.com/reusable-admin-panel-example-plugin/) to get up and running as quick as possible.

Have suggestions? Submit a Pull Requests via [Github](https://github.com/PolyPlugins/Reusable-Admin-Panel).

Features:

* Bootstrap
* Font-Awesome Field Info Buttons and Sidebar Info Helper
* jQuery Dynamic Navigation
* Validation using validator.js
* Automatic sanitization and saving of options
* Method built to easily get individual options
* Settings Grouped Under One Option in Database (Saved as Multi-Dimensional Array)
* Bootstrap Spinner Preloader (Prevents Layout Shifting on Load)
* Removes notices from other plugins when displaying admin panel
* Prevent users from deactivating by displaying a [sweetalert2](https://sweetalert2.github.io) to deactivate the plugin using the dependency.

Fields:

* Switch
* Text
* Textarea
* Email
* URL
* Password
* Number
* Dropdown
* Date
* Time
* Color
* Dropdown Toggle - Additional fields can be added under a dropdown which show/hide based on selected option
* Button - Add multiple buttons that can link or be targeted in custom JS


== Installation ==

1. Backup WordPress
1. Upload the plugin files to the `/wp-content/plugins/` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress


== Frequently Asked Questions ==

= Who is this built for? =

This is purely for developers to help streamline their development process by making it easier to produce a settings page for their plugins.


== Screenshots ==

1. Plugin Panel
2. Plugin Panel expanded with help sidebar
3. Warning on deactivation

== Changelog ==

= 1.0.7 =

* Added: Ability to pass label attribute for those that don't want the default assigned name
* Added: An optional step, min, and max attribute to number field
* Added: Textarea rows attribute to allow larger height textarea
* Added: Placeholder attribute to text, textarea, email, url, password, number, date and time fields
* Added: Documentation for field usage to polyplugins.com/docs/reusable-admin-panel/
* Added: Security enhancements
* Updated: The color field to use sanitize_hex_color instead of sanitize_text_field
* Bugfix: The "disabled" parameter was not available in dropdown type
* Bugfix: Dropdown Toggle not setting equal label widths correctly
* Bugfix: Support configuration is suppose to be optional
* Bugfix: If type is left out of config, it provides no error.
* Bugfix: If name is left out of config, it provides no error.

= 1.0.6 =

* Added: Textarea input
* Added: Callback to handle errors. Used when conditionally adding fields and needing an error to display.
* Bugfix: URL to have example url as placeholder instead of label
* Bugfix: Dropdowns to have Select Option as placeholder instead of the label

= 1.0.5 =

* Updated: Removed plugin name from panel h2
* Updated: Options panel to have a minimum height based on the height of tabs
* Bugfix: Labels for input-group-text not resizing properly
* Optimization: Restructured settings.js to be more readable

= 1.0.4 =

* Updated: Label styling to be next to the field for a cleaner look
* Bugfix: Tab indexing
* Bugfix: Handling of multiple fields for dropdown toggle
* Bugfix: Dropdown field not full width

= 1.0.3 =

* Added: dropdown_toggle field can add additional fields under a dropdown which show/hide based on selected option
* Added: Support for button fields
* Added: Support for custom JS to take advantage of button fields and other custom needs
* Added: Ability to use SweetAlert2 function in custom js
* Added: Plugin name to section titles
* Added: Ability to add classes to fields
* Optimized: Sanitization method
* Bugfix: Scroll to top on info button click

= 1.0.2 =

* Bugfix: Warning on initial activation
* Bugfix: Bootstrap 5 toggle button not displaying

= 1.0.1 =

* Bugfix: Default logo not showing if config is not set

= 1.0.0 =

* Initial Release

