# JDownloader 2 Dark Theme
After seeing so many requests for a dark theme, I configured my own. 
It uses the "Black Eye" UserInterfaceSetting and a matching colorscheme I configured for the rest of the window. 

I have not found anywhere it looks strange or where you cant read the text. **Edit The Menu Customizer has some troubles with text in selected fields not being readable...

I hope someone finds good use for it :)

- [Versions](#versions)
- [Merging_with_Existing_Settings](#merging settings)
- [Clean_Installation](#clean installation)
- [Gallery](#gallery)

## Versions
* JDownloaderDarkOnly - Contains Only the dark theme. No other custom settings included
* JDownloaderDarkCustomToolbars - Same as DarkOnly, only adding a some more organized toolbars (I think they are atleast, but customize away to your prefs!)
* JDownloaderDefault - What it says, all default values, as if a new install

## Merging Settings
(SOOO many thanks to [Georgeto] for this alternative method! Awesome work man!)
1. Go to `Settings -> Settings` and select the `Advanced Settings` category from the list on the left.
2. Enter `LookAndFeelTheme` into the search field.
3. Only the setting `GraphicalUserInterfaceSettings: Look and Feel Theme` should remain. Set its value to `BLACK_EYE`.
4. Go to `File -> Backup -> Backup all settings` and make a backup of your JDownloader settings.
5. Make a copy of the backup, because we are going to modify it in the next step.
6. Open the backup with the zip archiver of your choice (e.g. [7-Zip](https://www.7-zip.org/)).
7. Copy the content of the [config](config/) folder into the opened backup. If asked, confirm overwriting exisiting files.
8. Save the modified backup, if your archiver does not to that automatically.
9. Go to `File -> Backup -> Restore Settings` and choose the modified backup.
10. JD2 will restart now.

## Clean Installation
1. Go to "File -> Backup -> Restore Settings" !!!This step WILL clear ALL custom settings you may have, so backup those!!! (Thanks to  [Chya66](https://www.reddit.com/user/Chya66 "Chya66's Reddit") for pointing this out)
2. Choose the .jd2backup file you just downloaded
3. JD2 will restart

Now you got a Dark theme for JD2!

## Gallery:
(Some custom settings can be seen here. They are NOT included in the backup files!)

The main Download tab
![Sorry, this image cant be viewed :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/Download.JPG?)

The Linkgrabber tab
![Sorry, this image cant be viewed :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/Linkgrabber.JPG?)

And finaly, the Settings
![Sorry, this image cant be viewed :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/SettingsTab.JPG?)




