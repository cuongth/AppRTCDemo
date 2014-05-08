AppRTCDemo
==========

Android client for http://apprtc.appspot.com

In desktop chrome, navigate to http://apprtc.appspot.com and note the r=<NNN> room
this redirects to.  Launch AppRTC on the device and enter the same <NNN> into
the dialog box.

Alternatively, replace the <NNN> from the desktop chrome into the following
command:
adb shell am start -n org.appspot.apprtc/.AppRTCDemoActivity -a android.intent.action.VIEW -d '"https://apprtc.appspot.com/?r=<NNN>"'
This should result in the app launching on Android and connecting to the apprtc
page displayed in the desktop browser.

Yet another way to is to send the apprtc room URL to the Android device
