 
## 2.2.x Series

This series is part of the Stable branch of uGet and started on January 8th, 2018.

**uGet 2.2.0: (2018-01-08)**
1. mega plug-in: create new plug-in for MEGA site.
2. all plug-in: avoid crash if plug-in failed to start.
3. Fix: some category/status doesn’t refresh it’s download list.
4. update translation files.


## 2.1.x Series

This series is part of the Development (or beta) branch of uGet and started on February 20th, 2016.

**uGet 2.1.6: (2017-08-24)**
1. User can use sorting in any category and status.
2. curl plug-in: It can use ftruncate() to create large file.
3. media plug-in: don’t use folder in path if folder == NULL.
4. Fix: uGet doesn’t close File Descriptor when saving config file.
5. Fix: category functions can’t work correctly. (2017-08-27)
6. add translation files.

**uGet 2.1.5: (2017-02-18)**
1. URL Sequence Batch can setup 3 wildcard range.
2. Use character ↓/↑ to replace D:/U: to display speed.
3. avoid configure file corrupted on sudden shutdown.
4. curl plug-in: crashes when download file > 4GB.
5. Fix: program will move download to incorrect position if user switch to offline mode.
6. Fix: Segmentation fault after pressing delete key on gtk window.
7. Fix: Wayland hidden tray.
8. update translation files.

**uGet 2.1.4: (2016-05-16)**
1. In speed limit mode, program adjust existing task speed when adding new task.
2. Add new setting “Display large icon”.
3. Add configure argument “–enable-unix-socket” to use JSON-RPC over UNIX domain socket.
4. use msys2 + mingw to build uGet for windows.
5. curl plug-in: Don’t use CURLAUTH_ANY, it causes authentication failed.
6. Fix: User can’t use command-line to assign config directory (ui-gtk-1to2).
7. (2.1.3-2) Fix: Incorrect encoding on some characters (e.g. French characters)
8. (2.1.3-2) Fix: Program stop download queuing in some case. * uGet for Windows upgrade GTK+ from 3.10.4 to 3.16.6

**uGet 2.1.3: (2016-04-10)**
1. Fix: UI freeze if user activate download in sorted list.
2. Add Keywords entry into desktop file (Elías Alejandro Año Mendoza)
3. update translation files.

**uGet 2.1.2: (2016-04-01)**

1. Revert URI decoder to 2.0.4, it may fix incorrect encoding on some characters.

**uGet 2.1.1: (2016-03-20)**
1. curl plug-in: fix a bug that downloaded file may be incomplete in some case.
2. curl plug-in: improve downloaded segment handler.
3. curl plug-in: set min split size to 10 MiB.
4. curl plug-in: adjust speed if plug-in add/remove segments in speed limit mode.
5. aria2 plug-in: fix a memory leak.
6. media plug-in: report error if YouTube video has been removed. * This version fix bug that download speed is slow when progress near 100% * If you usually get error message “Incorrect source”, I suggest you use this version.

**uGet 2.1.0: (2016-02-20)**
1. Add new media plug-in to get link from media website.
2. if file “uget-portable-mode” exists, data files save in installed folder. (Windows)
3. curl plug-in: avoid showing “99:99:99” in “elapsed” when downloading start.
4. curl plug-in: avoid reporting “Incorrect source” when downloading finished.
5. Fix: Program stop running download when user set “Runnable” to it. * In Windows, If “uget-portable-mode” and “uget.exe” place in the same folder, data files will save in uGet installed folder.


## 2.0.x Series

This series is part of the Stable branch of uGet and started on May 1st, 2015.

﻿**uGet 2.0.11: (2018-01-06)**
1. all plug-in: avoid crash if plug-in failed to start.
2. Fix: some category/status doesn’t refresh it’s download list.
3. update translation files.

