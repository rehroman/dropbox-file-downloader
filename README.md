# Dropbox File Downloader

This is a Python script that uses the Dropbox API to download files from a shared Dropbox folder.

## Requirements

- Python 3.6 or above
- `requests` library

You can install the `requests` library using pip:

```
pip install requests
```
## Usage
The script can be run from the command line with the following syntax:

```
python dropbox_download.py -t YOUR_ACCESS_TOKEN -url YOUR_SHARED_FOLDER_LINK
```
Replace YOUR_ACCESS_TOKEN with your Dropbox API access token and YOUR_SHARED_FOLDER_LINK with the URL of the Dropbox folder you wish to download from.

Note: Take the full shared link you received and don't copy the URL from your browser after opening it. There is a "rlkey=" part in it. You can also go into a subfolder, but keep in mind to add the part beginning with "&rlkey" to the URL which is in your web browser.

## Options
The script also supports the following optional arguments:
```
-df, --download_folder: Sets the download folder (default is "downloads").
-c, --count: Sets the number of files to download (default is all files).
-v, --verbose: Prints the full API response.
--h: Displays these information.
```

## Dropbox API information

- https://www.dropbox.com/developers/documentation/http/documentation
