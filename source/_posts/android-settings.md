---
title: android settings
date: 2021-08-31 08:00:44
tags:
---
### turn on and turn off airplane mode:

Turn on:

adb shell settings put global airplane_mode_on 1
adb shell am broadcast -a android.intent.action.AIRPLANE_MODE
Turn off:

adb shell settings put global airplane_mode_on 0
adb shell am broadcast -a android.intent.action.AIRPLANE_MODE

### adb wifi
get wifi IP:
ifconfig

get device ID:
adb devices

set:
adb -s <device id> tcpip 5555​
adb connect <Wi-Fi IP>
