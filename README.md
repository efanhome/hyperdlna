<h1 align="center">HyperDLNA</h1> 
<p align="center">Android Upnp/DLNA client</p>

<br>

## Introduction
* HyperDLNA is a free, simple and easy to use client for browsing UPnP and DLNA media servers.
* Media can be streamed or downloaded to the device.
* It focuses on delivering a simple and lightweight experience.
* It is fork of [slick-dlna](https://github.com/KernelCrap/android-dlna) with changed and added features.
* Supports Latest/Not Outdated Android Versions.

## Improvements
HyperDLNA is a fork of [slick-dlna](https://github.com/KernelCrap/android-dlna). It was forked due to following reasons:
1. Slick DLNA is unmaintained.
2. Slick DLNA doesn't provide any build scripts.
3. Slick DLNA doesn't target Latest/Not Outdated Android versions. Instead it targets very old Android SDK.
4. Lack of proper Mime handling. It opens Media files in browser.

HyperDLNA removes these limitations. 
1. Hyper DLNA is maintained.
2. Hyper DLNA is well structured modern Android Application can be built in Android Studio.
3. Targets SDK-29 (Requires Android 10+).
4. Provides proper Mime handling. Media can be streamed in Media Player or Downloaded.

## Installation
[APK](https://github.com/varbhat/hyperdlna/releases/latest/download/app-debug.apk) can be downloaded from [Releases](https://github.com/varbhat/hyperdlna/releases/latest). It is built on each push by Github Actions. Note that it is debug build and Google Play Store may warn you while installation.

## Building Application
This Application can be built in Android Studio or Command Line.
Please Refer:
1. [Build and run Application](https://developer.android.com/studio/run)
2. [Building Application in Command Line](https://developer.android.com/studio/build/building-cmdline)

## DLNA Server
[dms](https://github.com/anacrolix/dms) can be used to setup DLNA Server on Device. Serving Device and HyperDLNA-installed Android Device must be on same network. Check that network of HyperDLNA is not tunneled through any VPN. Transcoding in DLNA Server is not at all necessary because modern media players like [mpv-android](https://github.com/mpv-android/mpv-android) and [VLC](https://www.videolan.org/vlc/download-android.html) can play Media of High Resoultion(or any resoultion) and supports most codecs you ever need.

```bash
dms -noTranscode -path /path/to/serving/directory
```

## Icons
* [Elementary icons](https://danrabbit.deviantart.com/art/elementary-Icons-65437279)
* [Oxygen icons](https://github.com/KDE/oxygen-icons)

## License
* [Apache-2.0 License](LICENSE)
* Each of components have their own license
