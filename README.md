# ffmpeg_build_android
FFmpeg Build Shell Script

## Download NDK
You can get the ndk from [NDK 下载  |  Android NDK  |  Android Developers](https://developer.android.com/ndk/downloads) <p>
or Just using ***SDK Manager*** like this [安装及配置 NDK 和 CMake  |  Android 开发者  |  Android Developers](https://developer.android.com/studio/projects/install-ndk)
## Download FFmpeg
FFmpeg Github Repo is [https://github.com/FFmpeg/FFmpeg](https://github.com/FFmpeg/FFmpeg) <p>
or Just Get it from [ffmpeg.org](http://ffmpeg.org/download.html)

## Setup Script
```shell
// 0. export ndk path
$ export ANDROID_NDK_HOME=/path/to/ndk 

// 1.  move the script into ffmpeg root path
$ mv build_ffmpeg.sh ./ffmpeg/

// 2. open the dir
$ cd ./ffmpeg/
```

## Compile
```shell
$ ./build_ffmpeg.sh ./ $ANDROID_NDK_HOME darwin-x86_64
```
***WARN!!!***<p>
the script has ***3*** params!! 
1. 1 for ffmpeg path; 
2. 2 for ndk home; 
3. 3 for host platform,like linux-x86_64 or darwin-x86_64;
## Fetch Libs
if success,go to ``` ./android-libs ``` to get the libs


## What's More
The Script is From ```ExoPlayer/Ffmpeg```@[build_ffmpeg.sh](https://github.com/google/ExoPlayer/blob/release-v2/extensions/ffmpeg/src/main/jni/build_ffmpeg.sh)