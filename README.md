QR-PTT PushToTalk
=======

QR-PTT PushToTalk is an easy to use ptt over IP Android client for voice and text communication that uses the [Jumble] (https://github.com/Morlunk/Jumble) protocol implementation and has a GPLv3 license. It can be used by companies that need to be in constant communication with their employees (Lone Workers), to give instructions, make comments, report incidents in real time by voice communication or by sending a text message within the app.
<br/>To try it for free enter "demo" as User ID and leave User PIN field empty.*

Its main features are:
- Easy to use
- Fast and low latency real time voice communication
- Superior voice compression
- Works over 2G, 3G, 4G mobile data or Wifi
- Auto-reconnect feature when Internet connection is lost
- Dual-pane channel and chat with swipe left and right gestures
- Channel tree view
- View text comments/description for each user or channel
- Local mute users
- Chat notifications
- Automatic in app certificate generation for the server connection
- Opus codec support
- Private messaging
- 256 bit voice encryption
- Compatible with the latest version of Android 5.0 Lollipop
- Capacity of 5000 simultaneous users on server and 50 on each channel
- Automatic channel assignment
- QR-PTT stays active in background so you can use any other app of the phone and 
listen to your Workers in real time
- It can be used alongside with QR-Patrol guard tour app which tracks your guards or Lone Workers patrols in real time 

Downloads
---------------------
<br />
<strong>QR-PTT PushToTalk on Google Play</strong>

<a href="https://play.google.com/store/apps/details?id=com.terracom.qrpttbeta.free&hl=en">
  <img alt="Get it on Google Play" src="https://developer.android.com/images/brand/en_generic_rgb_wo_45.png" />
</a>

<br />


<strong>QR-PTT PushToTalk on Dropbox </strong>

<a href="https://dl.dropboxusercontent.com/u/25024443/QR-PTT PushToTalk.apk">
  <img alt="Get it from my personal Dropbox" src="https://cf.dropboxstatic.com/static/images/index/logo-vflme-Gvg.png" />
</a>

<br/>

<strong>QR-Patrol guard tour on Google Play</strong><br/>

<a href="https://play.google.com/store/apps/details?id=com.terracom.gr.kerverosqrpatrol">
  <img alt="Get it on Google Play" src="https://developer.android.com/images/brand/en_generic_rgb_wo_45.png" />
</a>  
<br/><br/>

*Keep in mind that any communication through the demo channel is public. 


<br/>
Building on GNU/Linux
---------------------

Make sure you have the following installed on your linux machine: Android Studio, Oracle java,
ant, awk, make, git, the Android SDK and the Android NDK. Then fork or download the original github project created by Andrew Comminos at https://github.com/Morlunk/QRPushToTalk and execute the commands below:

    git submodule update --init --recursive
    ndk-build -C libraries/Jumble/src/main/jni/
    ./gradlew assembleDebug

This is necessary in order to download the libraries that the initial application uses.
Keep in mind that throughout the proccess you should use chmod command on the whole project file
to give it the right permissions. Finally, download the files of my project and overwrite the old
ones. If you encounter any problem throughout the procedure feel free to contact me.


Contributing	
============

Coding
------

Standard FOSS project procedure applies; fork and submit a PR or just write me a pm!

Please use Transifex for translations, not pull requests.
