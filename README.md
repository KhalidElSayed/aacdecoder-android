AACDecoder for Android
==================

This is a fork of http://code.google.com/p/aacdecoder-android

#summary How to build the the whole project - libs and apk.
#labels Featured

= System Requirements =

  * Android SDK - at least platform 3 (Android 1.5)
  * Android NDK - rev 6
  * (Apache Ant - http://ant.apache.org/)


= Getting Android OpenCORE Sources =

You have to download Android OpenCORE sources either by:
  * downloading OpenCORE sources from the [Downloads] tab
  * checking-out Android OpenCORE sources from the Androids repository: http://android.git.kernel.org             
    * unfortunately this was working in summer 2011, but there is not an easy way how to download pure OpenCORE module now (spring 2012)
    * If anybody can provide me the full sources (OpenCORE only) I would appreciate it

  * checking-out OpenCORE aacdec sources from the original project: 
http://code.google.com/p/opencore-aacdec/

If you download a zip file, then please unzip it somewhere.


= Compiling =

  # copy sample.ant.properties to .ant.properties and edit .ant.properties:
    * path to Android SDK
    * path to Android NDK
    * path to Android OpenCORE sources
  # run ant
  # use the libraries and/or the APK:
    * install the APK on the emulator or a device: adb install player/bin/AACMusicPlayer-debug.apk
    * the Java and shared libraries you find in decoder/libs

