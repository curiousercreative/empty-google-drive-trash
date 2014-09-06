empty-google-drive-trash
========================

!!!!! USE AT YOUR OWN RISK !!!!!

Utilizes Google Drive SDK and API to sort through your Google Drive trash and permanently delete all files that aren't Google Docs. It will take a very long time if you have lots of files in your trash. This is a no-frills app that you should monitor via a web console to make sure it's working.

This app uses the javascript API to:
1. Gain FULL access (via client authorization) to your Google Drive
2. Retrieve a full list of files that are currently in the trash (1000 files per request, requested in serial)
3. Filter out all Google Docs and permanently delete the remaining files (3 file delete requests/second to avoid excessive request rate limit)

You will need to register an app with Google and add your application's client ID in order to authenticate. Lots of information here: https://developers.google.com/drive/web/ and specifically for creating a Google app for authorization here: https://developers.google.com/drive/web/about-auth
