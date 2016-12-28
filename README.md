# RiseAndShine
An accompanying Android app for controlling alarms on the ENGR 1620 project of the same name.

## The Project
Originally conceived to tackle the issue of auditory alarms being ineffective for people with diminished or lost sense of hearing. This developed into a system that rapidly inflates a pillow under the user's head to displace them out of sleep.

Components:
* Android app
* Arduino Uno w/ Bluetooth module
* Electrical relay
* Air pump
* Rubber tubing
* Inflatable pillow

## The App
Allows the user to set a desired alarm time using a TimePicker, then sync with the Arduino.

Internally, it opens a BluetoothSocket hardcoded to communicate with the specific project Bluetooth module. Upon syncing the desired alarm, the app sends the Arduino an encoded string containing both the current time and the desired time.
