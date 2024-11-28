## Days Since Pro 3 - End of Support 

Days Since Pro 3 is now out of the Google Play Store. (Nov 2024)
Google makes it difficult for the individual programmer to post apps and demand just too much personal information. My google app store is closed (by Google).

Days Since Pro 3.1.5 published in Oct 4 2023 was the final version. 

**Unfortunately when you upgrade your phone you will not be able reinstall the app.**

Thank you all for suggestions and input for the fairly successful app that ran on over 10,000 devices and were on most continents.

## Old, obsolete but interesting information

The following information was all true before my app store is closed.

### Days Since Pro 3

The first version of [Days Since Pro](https://play.google.com/store/apps/details?id=com.alexcmak.dayssincepro) was released on Sep 18, 2016 as a replacement to the app's predecessor *Days Since Lists*, which was launched even earlier. Days Since Lists was designed for Android 2.0 and was created with a very early way of creating android apps through an Eclipse plugin. Days Since Pro is a free app and has hundreds of users from all over the world.  

Users can enter any number of life events and the app simply tell you have many days since that event or how many days until the event. The app let the user organize in categories, and present the data in several formats.

Each entry is stored on your phone in a [SQLite](https://www.sqlite.org/) data file. The data file is stored in a place where even if you plug in your phone and use it as an USB device, you still cannot find it in Windows Explorer.

An android phone is good for about 3 years. What happens to the entries that were created by the user? How can the entries get to the new phone?



### Auto Backup for Apps 

Modern android apps support [auto backup](https://developer.android.com/guide/topics/data/autobackup). Days Since Pro has auto backup enabled. 

Before you start using a new phone, you should go to Settings | System | Backup on your old phone to back up data to the cloud.

On your new phone, when you find the app from Google Play again, your data *should* already be there.

In most cases, you do not need to worry about backup and restore.

### Backup and Restore

Some users has reported that auto backup did not work. There is a work around. 

There is a *Back Up* menu item in on the app. Use that to **export the database file** (daysSince.db) in a directory where you can retrive it and store in you PC. 
Plug in your new phone with a USB cable and set as File Transfer.

You should be able to locate the database file in a folder like this:

![screenshot](https://github.com/alexcmak/AndroidApps/blob/main/DaysSincePro3/internal_shared_storage_dsp.png)

The **db** file is not a Microsoft Access file, it is a SQLite file. If you are interested you can download [SQLite browser](https://sqlitebrowser.org/) and open the file if you wish to examine its contents.

Copy that file in your computer.

### Restore (Replace data from file)

Older Android phones:

The restore function will bring up a browser, you can navigate the file system and find your database file.

For Android 11 and newer, you need to place the file into the only directory that the app can access. See figure above.


Plug in the new phone, transfer the daysSince.db file to the new phone. 


A Choose your file dialog appears, *daysSince.db* should appear. If you pick that, the data is replaced.


