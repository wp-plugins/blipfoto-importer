# Blipfoto importer

A WordPress plugin to import journal entries and photos from [Blipfoto](https://www.polaroidblipfoto.com) into a WordPress website.

Blipfoto is an online daily photo journal. Each day you can upload one photo and add some words. It is also an extremely friendly community where people comment on and rate each other's photos, choose favourite 'blips' (the informal name given to journal entries), follow journals, join groups and take part in discussions.

Blipfoto Importer lets you easily import all your photos and journal entries from Blipfoto into your WordPress website. Each imported entry will create a post on your website and set the photo to be the 'featured image'. You can choose the post status (published, draft, private, or pending review) and, if you wish, automatically insert the image into the post content.

## Important notes

This plugin was initially written extremely quickly in response to uncertainty over the future of the Blipfoto website. Please treat it as very much a 'beta' product.

Feedback, feature requests and bug reports are all very welcome (please use the [support forum](https://wordpress.org/support/plugin/blipfoto-importer) or the [GitHub issues page](https://github.com/lumpysimon/blipfoto-wordpress-importer/issues)).

I would strongly advise that you make a back up of your database before using this plugin.

There appears to be no way to retrieve original high resolution images from Blipfoto, so this plugin retrieves the 'standard' size image instead. This is still good enough for display on most websites, but it is not your original full size image that you uploaded to Blipfoto.

## Instructions

1. Go to the 'Blipfoto Importer' settings page (under the Settings menu).
2. In a new tab or window, go to the [Blipfoto apps page](https://www.polaroidblipfoto.com/developer/apps)
3. Click the 'Create a new app' button.
4. Enter your name.
5. Choose 'web application'.
6. Type anything in the description field.
7. Enter the address of your website in the 'Website' field.
8. Leave the 'Redirect URI' field blank.
9. Click the 'I agree' checkbox.
10. Copy the 'Client ID', 'Client secret' and 'Access token' into the relevant fields on the settings page on your WordPress website.
11. Set the other options as required.
12. To run the import, go to the 'Blipfoto Importer' page in the 'Tools' menu. The import is run in batches to prevent timeouts or exceeding the Blipfoto API rate limit. Just keep hitting the 'Go!' button until all your entries have been imported.
13. If you hit the Blipfoto API rate limit (about 500 entries), put your feet up with a nice cup of tea and try again in about 15 minutes.

## Known bugs and future plans

See the [GitHub issues](https://github.com/lumpysimon/blipfoto-wordpress-importer/issues).

## Changelog

### 1.1.3 (18th March 2015)

* More readme changes

### 1.1.2 (16th March 2015)

* Improved instructions

### 1.1.1 (16th March 2015)

* Use 'post' method for the import form to avoid long URLs

### 1.1 (16th March 2015)

* Make it compatible with PHP versions below 5.4
* Option to insert images into post content
* Various bug and typo fixes

### 1.0 (16th March 2015)

* Initial release
