Debian GNU/Linux 9.9 (stretch)

$ sudo apt-get install google-android-ndk-installer

$ export PATH=$PATH:/usr/lib/android-ndk

$ export NDK_PROJECT_PATH=.
$ ndk-build NDK_APPLICATION_MK=./Application.mk 
$ adb push libs/armeabi-v7a/main.out /data

adb connect 192.168.10.90:5555

 2078  adb shell netcfg
 2079  adb shell
 2080  adb tcpip 5555
 2081  adb connect 192.168.10.95:5555

LINKS

https://software.intel.com/en-us/articles/building-an-android-command-line-application-using-the-ndk-build-tools
https://github.com/libusb/libusb/tree/master/android
