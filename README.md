# Project Runner
An Android application using C++ through the Android Native Development Kit, Project Runner is a 2D
 Top-Down, endless running platformer where the player looks down at the player and leads their
 character through a never ending dungeon. Design inspired by Temple Run and art inspired by The
 Impossible Game, the player will use swipes to change lanes and directions in order to avoid
 obstacles to achieve a high score.

## Dependencies
**[JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)**

**[Apache Ant](http://ant.apache.org/bindownload.cgi)**

**[Android NDK](http://developer.android.com/ndk/downloads/index.html)**

**[Android SDK Manager](http://developer.android.com/sdk/index.html#Other)** - Android 5.1 (Lollipop)

Set JAVA_HOME environment variable to JDK (ex: C:\Program Files\Java\jdk1.8.0_45)

Set ANDROID_HOME environment variable to Android SDK (ex: C:\Android\sdk)

Ensure that the NDK, Ant, and Android SDK platform tools are in your Path environment variable
(ex: C:\android-ndk-r10e;C:\apache-ant-1.9.6\bin;C:\Android\sdk\platform-tools)

## Libraries
**[SDL2](https://www.libsdl.org/download-2.0.php)**

## How to build & install
##### Debug build
`ndk-build && ant debug install`

OR

`make install`

in the root folder.

##### Release build
Create a `local.properties` file in the root folder which contains the following:
```
ndk.dir=C\:/your/ndk/path/android-ndk-r11c
sdk.dir=C\:/your/sdk/path/Android/sdk
key.store=C\:/your/keystore/path/android.jks
key.alias=yourkeyname
```
Then in the root directory:
`ndk-build && ant release install`

## Code
Java source can be found in `/src` and C/C++ source can be found in `/jni/src`

Copyright Notice:
-----------------
The files within this zip file are copyrighted by Lazy Foo' Productions (2004-2015)
and may not be redistributed without written permission.

This project is linked against:
----------------------------------------
##### Windows:
SDL2

SDL2main

SDL2_image

SDL2_ttf

##### *nix:
SDL2

SDL2_image

SDL2_ttf
