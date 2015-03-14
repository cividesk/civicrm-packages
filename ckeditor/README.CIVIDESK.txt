NG, 9/6/2013

This is how you rebuild the ckeditor package with a special configuration:
- Go to: http://ckeditor.com/builder
- Select upload build-config.js and select the latest packages/ckeditor/build-config.js
- Add/remove plugins as needed, then click on Download at the bottom of the page

Then in the file config.js that was downloaded with the above:
- in config.removeButtons, replace 'Underline' with 'Strike'
- in config.removeDialogTabs, remove 'link:advanced';

Add Following line-
  config.allowedContent = true; // Allow copy content with background color (disable the filter)
  config.startupShowBorders = false; // Hide the table border

Don't forget to clear your browser cache since the icon file will have changed!
