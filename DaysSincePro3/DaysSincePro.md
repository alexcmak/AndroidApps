## Days Since Pro 3
The first version of [Days Since Pro](https://play.google.com/store/apps/details?id=com.alexcmak.dayssincepro) was released on Sep 18, 2016 as a replacement to the app's predecessor *Days Since Lists*, which was launched even earlier. Days Since Lists was designed for Android 2.0 and was created with a very early way of creating android apps through an Eclipse plugin. Days Since Pro is a free app and has hundreds of users from all over the world.  

Users can enter any number of life events and the app simply tell you have many days since that event or how many days until the event. The app let the user organize in categories, and present the data in several formats.

Each entry is stored on your phone in a [SQLite](https://www.sqlite.org/) data file. The data file is stored in a place where even if you plug in your phone and use it as an USB device, you still cannot find it in Windows Explorer.

An android phone is good for about 3 years. What happens to the entries that were created by the user? How can the entries get to the new phone?

## Auto Backup for Apps

Modern android apps support [auto backup](https://developer.android.com/guide/topics/data/autobackup). Days Since Pro has auto backup enabled. On your new phone, if you find the app from Google Play again, your data *should* already be there.

## Backup and Restore

Some users has reported that auto backup did not work. There is a work around. 

There is a *Back Up* menu item in on the app. Use that to export the database file (daysSince.db) in a directory where you can retrive it and store in you PC. 
Plug in your new phone with a USB cable and set as File Transfer.

You should be able to locate the database file in a folder like this, 

![screenshot](https://github.com/alexcmak/AndroidApps/blob/main/DaysSincePro3/internal_shared_storage_dsp.png)


Copy that file in your computer.

## Restore (Replace data from file)

Plug in the new phone, transfer the daysSince.db file to the new phone. 
For Android 11 and newer, you need to place the file into the only directory that the app can access.


*Restore* menu item to find it.