**uGet 2.0.10: (2017-08-24)**
1. User can use sorting in any category and status.
2. curl plug-in: It can use ftruncate() to create large file.
3. Fix: uGet doesn’t close File Descriptor when saving config file.
4. Fix: category functions can’t work correctly. (2017-08-27)
5. add translation files.

**uGet 2.0.9: (2017-02-18)**
1. Use character ↓/↑ to replace D:/U: to display speed.
2. avoid configure file corrupted on sudden shutdown.
3. curl plug-in: crashes when download file > 4GB.
4. Fix: program will move download to incorrect position if user switch to offline mode.
5. Fix: Segmentation fault after pressing delete key on gtk window.
6. Fix: Wayland hidden tray.
7. update translation files.

**uGet 2.0.8: (2016-05-16)**
1. In speed limit mode, program adjust existing task speed when adding new task.
2. Add new setting “Display large icon”.
3. Add configure argument “–enable-unix-socket” to use JSON-RPC over UNIX domain socket.
4. use msys2 + mingw to build uGet for windows.
5. curl plug-in: Don’t use CURLAUTH_ANY, it causes authentication failed.
6. Fix: User can’t use command-line to assign config directory (ui-gtk-1to2).
7. (2.1.3-2) Fix: Incorrect encoding on some characters (e.g. French characters)
8. (2.1.3-2) Fix: Program stop download queuing in some case.

– uGet for Windows upgrade GTK+ from 3.10.4 to 3.16.6

**uGet 2.0.7: (2016-04-09)**
1. Fix: UI freeze if user activate download in sorted list.
2. Add Keywords entry into desktop file (Elías Alejandro Año Mendoza)
3. update translation files.

**uGet 2.0.6: (2016-04-01)**
1. curl plug-in: fix a bug that downloaded file may be incomplete in some case.
2. curl plug-in: improve downloaded segment handler.
3. curl plug-in: set min split size to 10 MiB.
4. curl plug-in: adjust speed when plug-in add/remove segments in speed limit mode.
5. curl plug-in: avoid showing “99:99:99” in “elapsed” when downloading start.
6. aria2 plug-in: fix a memory leak.
7. Fix: Program stop running download when user set “Runnable” to it.
8. Revert URI decoder to 2.0.4, this may fix incorrect encoding on some characters.
9. if file “uget-portable-mode” exists, data files save in installed folder. (Windows)

– This version fix bug that download speed is slow when progress near 100%
– If you usually get error message “Incorrect source”, I suggest you use this version.
– In Windows, If “uget-portable-mode” and “uget.exe” place in the same folder, data files will save in uGet installed folder.

**uGet 2.0.5: (2016-02-08)**
1. curl plug-in: Disable SSL verification for host.
2. curl plug-in: Don’t check post and cookie file if no HTTP setting data.
3. curl plug-in: Don’t assign data if plug-in start failed.
4. avoid crash when program re-enter signal handler. (e.g. SIGINT)
5. adjust width of download properties form by width of category chooser.
6. Fix: Can’t stop all task when program into offline mode.

**uGet 2.0.4: (2016-01-01)**
1. save and restore width of download column.
2. adjust schedule form for large font size.
3. in speed limit mode, program adjust speed when downloading start-up.
4. use filename from RPC request to match category if URL doesn’t contain filename.
5. curl plug-in: use posix_fallocate() to preallocate space for a file on Linux.
6. curl plug-in: use SetEndOfFile() to preallocate space for a file on Windows.
7. Fix: program crash when simultaneously download > 32 files.
8. Fix: Can’t save height of summary area.
9. Add compressed 256×256 icon for Windows 7.

**uGet 2.0.3: (2015-11-11)**
1. curl plug-in: update control file path if download file was renamed.
2. curl plug-in: update downloaded size after loading aria2 control file.
3. curl plug-in: update file size when allocating disk space.
4. Don’t show border in right side of setting dialog.

