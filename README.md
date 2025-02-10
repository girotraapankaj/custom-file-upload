# custom-file-upload

To use this custom file upload widget in AF v1, do the following steps:


1. Open the adaptive form in edit mode.
2. Open the Property dialog for the file upload field on which you want to apply the custom appearance.
3. In the Styling tab, update the CSS class property to add this `widget_customfileupload`


To modify the custom storage logic for each file upload, please refer to the code here: [custom-fileuploader.js.](https://github.com/rismehta/custom-file-upload/blob/main/src/main/content/jcr_root/etc/clientlibs/custom/custom-fileupload/integration/javascript/custom-fileuploader.js#L36-L157)

When the remove icon is clicked on a file, the following function is called: [custom-fileattachment.js](https://github.com/rismehta/custom-file-upload/blob/main/src/main/content/jcr_root/etc/clientlibs/custom/custom-fileupload/integration/javascript/custom-fileattachment.js#L522). Please implement the logic to remove the file upload from the custom storage accordingly.
