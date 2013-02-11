Bing Wallpaper for Mac (and now Ubuntu!)
========================================

Information
-----------
A script which downloads the latest picture of the day from Bing.com and saves it to a directory.

The script was tested in Mac OS X 10.8.2.

[Blog entry](http://blog.ideasftw.com/bing-desktop-for-mac)

How to use?
-----------
* If desired change the default **PICTURE_DIR** in **bing-wallpaper.sh** to the wallpaper directory. If left unchanged the default value is **~/Pictures/bing-wallpapers/**.
* Change the path of **bing-wallpaper.sh** in **bing-cron** to the script location. If left unchanged the default value is **~/Pictures/bing-wallpaper.sh**.
* To have the script run everyday automatically you will need to setup launchd (Mac only, for Ubuntu see below).
* Open Mac's `System Preferences` -> `Desktop & Screensaver`, add the wallpaper directory, and configure to taste.

Ubuntu
------
Steps to configure are identical to the Mac version except for the following:
* From the terminal run `crontab /path/to/bing-cron` to setup the cronjob.

The Ubuntu script was tested in Ubuntu 12.10.


Original script by ktmud can be found at [https://github.com/ktmud/bing-wallpaper](https://github.com/ktmud/bing-wallpaper).