**uGet 2.0.2: (2015-09-11)**
1. curl plug-in: fix memory leak and avoid accessing NULL pointer.
2. curl plug-in: create new file with correct size if file size is not the same.
3. curl plug-in: create new file only in first connection.
4. curl plug-in: change setting’s file name if plug-in created new file.
5. replace invalid characters /:*?”<>| by _ in filename.
6. Don’t resume file with incorrect aria2 control file (no bit field).

**uGet 2.0.1: (2015-08-15)**
01. curl plug-in: create new download file if file size is not the same.
02. curl plug-in: use common user & password by default.
03. curl plug-in: response error if post or cookie file not found.
04. curl plug-in: don’t create aria2 control file if download file create failed.
05. curl plug-in: if error occurred while allocating disk space, delete created download file.
06. curl plug-in: count downloaded size after splitting download. (avoid progress > 100%)
07. avoid crash if user doesn’t specify argument value.
08. When creating folder failed, check folder exists before returning error.
09. When uGet get SIGTERM, it will save settings and call sync() for Linux.
10. check and fix settings after loading Setting.json

**uGet 2.0: (2015-05-01)**
1. All of the features and improvements from 1.91.0 – 1.99.6 are included in 2.0.0
2. Try to ignore some error when parsing JSON file.
3. clipboard monitor add a new file type ‘WEBM’.
4. Adjust main window default size.
5. Add and update translation files.
## 1.9x Series

This series is part of the Development (or beta) branch of uGet and started on May 10th, 2014.

**uGet 1.99.6: (2015-03-25)**
1. provide JSON-RPC over TCP (connect to localhost:14777) **
2. match category by filename if URI doesn’t match.
3. reduce start-up time.
4. Add some items to tray icon menu.
5. category list in dialog use the same width in main window.
6. Fix: command-line argument “–category-index” doesn’t work.

– see “doc/JSON-RPC interface.txt” in Git repo.

**uGet 1.99.5: (2015-01-18)**
1. curl plug-in: report more error (e.g. Failed to create file) after connecting.
2. curl plug-in: avoid crash if filename repeated counts > 999
3. aria2 plug-in: clear uploading flag if aria2 status changed.
4. IPC: program can handle ‘n’ character from command-line. (for FlashGot)
5. adjust main windows default size.
6. restore main window position and size when window presented by command-line (IPC).
7. Enable Individual Download Speed Limiting.
8. Adjust widget layout and color for GTK+ 3.14
9. Add and update translation files.

**uGet 1.99.4: (2014-10-24)**
01. curl plug-in: retry all URI (include mirrors) every time.
02. curl plug-in: response error if file size is different.
03. aria2 plug-in: change lowest speed limit to 128 byte/sec.
04. aria2 plug-in: Don’t change node name If URI scheme is “magnet”.
05. aria2 plug-in: Don’t change URI If URI scheme is “magnet”.
06. aria2 plug-in: Don’t set uploading status if no downloaded data.
07. magnet: get and show name from magnet URI.
08. Adjust layout of Download Form for GTK+ 3.12.
09. Implement multiple wildcards in Sequential Batch.
10. Fix : discard filename option from command-line.

**uGet 1.99.3: (2014-09-06)**
1. use abstract socket in linux by default.
2. change category capacity limit from 9999 to 99999.
3. reduce start-up time.
4. curl plug-in: reset speed if download thread restart.
5. curl plug-in: change file auto rename counts to 10000.
6. curl plug-in: response error if error occur when create large file.
7. Fix: program doesn’t backup cookie or post file from command-line.
8. Fix: user can’t pause some downloading task. 9. Fix: download dialog can’t accept magnet URI.

**uGet 1.99.2: (2014-06-24)**
1. “Enable offline mode on startup” is workable now.
2. Don’t do completion action if user stop download manually.

**uGet 1.99.1: (2014-06-13)**
1. “Start in tray” is workable now.
2. Show confirm dialog when user delete category.

