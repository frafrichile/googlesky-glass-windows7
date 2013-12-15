googlesky-glass-windows7
========================

loading googlesky.apk with windows 7
Before we begin it is important that you already have the Android SDK.
Most importantly you need ADB (android debug bridge). 
You also need to be somewhat familiar with opening a new terminal window.

Download and Install the Android SDK (http://developer.android.com/sdk/index.html 

Go to the folder where you have the Android SDK (adt-bundle-windows-x86_64-20131030\sdk\platform-tools)
Hold Shift down and right click on the folder where you have ADB . 
The open terminal option becomes available if you hold down shift .
on the CMD terminal

type :
ADB devices ( make sure your device is visible) 
Adb shell am start –a android.intent.action.MAIN n-
adb shell dumpsys | findstr android.intent.action.MAIN
adb shell am start -a android.intent.action.MAIN -n com.google.android.stardroid/com.google.android.stardroid.activities.SplashScreenActivity 
At this point tap your Glass on and the app should be running.
You will need to “down swipe” on your glass to cancel the agreement window. 
If you see the app running, disconnect, go outside, and check this out at nighttime! 

source: http://www.gosphero.com/how-to-load-apps-on-google-glass/

note: I edited some commands to make this work on windows 7
all credits go to "Official Orbotix SDK and Samples"
https://gist.github.com/orbotix

