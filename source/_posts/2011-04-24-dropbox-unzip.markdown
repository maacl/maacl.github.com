---
layout: post
title: "Dropbox Unzip"
date: 2011-04-24 12:00
comments: true
external-url:
categories: [dropbox, unzip, tool, incron, inotify, osx, ubuntu]
alias: "index.php/2011/04/24/dropbox-unzip/"
---
Inspirer by this [post][1] where the author shows how to add automatic unzipping to a [Dropbox][2] folder on OS X, I wanted to see if something similar was easily achievable on Ubuntu (10.10).

After a bit of searching I found [incron][3]. Quoting from the website incron “is an “inotify cron” system. It consists of a daemon and a table manipulator. You can use it a similar way as the regular cron. The difference is that the inotify cron handles filesystem events rather than time periods.”

To create a folder in your Dropbox that automatically unzips any zip file dropped into it first install incron. It is available in the Ubuntu Universe repository and can be installed using:

    sudo apt-get install incron

After the package is installed you must add the username of all users who should be permitted to add jobs to incron to /etc/incron.allow like this(replace [username] with your username):

    sudo echo “[username]” >> /etc/incron.allow

Next create the unzip folder in your Dropbox folder:

    mkdir [path to your Dropbox folder]/unzip

Next we need to add the actual unzip job row to incron like this:

    icrontab -e

This opens the user incron table in the deafult editor. Insert the following line, replacing [path to your Dropbox folder] with the absolute path (don’t use ~) to your Dropbox folder:

    [path to your Dropbox folder]/unzip IN_CLOSE_WRITE unzip $@/$# -d $@

Check that the job row was added to your incron table:

    incrontab -l

This should output the line you just added above. If this works try copying a zip file into the Dropbox/unzip folder. If everything works it should unzip automatically. This obviously only so long the machine you installed the incron job is online.

   [1]: http://wetzler.me/ios-unzipping/
   [2]: http://www.dropbox.com/
   [3]: http://inotify.aiken.cz/?section=inotify&page=about&lang=en