**uGet 1.99.0: (2014-06-07)**
1. Remove speed limit option in download property. Use global speed limit to replace it.
2. “Force start” can work with Scheduler and Offline mode.
3. Force shutdown aria2 on exit even if aria2 tasks running.
4. Fix: Program crashes on exit.
5. restore SSL cipher list to default value.

**uGet 1.97.1: (2014-05-31)**
1. curl plug-in: change SSL cipher and restore default SSL version.

**uGet 1.97.0: (2014-05-31)**
1. Refresh download status when user enable/disable scheduler.
2. change SSL cipher list to avoid “SSLv3 alert handshake failure”.
3. Remove some duplicate strings.
4. Update translation files.

**uGet 1.95.0: (2014-05-24)**
1. curl plug-in: Program must get file timestamp even if file has existed.
2. curl plug-in: Enable infinite retries if retry limit is zero.
3. aria2 plug-in: “max-concurrent-downloads” is global option, don’t use it with gid.
4. aria2 plug-in: add “split” option to avoid less connections if user specify mirrors.
5. aria2 plug-in: global speed limit must set correct value. 6. Remove line breaks from setting of clipboard monitor and aria2 arguments.
6. Add missing Android.mk files.

**uGet 1.93.0: (2014-05-18)**
1. aria2 plug-in: support RPC authorization secret token (Aria2 v1.8.4 new feature)
2. update uGet RSS every 30 minutes.

**uGet 1.91.0: (2014-05-10)**
1. First uGet2 beta version.
## 1.10.x Series

This series is part of the Stable branch of uGet and started on September 7th, 2012.

**uGet 1.10.4: (2014-01-01)**
1. aria2 plug-in support magnet
2. Add GnuTLS support (configure –enable-gnutls)
3. Fix: uGet unexpectedly exits with large list of urls.
4. add and update translation files.

**uGet 1.10.3: (2013-01-23)**
1. Add new download option – “mirrors”.
2. Change hotkey, Shift+Delete to delete data, Ctrl+Delete to delete file and data.
3. Change logo and icons.
4. Rearrange menu items.
5. Add & update translation files.

**uGet 1.10.2: (2012-10-01)**
1. Display “unnamed URL” if no filename specified.
2. Add new hotkeys: Enter, Shift+Enter, Delete, and Shift+Delete.
3. Don’t assign filename even if program accept ‘–quiet’ argument.
4. Hide aria2 console window in Windows platform.
5. Program can build with gstreamer-1.0 (auto detect by autoconf).
6. update Italian translation file.

**uGet 1.10.1: (2012-09-16)**
1. Restart download if aria2 response “speed was too slow”.
2. Don’t assign filename if user doesn’t specify it by commandline or UI.
3. Show error message if uGet can’t connect to aria2 on startup. (about 7 to 10 sec)
4. Add “Website by: Michael Tunnell (visuex.com)” in about dialog.
5. Fix: program doesn’t save/restore summary visible settings.

**uGet 1.10: (2012-09-07)**
01. This version need GTK 3.4+ and GLib 2.32+.
02. Add global speed limits for aria2.
03. Add new option “Retrieve timestamp” in Download dialog.
04. Add new option “User Agent” in Download dialog.
05. Add Commandline Settings for some FlashGot users.
06. Add setting option “Apply recently download settings”. (Enable by default)
07. Change aria2 default arguments to “–enable-rpc=true -D –check-certificate=false”.
08. aria2 plug-in use argument “continue=true”.
09. aria2 plug-in can use user specified filename.
10. curl plug-in disable peer SSL certificate verification.
11. curl plug-in can keep user specified filename.
12. update French translation file.
13. Fix: program crash when user deleting files.
14. Fix minor bugs.

## Older Versions

Unfortunately, this list is not yet complete. The process of collecting items and dates for the older versions is on-going so for now this is where the page will end. I will update this page as soon as possible.
