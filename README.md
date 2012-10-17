# AACDecoder for Android
==================

This is a fork of:

Freeware Advanced Audio (AAC) Decoder for Android
http://www.spoledge.com

The original source code can be obtained at http://code.google.com/p/aacdecoder-android/

This is a port of the "OpenCORE aacdec" open source library to Android platform.

## Usage

### Preparing

You must copy both Java JAR and the shared library files to your
project's "libs" directory:

        $ cp -R decoder/libs <your_android_project>/libs

### Using


Please look at the example activity using the AAC decoder:

        player/src/com/spoledge/aacplay/AACPlayerActivity.java


## Summary How to build the the whole project - libs and apk.


### System Requirements

  * Android SDK - at least platform 3 (Android 1.5)
  * Android NDK - rev 6
  * Apache Ant - http://ant.apache.org/



### Getting Android OpenCORE Sources

You have to download Android OpenCORE sources either by:
  * downloading OpenCORE sources from the [Downloads] tab
  * checking-out Android OpenCORE sources from the Androids repository: http://android.git.kernel.org             
    * unfortunately this was working in summer 2011, but there is not an easy way how to download pure OpenCORE module now (spring 2012)
    * If anybody can provide me the full sources (OpenCORE only) I would appreciate it

  * checking-out OpenCORE aacdec sources from the original project: 
http://code.google.com/p/opencore-aacdec/

If you download a zip file, then please unzip it somewhere.



### Compiling

  * copy sample.ant.properties to .ant.properties and edit .ant.properties:
    * path to Android SDK
    * path to Android NDK
    * path to Android OpenCORE sources
  * run ```ant```
  * use the libraries and/or the APK:
    * install the APK on the emulator or a device: adb install player/bin/AACMusicPlayer-debug.apk
    * the Java and shared libraries you find in decoder/libs


## COPYRIGHTS


#### For this software the following license applies:


     AACDecoder - Freeware Advanced Audio (AAC) Decoder for Android
     Copyright (C) 2011, 2012 Spolecne s.r.o., http://www.spoledge.com
      
     This file is a part of AACDecoder.
    
     AACDecoder is free software; you can redistribute it and/or modify
     it under the terms of the GNU Lesser General Public License as published
     by the Free Software Foundation; either version 3 of the License,
     or (at your option) any later version.
     
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
     
     You should have received a copy of the GNU Lesser General Public License
     along with this program. If not, see <http://www.gnu.org/licenses/>.


#### NOTE-OpenCORE:
    This software uses libraries from the OpenCORE project under the Apache
    License, Version 2.0. (see decoder/jni/opencore-aacdec/Apache-LICENSE-2.0.txt).
    For more information about OpenCORE aacdec, please visit
    http://code.google.com/p/opencore-aacdec/


#### PLEASE NOTE

    That using of this software may require the payment of
    patent royalties. You need to consider this issue before you start
    building derivative works. We are not warranting or indemnifying you in
    any way for patent royalities! YOU ARE SOLELY RESPONSIBLE FOR YOUR OWN
    ACTIONS!

For more information about the AAC patents, please visit
http://www.vialicensing.com/licensing/AAC_index.cfm