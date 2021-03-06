# Google Drive Scripts

Contains scripts for use with Google Drive artifacts.

## listFilesInFolder.script

It can sometimes be difficult to maintain duplicate files in a Google Drive folder. There is also no good 
current way to simply get a list of files as an export, along with other common filesystem operations. For example, 
if you have two folders with similar contents, files with the same filename may be duplicated. 
The file [`listFilesInFolder.script`](https://github.com/colossus9/google-drive-tools/blob/master/scripts/listFilesInFolder.script)
will attempt to create a list of files in a particular Google Drive folder to help you identify duplicates.

To use the script:

1. Navigate to the root of your Google Drive
1. Click on **New > Google Sheets**
1. Name the spreadsheet `listFilesinFolder`
1. Click on **Tools > Script editor**
1. In the new script window, copy and paste the contents of [`listFilesInFolder.script`](https://github.com/colossus9/google-drive-tools/blob/master/scripts/listFilesInFolder.script)
1. Click **File > Save** and save the project as `listFilesInFolder.script`
1. Close the script window to go back to the spreadsheet
1. In cell A1, type the following formula and press **Enter**:

    ```
    =listFilesInFolder("PictureArchive")
    ```

