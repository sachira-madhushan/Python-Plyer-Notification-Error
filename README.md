# Python-Plyer-Notification-Error

Python plyer notification module error

Quection :
  My app is doing something weird. When the app sends a notification, it works just fine in the source    code when its run with vs code. But after compiling with pyinstaller, suddenly it doesn't work.

Answer :

>Add this raw when you compile the python program
  >>--hidden-import plyer.platforms.win.notification<<



Example :
  >>pyinstaller --onefile --windowed --hidden-import plyer.platforms.win.notification SiteBlocker.py
