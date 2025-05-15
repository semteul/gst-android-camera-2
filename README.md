# Gstreamer for Android Tutorial

* Android Studio Compatible
* Update gradle

# prerequisites
* Latest version of SDK
* gstreamer android prebuilt 1.26.1
  * https://gstreamer.freedesktop.org/download/#android
    * Unzip the file (place it wherever you want)
* NDK version r25c

# How to build
* set `gstAndroidRoot` in gradle.properties, or set global variable `GSTREAMER_ANDROID_ROOT` as Unzipped gstreamer prebuilt directory's location

```
export GSTREAMER_ANDROID_ROOT = YOUR_GSTREAMER_FOR_ANDROID_ROOT
```

gstAndroidRoot must be set when the app is built directly with Android Studio, not from the terminal.

* Build with debug option
```
./gradlew buildDebug
```

* Install APP in your Android device
** Using a real Android device other than emulators is highly recommended ** 
```
./gradlew installDebug
```