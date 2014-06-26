android-obd-reader
========================

Android OBD-II reader designed to connect with Bluetooth Elm327 OBD reader.

I'm still migrating things over here, so keep with me :-)

## Prerequisites ##
- JDK 7
- Android Studio (tested on 0.5.5)
- Gradle 1.11
- Android SDK (API 19, Build tools 19.0.1)

## Test with device ##

Be sure to have the device connected to your computer.

```
cd whatever_directory_you_cloned_this_repository
gradle clean build installDebug
```

## Test with OBD Server ##

If you want to upload data to a server, for now, check the following:
* [OBD Server](https://github.com/pires/obd-server/) - a simple implementation of a RESTful app, compiled into a runnable JAR.
* Enable the upload functionality, by defining ```private static final boolean UPLOAD = true;``` in ```MainActivity.java```;
* Set proper endpoint address and port in class ```UploadAsyncTask``` defined in ```MainActivity.java```.

## Tested on ##

* Samsung Galaxy Nexus (Android 4.3)
* LG Nexus 5 (Android 4.4)
