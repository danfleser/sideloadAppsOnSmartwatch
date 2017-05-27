# sideloadAppsOnSmartwatch
Sideload apps on smartwatch with adb

1 anable usb debug on phone and on smartwatch
2. terminal:
adb forward tcp:4444 localabstract:/adb-hub
adb connect localhost:4444
adb devices => u need to see localhost:4444	device
adb -e install ~/Desktop/pdf.apk  - to install apks
adb -s localhost:4444 push ~/Desktop/prelimg/ /sdcard/0/ - to copy files
