Bing Wallpaper for Mac (and now Ubuntu!)
========================================

Information
-----------
A script which downloads the latest picture of the day from Bing.com and saves
it to a directory.

The script was tested in Mac OS X 10.8.2 and 10.8.3.

[Blog entry](http://blog.ideasftw.com/2012/12/bing-desktop-for-mac.html)

How to use?
-----------
* Just run the **bing-wallpaper.sh** script from the terminal. The script will
download the bing image.
* If desired, change the default **PICTURE_DIR** in **bing-wallpaper.sh** to the
wallpaper directory. If left unchanged the default value is
**~/Pictures/bing-wallpapers/**.
* Open Mac's `System Preferences` -> `Desktop & Screensaver`, add the wallpaper
directory, and configure to taste.

Tools
-----
* To have the script run everyday automatically you will need to setup launchd
(Mac only, for Ubuntu see below). I have provided a sample plist file, found in
the Tools directory, which can be copied to **$HOME/Library/LaunchAgents** and
loaded with the command `launchctl load
$HOME/Library/LaunchAgents/com.ideasftw.bing-wallpaper.plist`. Modify the plist
as needed to point to **bing-wallpaper.sh**. For more information on configuring
launchd [see here](http://blog.ideasftw.com/2013/02/run-script-from-launchd-instead-of-cron.html).
* Another option on Mac (and arguably a little simpler) is to set the Calendar
app to run the **Tools/Bing Wallpaper.app** [at a recurring daily time](http://blog.ideasftw.com/2013/03/use-mac-calendar-and-automator-to-run.html).
Modify the app (from within Automator) as needed to point to **bing-wallpaper.sh**
and the correct **PICTURE_DIR**.

Ubuntu (Linux)
--------------
Steps to configure are identical to the Mac version except for the following:

* Change the path of **bing-wallpaper.sh** in **Tools/bing-cron** to the script
location. If left unchanged the default value is **~/Pictures/bing-wallpaper.sh**.
* From the terminal run `crontab /path/to/bing-cron` to setup the cronjob.

The Ubuntu script was tested in Ubuntu 12.10 and 13.04.

Acknowledgement
---------------
Original script by ktmud can be found at [https://github.com/ktmud/bing-wallpaper](https://github.com/ktmud/bing-wallpaper).
