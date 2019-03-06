# JDownloader 2 Dark Theme
After seeing so many requests for a dark theme, I configured my own. 
It uses the "Black Eye" UserInterfaceSetting and a matching colorscheme I configured for the rest of the window.

I have not found anywhere it looks strange or where you cant read the text. **Edit The Menu Customizer has some troubles with text in selected fields not being readable...

I hope someone finds good use for it :)

- [Installing](#installing)
- [Assets List](#assets_list)
- [Gallery](#gallery)

## Installing

### Dark theme
This method will keep your current settings and add dark theme ontop
(SOOO many thanks to [Georgeto](https://github.com/Georgeto) for this alternative method! Awesome work man!)
1. Go to `Settings -> Settings` and select the `Advanced Settings` category from the list on the left.
2. Enter `LookAndFeelTheme` into the search field.
3. Only the setting `GraphicalUserInterfaceSettings: Look and Feel Theme` should remain. Set its value to `BLACK_EYE`.
4. Go to `File -> Backup -> Backup all settings` and make a backup of your JDownloader settings.
5. Make a copy of the backup, because we are going to modify it in the next step.
6. Open the backup with the zip archiver of your choice (e.g. [7-Zip](https://www.7-zip.org/)).
7. Copy the content of the [config](config/) folder into the opened backup. If asked, confirm overwriting exisiting files. ([laf](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/laf) is the dark theme, [menus_v2](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/menus_v2) is the toolbars) 
8. Save the modified backup, if your archiver does not to that automatically.
9. Go to `File -> Backup -> Restore Settings` and choose the modified backup.
10. JD2 will restart now.

Now you got a Dark theme for JD2!

### Custom Themes
If you want a custom theme (our edited BlackEye for example)
1. Go to `pathtoyourjdownloaderinstall\libs\laf`
2. In this example, we rename `syntheticaBlackEye.jar` to `syntheticaBlackEye.jar.bak` (you could edit any theme you want, but you have to use the exact name of the theme you replace. This time, I edited the Blackeye)
3. Paste our edited [syntheticaBlackEye.jar](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/syntheticaBlackEye.jar) here
4. Restart JD2

Strange thing I found, if a pasted a new theme.jar file here, with its own name, JD2 could not find it in its list of themes. Anybody know where the file containing the theme list is?

## Assets_List
- [Main Dark theme conf](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/laf)
- [Reorganized Toolbars](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/menus_v2)
- [Green Download Progress bar](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(progressbar))
- (soon to be released) "Flat and Unglossy" style buttons (currently: Beta branch)

## Gallery:

### UI

Download tab

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/Download.JPG?)

Linkgrabber tab

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/Linkgrabber.JPG?)

Settings page

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/SettingsTab.JPG?)

### Mac

(Thanks to [elliotttate](https://github.com/elliotttate) for this part!)
![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/blob/master/images/OSXDownload.png)
To get the top bar to show up with the dark theme, you'll also need to run this in terminal: 
``defaults write org.jdownloader.launcher NSRequiresAquaSystemAppearance 0``

### Reorganised Toolbars

Downloads

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/DownloadsToolbar.JPG?)

Linkgrabber

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/LinkgrabberToolbar.JPG?)

### Custom Stuff

Green Progressbar

![Must have taken a wrong turn :/ ](https://github.com/Vinylwalk3r/Jdownloader-2-Dark-Theme/blob/master/images/GreenProgressBar.JPG?)
