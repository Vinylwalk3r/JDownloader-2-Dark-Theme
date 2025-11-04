# JDownloader 2 Dark Theme
After seeing so many requests for a dark theme, I configured my own. 
It uses the "Black Eye" UserInterfaceSetting and a matching colorscheme I configured for the rest of the window.

I have not found anywhere it looks strange or where you cant read the text. **Edit The Menu Customizer has some troubles with text in selected fields not being readable...

I hope someone finds good use for it :)

- [Installing](#installing)
   - [The Dark Theme](#dark-theme)
   - [Adding Green Progress Bar](#adding-custom-assets)
- [Notes and Oddities](#notes-and-oddities)
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
7. Copy the content of the [config](config/) folder into the opened backup. If asked, confirm overwriting exisiting files. ([laf](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/laf) is the dark theme, [menus_v2](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/menus_v2) are the toolbars, [images](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/themes/standard/org/jdownloader/images/) are the white icons) 
8. Save the modified backup, if your archiver does not to that automatically.
9. Go to `File -> Backup -> Restore Settings` and choose the modified backup.
10. JD2 will restart now.

>! If your running Mac OSX and want the top bar to follow the dark theme, run this command in a terminal:
```defaults write org.jdownloader.launcher NSRequiresAquaSystemAppearance 0``` (Thanks @elliotttate for supplying the command!)

Thanks to @L0sha for figuring out this next step!
11. You will notice that every other row is hard to read, as said in [issue #16](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/issues/16). To fix this, we need to replace the file [org.jdownloader.settings.GraphicalUserInterfaceSettings.json](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/org.jdownloader.settings.GraphicalUserInterfaceSettings.json) in "./cfg". 
If you don't want to replace your Settings.json file, find and change this line in that file and you've fixed it `"packagesbackgroundhighlightenabled": false,`. Or, if you want to go the GUI route, go into `Settings -> Settings` and  then `Advanced` and search for `Background`. Look for the setting `GraphicalUserInterfaceSettings: Packages Background Highlight` and untick that box. Then restart JD2.

Now you got a Dark theme for JD2!

### Adding Custom Assets
This will require us to dig a little deeper.
1. Go to `pathtoyourjdownloaderinstall\libs\laf`
2. Make a copy of `syntheticaBlackEye.jar` and paste in the same directory
3. In this example, we rename `syntheticaBlackEye.jar` to `syntheticaBlackEye.jar.bak` (you could edit any theme you want, but you have to use the exact name of the theme you replace. This time, I edited the Blackeye)
4. Choose which version of the [progressbar images](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(progressbar)) you wish to use. (If you want an animation, edit them individually, each image is one frame of the animation. If you only want a solid color or still image, just edit one image and then make copies and rename them accordingly so JD2 can show them)
5. Now open our .jar file with a program like WinRAR or 7Zip. NOT THE BACKUP .JAR!!!
6. Navigate in the file to `/de/javasoft/plaf/synthetica/blackeye/images/`
7. Paste our edited progressbar images here. Overwrite the once already there. 

7.1. This is also where you can paste the [flatbuttons](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(flatbutton))
7.2 If you don't like the blue outline JD2 uses to show the focused section, paste the [focusbutton](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(focusbutton)) to get a nice dark outline instead.

8. Close 7Zip and restart JD2

Your Done! Well done, have a cookie ^^
Many thanks to @Bims0n for creating both the dark and green animated progress bars and also the dark outlines!


## Notes and Oddities
* I've found the images used (and imo, OVERUSED) by JDownloader 2 to be either in the theme .jar file or in the directory `.\themes\standard\org\jdownloader\images`. 

* Strange thing I found, if I pasted a new theme.jar file here, with its own name, JD2 could not find it in its list of themes. Anybody know where the file containing the theme list is?

## Assets_List
- [Main Dark Theme](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/laf)
- [Reorganized Toolbars](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/config/cfg/menus_v2)
- [Green Download Progress bar](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(progressbar))
- [Flat and Unglossy Buttons](https://github.com/Vinylwalk3r/JDownloader-2-Dark-Theme/tree/master/themeNameHere.jar/de/javasoft/plaf/synthetica/blackeye/images/(flatbutton))

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
